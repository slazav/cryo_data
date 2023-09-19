----------------------------------------------------------------------
## RUN1 17.12.2019 - 22.01.2020

- No cell.
- Old resistance bridge (Oxford) replaced by LakeShore 370AC with 16-channel scanner.
- Additional thermometers added.


### Results

Cryostat

- He level meter is bad. Should we order new one?

Dilution refregirator:

- condensing lines blocking: condensing pressure increased twice
during 20 days of work at lines 3 and 4. If lines are half-blocked
condensing pressure strongly drops during He transfer.

- Heat exchanger thermometers 10 and 6 are much more sensitive to
vibrations then others

- Mixing chamber thermometer is badly filtered (worse then heat exch.
thermometers?)

- CW wire measurement:
    - Drive currnet: 1.0V / 1100Ohm
    - Magnet 3A (in old measurements it was 5A)
    - sweep rate 100 mA/s heats mixing chamber

- Pulse wire measurement: no results yet

- DilutionHeat: test dilution refregirators regimes at different Qmix, Qstill
Low- and High- circulation regimes. Optimal circulation is between 40 and 70 umol/s.
Lowest temperature 3.5 mK.

### Thermometer calibrations

 Bath thermometer \#6 (vacuum can flange) was calibrated using PT1000
attached to it and 4.2K point. Bath resisters \#2..\#9 calibrations was
obtained by linear scaling of \#6 calibration to fit 300K and 4.2K points.
Bath resistor \#1 calibration was obtained by shifting \#6 calibration to
fit 300K point.

Bath diode was calibrated using PT1000. Calibration slightly differs from
the original calibration (possible reason: finite input resistance of the
ADC wich is 1 MOhm).

### Resistance bridge channels:

* CH1: 1K pot, original thermometer.
  Red connector 1,16 + 14,15 common.
  STATUS: works
  TODO: calibrate high temperaures vs PT1000

* CH2: 20 mK, original thermometer.
  Red connector 2,17 + 14,15 common.
  TODO: calibrate high temperaures vs PT1000
  TODO: make some reasoable calibraton of all HeatExch thermometers

* CH3: Heat Exchanger 2, original thermometer.  50 Ohm
  Red connector 3,18 + 14,15 common.

* CH4: Heat Exchanger 4, original thermometer.  50 Ohm
  Red connector 4,19 + 14,15 common.

* CH5: Heat Exchanger 6, original thermometer.  50 Ohm
  Red connector 5,20 + 14,15 common.

* CH6: Heat Exchanger 8, original thermometer.  50 Ohm
  Red connector 6,21 + 14,15 common.

* CH7: Heat Exchanger 10, original thermometer. 50 Ohm
  Red connector 7,22 + 14,15 common.

* CH8: Mix.Ch., original thermometer. 65 Ohm
  Red connector 8,23 + 14,15 common.

CH1-CH8 Two common wires and two individual wires down to 4K connector (in the VC),
then 1 common and 1 individual (~55 Ohm per wire).
CH2-CH7 has a 100nF filtering capacitors at 20mK plate.
CH8 has RC filters, about 300 Ohm per wire.

* CH09: PT1000 at 1K pot.
  Blue connector 11,12 + 1,2 common

* CH10: Still, original thermometer.
  Blue connector 3,10 + 1,2 common

* CH11: PT1000 at 20mK
  Blue connector 19,20 + 1,2 common

* CH12: RuO 1.2 kOhm resistor (Farnell:2447275) at 20mK shield.
  Blue connector 21,23 + 1,2 common.
  STATUS: stopped working at some point

* CH13: RuO resistor (marked "F.4 MC 11/2016 38 Ohm")
  Lowest SMB connector on Mix.Ch.
  Conectors I5,I6, 4-wires down to Mix.Ch.

* CH14: RuO resistor (marked "F.4 outer cell 11/2016 66 Ohm")
  Magnetic connector on Mix.Ch.
  Conectors I9,I10, 4-wires down to Mix.Ch.

* CH15: PT1000 at Mix.Ch. (silver wire to V connectors)
  Connectors I11,I12, 4-wire measurement.

* CH16: Speer 47.8 Ohm (grinded to 109 Ohm) on Mix.Ch, same location as PT1000.
  Connectors V11,V12, 4-wire measurement.

### Diodes

* Still: Blue conn. 8+,9 -- 0.72V

* 4K: Green conn. 17+,18 -- 0.66V

### Heaters

* Mix.Ch. heater 1, 58 Ohm (278 at BNC panel)
  Blue connector, 13,14

* Mix.Ch. heater 2, 55 Ohm (261 at BNC panel)
  Blue connector, 15,16 (16=14)

* 20mK heater, 118 Ohm (243 at connector)
  Red connector, 11,12

* Still heater 1, 122 Ohm (237 at BNC panel)
  Blue connector, 4,5

* Still heater 2, 131 Ohm (247 at BNC panel)
  Blue connector, 6,7

* IVC heater -- 76.4
  Green connector 23-24

* He3 boiler -- 100.0 (107.3 on He connector)
  Green connector 21-22

* Demag magnet switch
  Green connector, 3,4

### Wires

* Mix.Ch.: connectors I7, I8,   384 Ohm at connectors

### GMR sensors (from previous cooldown), NVE AA002-02e

* Vertical: connectors I1,I2  4.86 kOhm at connectors
* Radial:   connectors I3,I4  4.98 kOhm at connectors

### Magnets:

Mix.Ch. fork: 2064 kOhm

### Bath thermometers

* R1 94 cm from 4K flange  156.7  green 7,8
* R2 74 cm from 4K flange  148.2  green 7,9
* R3 55 cm from 4K flange  164.1  green 7,10
* R4 39 cm from 4K flange  150.4  green 7,11
* R5 22 cm from 4K flange  166.1  green 7,12
* R6  0 cm from 4K flange  156.6  green 7,13
* R7  dewar bottom  (193.3 on He conn)  green 7,14
* R8 magnet 1  green 7,15
* R9 magnet 2  green 7,16
* PT1000 at #6, green 5,6



----------------------------------------------------------------------
##  RUN2 18.03.2021 - 20.04.2021

### Modifications

First run with aerogel cell. Many modifications (new thermometer/heater wiring,
new 20mK radiation shield, niobium shields, modified pumping system).

### Results

All vibrating wires work. Problem with magnet wiring (heat connection
between Mix.Ch, 20mK plate and Still), lowest temperature ~20mK.
Measurements of vibrating wires in 4K and 20mK in vacum, filling cell.
Something strange with magnets/shields. No NMR signal. Run finished
because of cold leak.



----------------------------------------------------------------------
## RUN3 23.04.2021 - 06.05.2021

### Modifications

Magnet wiring fixed. IVC feedthoughs covered with stycast (to close
possible leak).

### Results

Found NMR signal from Cu thermometers, too wide lines.
Investigating shields, magnets. 20mK shield and NMR magnet shield are quenching
when ramping demag magnet. Stopping cryostat for removing shelds.



----------------------------------------------------------------------
## RUN4 06.05.2021 - 01.06.2021

### Modifications

Niobium shields (20mK and Mix.Ch) removed.

### Results

Filling the cell. Found that HS magnet shield is also quenching when
ramping demag magnet. Find how to protect the sheld with NMR magnet.
Run finished because of cold leak. Searching for the leak at 77 and 4 K.



----------------------------------------------------------------------
## RUN5 03.06.2021 - 11.06.2021

Changing soap seal, putting stycast of silver wires.
Run finished because of cold leak after one day of circlation.



----------------------------------------------------------------------
## RUN6 11.06.2021 -16.06.2021

Cooldown without cell, magnet, radiation shields. Testing cryostat with
He4. No leaks.



----------------------------------------------------------------------
## RUN7 18.06.2021 - 24.06.2021

Silver wires on MC flange fixed with Stycast (remove old sycast around
wires with Dremel, put new one).

Leak after 2h of mixture condensing. Measuring vibrating wires at 4K, at
small pressures. Cell2 is partially blocked (bad flushing before the
run?).



----------------------------------------------------------------------
## RUN8 28.06.2021-16.07.2021

Fully open MC flange (cut bottom part of heat exchangers), cover it
with Stycast. Cover bottom part of MC with Stycast.

Cryostat is leaking; cell is leaking.



----------------------------------------------------------------------
## RUN9 23.08.2021-28.09.2021

Leaks in the cruostat are fixed! (leak in the cell cone flange + leak in
HS2). HS magnet wiring is broken (quench at 40mA). W2NM is broken. R20MK2
is broken. Cell is leaking.

Measuring wires at 4 K



----------------------------------------------------------------------
## RUN10 01.10.2021-04.10.2021

Fix HS magnet(?). Fix thermalization of magnet wiring. Fix R20MK2
thermometer. Resolder cell filling lines. Use B coax cable for MCTF
signal. Leak in the cell at 130K



----------------------------------------------------------------------
## RUN11 15.10.2021- - 19.10.2021

Fix cold leak in the cell flange with white stycast(?). MCTF is broken.
Leak in the cell open at >130K.



----------------------------------------------------------------------
## RUN12 02.11.2021 - 08.11.2021

Fill upper part of the cell flange with black stycast.

Leak in the cell open at 10K, closed at ~200K.



----------------------------------------------------------------------
## RUN13 12.11.2021 - 16.11.2021

Fill upper part of the cell flange with soap seal.

Leak in the cell open at >120K, closed at 220K.



----------------------------------------------------------------------
## RUN14 02.12.2021 - 06.12.2021

Rebuild upper part of the cell. New cell heaters. MCTF fixed. Remove NMR
thermometers.

Cold leaks in both cryostat and the cell at >120K.



----------------------------------------------------------------------
## RUN15 2022-01-06 - 2022-01-12

### Modifications

Cell covered with black stycast. Filling lines moved to cell
bottom. Cell connection to MC tightened.

### Results

- leak at 10K


----------------------------------------------------------------------
## RUN16 2022-02-03 - 2022-02-28

### Modifications

Re-make cell filling lines (different Stycast)

### Results

* No leaks!
* Cryostat is working, but not very good (10mK base temperature, not stable)
* HE6 is most sensitive to vibrations
* Second themometer on HE10 shows too high temperature

* All wires are working except w2nm
* calibration of MCTA and W*TA are slightly different (9.5 vs 8 mK)
* Magnets are working (NMR=+1200, HS up to +/-4000mA, MC=+1500mA)
* HS shield is quenching, can't magnetize properly

* Main magnet inverted? Check! -- No.

### Measurements

* All wires vs drive and field at vacuum, 10mK
* Wire measurements at 4K: all tantalum wires vs field, all cell wires vs pressure.

----------------------------------------------------------------------
## RUN17 2022-03-07 - 2022-03-16

### Modifications

* New heater on HS Nb shield: 40um constantan wire, 317 R.
  leads: single-core supercond. in CuNi clad, 12.8 R/wire.
* Mu-metal shield (unknown grade, from storage) around HS Nb shield.
  Five plates 25x30x1mm covered with kapton tape.
* GMR2 sensor: AA002-02E
  wiring: 1V+ 5V- 4I- 8I+. cable: 2 pairs CuNi, 19 R/wire
  Chan 14 of ResBridge (chan 12 is broken).
  The sensor is inside HS magnet.
* Check wires of HE10R2 thermometer, 10 R/wire. Remove the thermometer.
* Kapton tape on heat exchangers.
* CuNi shortcut on NMR magnet, 2.5R (~150ms calculated time constant).

### Results

Leak in IVC (He4) after starting circulation



----------------------------------------------------------------------
#RUN18 2022-03-18 - 2022-03-29

### Modifications

* Run without cell

### Results

Cryostat working, 3.5mK


----------------------------------------------------------------------
## RUN19 2022-03-30 - 2022-06-07

### Modifications

* Run with cell, same as RUN17
* Use ET1091 LCR meter for cell pressure gauge

### Results

Demag measurements at P = 0 and 4.35 bar

- Cryostat, cell and all wires (except w2nm) work.
  Cell1 is leaking to outer cell.

- 2022-04-05 demag1 (70A), starting from 12 mK. Try to keep GMR2 near zero.
  HS does not work, big heating of MC because of shield quenches.
  Lowest temperature about 3mK.
  Learn how to heat shield above Tc without evaporating cell and cryostat.
- 2022-04-10 demag2 (65A), lowest temperature 0.240mK
  Found that cell1 is leaking to the outer cell.
  Check cell heaters, explore heat leaks
- 2022-04-17 demag3 (71A), lowest temperature 0.168mK
  Measure w2ta, w2um resonances as a function of drive
- 2022-04-28 demag4 (71A) with long precooling, lowest temperature 0.122mK (0.270 in cell1)
- 2022-05-09 demag5 (71A) lowest temperature 0.117mK (0.216 in cell1), fast heating measurements
- P=4.35 bar
- 2022-05-19 demag6 (71A) failed (demag to 0)
- 2022-05-23 demag7 (71A) failed (probably, field trapped in HS shield)
- 2022-05-30 demag8 (71A) lowest temp 0.22mK/0.15Tc (0.51mK in cell1)

- 2022-06-07 broken PS of MC magnet -> magnet quench -> cell is broken

Dilution fridge with disconnected HS:
- 0.3V  3.40mK
- 0.5V  5.51mK
- 0.65V 6.72mK

## Problems

* Condensing lines are blocking. It helps to switch lines during transfer
* Cryostat works badly at large condensing line pressure >0.57bar.
* MCTA extra resonance at high demag field (not always!)
* Strange field profiles
* Big field-dependent heat leak to cell0
* OVP on Tenma PS does not always work (software OVP is needed)
* PST3 is broken
* cell is broken after the run

----------------------------------------------------------------------
## RUN20 2022-09-07 - 2022-09-20

### Modifications

* Install cell2022

### Results

* leak in the cryostat (He3 input in MC)

----------------------------------------------------------------------
## RUN21 2022-09-28 - 2022-11-09

### Modifications

* Fix leak in MC

### Results
- 2022-10-10 demag1: large amount of He4 in the cell
- 2022-10-13..19 - cleaning He3
- 2022-10-26 demag2: lowest temperature 140uK in cell2,
  200uK in cell1 (heater was connected, big heat leak!)

## Problems

* W0TA does not work
* small overheating of MC by COMP magnet

----------------------------------------------------------------------
## RUN22 2023-01-04 - 2023-06-23

### Modifications

* remake COMP magnet wires (Cu - CuNi connection)
* make ground for coaxial lines (~20 cm of 0.2mm NbTi in CuNi matrix)
  -- no result, MCTA background is still high, 12uV at 0.1V (4.2uA) excitation

* revert I2 and T wire connectors, fix broken w2b wire (not important as the wire is broken)
* connect V12 and T6 at 4K, now w2d can be measured through T6 transformer

### Measurements

* wire backgrounds w/o field from 15K to 20mK
* wire resonances at <20mK
* field dependence (thin wires at low field, Ta wires at all fields)

* 0bar, 2bar, 5bar pressures

----------------------------------------------------------------------
## RUN23 2023-06-29 - 2023-07-06

Leak in IVC

----------------------------------------------------------------------
## RUN24 2023-08-18 - 2023-08-22

### Modifications

* fixing leak in the IVC feedthrough
* fixing leak in He bath (o-ring of the bottom Lemo connector)
* heater on condensing lines 3 and 4

Leak in IVC

----------------------------------------------------------------------
## RUN25 2023-08-23 - 2023-08-25

One more attempt to glue broken feedthrough.
Leak in IVC - bigger and faster then at RUN24.

----------------------------------------------------------------------

## RUN26 2023-09-12 -

* new feedthrough

