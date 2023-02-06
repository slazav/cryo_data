## f4_2021 databases

Old databases are in f4db_2019

actual list gan by obtained by `device_c ask db list` command,
or using url `http://slazav.xyz:8095/list`.


### Pressure measurements in the pump room.

* press_1K -- 60mbar gauge on the still pumping line.
* press_cell_panel -- 40bar gauge on He3 panel. Not accurate at small pressures.
* press_cond -- 1.5 bar gauge on the condensing line.
* press_still -- Pirany gauge on the input ot rotary circulation pump.
* press_traps -- 1.5 bar gauge on the output of rotary circulation pump
* press_misc -- Switching box with many Pirany gauges on the gas handling system.

float: U[V]

Syncronized from databases on f4rpi computer. Values are stored in volts,
`f1` filter converts them to bar (mbar for still).

### Bath resistors:

Allen Bradley or similar resistors mounted in the He bath.

* Rbath1 -- 94 cm from IVC flange
* Rbath2 -- 74 cm from IVC flange
* Rbath3 -- 55 cm from IVC flange
* Rbath4 -- 39 cm from IVC flange
* Rbath5 -- 22 cm from IVC flange
* Rbath6 -- IVC flange
* Rbath7 -- magnet top
* Rbath8 -- magnet bottom
* Rbath9 -- bottom of He bath

float: R [Ohm]

Filter 1: temperature [K] calibrations done in 2019 run: Rbath5
calibrated against PT1000 + 4.2K, others are modified by
linear transformation to match 300K and 4K values.

Calibrations for magnet resistors are not accurate: they are of a
different type and non-monotonic (resistance minimum below room
temperature).


### Bath diode

* DBATH -- diode on IVC flange, near Rbath6. Measured with 10uA current
source and multiplexer.

type: FLOAT

columns: U [Ohm]

filter1: temperature [K], not very accurate below 45 K


### He level (cm)

* he_level -- cryogenics level meter

float: U [V], level [mm]

No output filters, calculated level is recorded as a second column.
This is done because change of the level meter is more probable then
change of the calibration.


### Demag

* demag_vi   -- measured voltage (V1), measured DVM output (V2)
  filter1: current, A
  filter2: field, T
  filter3: magnet voltage without voltage drop on leads

* demag_pc   -- "persistent current", same as demag_vi but updated only if demag_ps > 4

* demag_ps  -- persistant switch heater, measured voltage
  filter1: 0 or 1 depending on the heater state


### Cell pressure gauge

* press_cell_cap -- capacitance [pF], loss [nS]

### Resistance bridge

* R1K    -- original thermometer on 1K pot
* RSTILL -- original thermometer on still
* R20MK  -- original thermometer on 20mK plate
* RHE02  -- original thermometer on heat exchanger 2
* RHE04  -- original thermometer on heat exchanger 4
* RHE06  -- original thermometer on heat exchanger 6
* RHE08  -- original thermometer on heat exchanger 8
* RHE10  -- original thermometer on heat exchanger 10
* RMC    -- original thermometer on the mixing chamber (in the mixture)

* R1K2    -- second thermometer on 1K pot
* RSTILL2 -- second thermometer on the still
* R20MK2  -- second thermometer on 20mK plate (removed)
* RMC2    -- second thermometer on the mixing chamber (on )
* RHE102 -- second thermometer on HE10 (now removed)
* GMR1 -- GMR sensor above NMR magnet (RUN3..)
* GMR2 -- GMR sensor in HS magnet (RUN17..RUN19)

type: FLOAT
data: resistance [Ohm], temperature [K] (calibration in the resistance bridge), power [W]
filter1: Temperature calibration (except HE* and GMR*)
filter2: R/Rroom (for RHE*, R20MK, RMC)

There is a problem with time drift of all resistors. There are databases with manually
added room-temperature values used for scaling calibration:

* R1K_RT
* RSTILL2_RT
* RSTILL_RT
* R20MK_RT
* RHE02_RT
* RHE04_RT
* RHE06_RT
* RHE08_RT
* RHE10_RT
* RMC_RT
* RMC2_RT

type: FLOAT
data: R [Ohm]

### Heaters
* heater1 -- cell heater 1
* heater2 -- cell heater 2
* heater3 -- cell heater 3
* heater4 -- cell heater 4
* heat_hs_shield -- Heater on the Nb shield of Heat switch magnet
* heat_still -- Still heater

type: FLOAT
data: voltage [V], power [W] (check!)

### Vibrating wires and forks, CW measurements

Wire names for Cell-2020:

* w0ta -- 0.127mm tantalum wire in the outer cell
* w1ta -- 0.127mm tantalum wire in the inner cell 1 (aerogel)
* w2ta -- 0.127mm tantalum wire in the inner cell 2 (empty)
* w0um -- 4.5um NbTi wire in the outer cell
* w1um -- 4.5um NbTi wire in the inner cell 1 (aerogel)
* w2um -- 4.5um NbTi wire in the inner cell 2 (empty)
* w1nm -- 450nm NbTi wire in the inner cell 1 (aerogel)
* w2nm -- 450nm NbTi wire in the inner cell 2 (empty)

Wire names for Cell-2022:

* w0ta2 -- 0.127mm tantalum wire in the outer cell -- broken
* w1ta2 -- 0.127mm tantalum wire in the inner cell 1 (aerogel)
* w2ta2 -- 0.127mm tantalum wire in the inner cell 2 (empty)
* w1a -- 4.5um NbTi wire in the inner cell 1 (aerogel)
* w2a -- 4.5um NbTi wire in the inner cell 2 (empty)
* w1bh -- 13.5um NbTi wire - bolometer heater in the cell 1
* w2bh -- 13.5um NbTi wire - bolometer heater in the cell 2
* w1bt -- 4.5um NbTi wire - bolometer thermometer in the cell 1
* w2bt -- 4.5um NbTi wire - bolometer thermometer in the cell 2
* w1b -- 0.350um NbTi wire (classic design) in cell 1
* w2b -- 0.180um NbTi wire (classic design) in cell 2 - broken
* w1c -- 0.390um NbTi wire (PCB design) in cell 1 - broken
* w2c -- 0.315um NbTi wire (PCB design) in cell 1 - broken?
* w2d -- 0.180um NbTi wire (PCB design) in cell 2 - ?

Other names:

* mcta -- 0.127mm tantalum wire in the miing chamber
* mctf -- tuning fork in the mixind chamber

Databases:
* `<name>` -- fit result: Tcnt,drive volt,Err,A,Ae,B,Be,C,Ce,D,De,F,Fe,dF,dFe [X4 Y4 F-F0]
* `<name>_pars` -- sweep parameters: T0, TE-T0, F1, F2, N, dt, dtf, dir, drive volt, drive ph
* `<name>_dbox`  -- drive box parameters: type:INT32, data: Rbox [Ohm], attenuator [dB]
* `<name>_sweeps` -- sweep data: time[s], freq[Hz], X1[V], Y1[V], Drive[V]
* `c_<name>_n`  -- calibration table for normal phase: W,P0,T0,P1,T1,...
* `c_<name>_b`  -- calibration table for B-phase: W,P0,T0,P1,T1,...



Measurement program can have a pre-measured background. Original values
from lock-in are X1, Y1. Values after background is subtrackted is X2,
Y2. In the tracking mode offset found in the fit is also subtracted
(values X3,Y3), values are rotated to the direction of applied force (X4,Y4)

Change 2023-01-20 in `<name>_sweeps` database (does not affect old data):
* Old columns: "time, freq, X1, Y1" in sweep mode, "time, freq, X3,Y3" in tracking mode.
* New columns: "time, freq, X1, Y1 [, X2, Y2]" in both modes. X2,Y2 are recorded only if the pre-measured background was used.

Change 2023-01-29 in `<name>` database:
* in tracking mode "X4 Y4 F-F0" values are added

Change 2023-02-06 in `<name>_sweeps` database (old data is modified):
* always "time, freq, X1, Y1, Drive"

Filters:
* <name>:f1 -- temperature calibration [mK] and T/B [mK/T]


### CW NMR data

In first runs there were 4 NMR thermometers on cell nuclear stage blocks.
Databases are similar to CW fork databases

* `nmr<n>cw`
* `nmr<n>cw_pars`
* `nmr<n>cw_sweeps`

with `<n>` = 1,2,3,4

### Magnets

* magnet_mc -- Mixing chamber magnet (data: Iset [A], Imeas [A], Vmeas [V])
* magnet_mc_a -- auto text comments

* magnet_hs -- Heat switch magnet
* magnet_hs_a

* magnet_nmr -- NMR/Compensation magnets
* magnet_nmr_a

### Other

* cell0_phase -- manually added liquid phase in cell0 (1 - vacuum/gas, 2 - normal liquid, 3 - superfluid liquid)
* cell1_phase -- same for inner cell 1
* cell2_phase -- same for inner cell 2
* cell_press  -- manually added pressure in the cell, bar
* comments    -- comments (type: TEXT)

* volt_hs -- voltage measured at the heat switch magnet
* leak -- signal from leak detector (leak rate, pressure)

