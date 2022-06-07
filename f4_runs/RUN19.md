* 2022-03-30 - 2022-06-07

## Modifications

* Run with cell, same as RUN17
* Use ET1091 LCR meter for cell pressure gauge

## Results

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
