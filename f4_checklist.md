## F4 Checklist (2022-02-03)

#### magnets
* HS          130
* NMR         2534
* MC wire     2063

#### top boxes
* W0TA - I1 - V3
* W1TA - I2 - V4
* W2TA - I3 - V5
* W0UM - I4 - T1
* W1UM - I5 - T3
* W2UM - I6 - T4
* W1NM - I12 - T5
* W2NM - I11 - T6  broken
* MCTA - I7 - I8
* MCTF - I9 - I10/-sometimes works
* NMR magnet leads  V8
* HS magnet  leads  V9
* 0 Ohm             V10  (noise tests)

#### resistance bridge
* R1K    -- cryobridge CH1  48.422
* RSTILL -- cryobridge CH2  109.24
* R20K   -- cryobridge CH3  55.886
* RHE02  -- cryobridge CH4  49.426
* RHE04  -- cryobridge CH5  49.202
* RHE06  -- cryobridge CH6  50.094
* RHE08  -- cryobridge CH7  49.179
* RHE10  -- cryobridge CH8  49.562
* RMC    -- cryobridge CH9  65.111
* RMC2    -- cryobridge CH10 46.445
* RHE102  -- cryobridge CH11 47.751
* GMR1    -- cryobridge CH13 1153
* R20MK2  -- cryobridge CH15 44.437
* RSTILL2 -- cryobridge CH16 39.862

#### cryostat heaters and diodes
* Q20MK   -- pair 1 R0=100
* QMC1    -- pair 2 R0=132.2
* QMC2    -- pair 3 R0=115.5
* QSTILL1 -- pair 7 R0=131
* QSTILL2 -- pair 8 R0=122 R=900
* DSTILL  -- pair 6
* DBATH

#### cell heaters
* Q1 200R  - (heater broken)
* Q2 200R (was broken before?)
* Q3 200R
* Q4 200R

#### multiplexer (bath resistors, level meter, demag)
* RBATH01
* RBATH02
* RBATH03
* RBATH04
* RBATH05
* RBATH06
* RBATH07
* RBATH08 (He bath bottom)
* RBATH09 (magnet top)
* RBATH10 (magnet bottom)
* level meter
* demag_v
* demag_i
* demag_ps

#### pressure gauge
* pressure gauge

#### cryostat pressures (measured with RPI computer)
* press_traps      - back of rotary pump, input of N2 traps, 1.6bar merit gauge
* press_cond       - condensing line, 1.6bar merit gauge, 0.006->0bar
* press_1K         - 1K pot, 60mbar merit gauge, 10.63V->overload
* press_cell_panel - cell pressure, 1.6bar merit gauge, 0.036->0bar
* press_still      - still pressure, log!
* press_misc       - pirani gauges (started at RUN3)

#### "Green" connector
* IVC heater 77 Ohm, green 23-24
* He boiler 110 Ohm, green 21-22
* Pot filling line heater, 145 Ohm, 19-20
* demag PS heater 138 Ohm green 3-4

