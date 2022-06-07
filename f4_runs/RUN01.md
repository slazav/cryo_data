###  RUN1 17.12.2019 - 22.01.2020

- No cell.
- Old resistance bridge (Oxford) replaced by LakeShore 370AC with 16-channel scanner.
- Additional thermometers added.


## Results

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

## Thermometer calibrations

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
