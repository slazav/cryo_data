## F4 Checklist (2021)

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
* W1NM - V1 - T5?
* W2NM - V2 - T6?
* MCTA - I7 - I8
* MCTF - V11 - (V12)  -> V12 changed to coax B
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
* R1K2    -- cryobridge CH11 47.751 -- RHE102 in RUN4
* GMR1    -- cryobridge CH13 1160  -- RUN3
* R20MK2  -- cryobridge CH15 44.437
* RSTILL2 -- cryobridge CH16 39.862

#### cryostat heaters and diodes
* Q20MK   -- pair 1
* QMC1    -- pair 2 R=132.2
* QMC2    -- pair 3 R=115.5
* QSTILL1 -- pair 7
* QSTILL2 -- pair 8
* DSTILL  -- pair 6
* DBATH  4.399V

#### cell heaters
* Q1 - cryobridge CH13  341.7
* Q2 - cryobridge CH14  348.4
* Q3 - cryobridge CH15  354.0
* Q4 - cryobridge CH16  349.7

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
* press_traps      - back of rotaty pump, input of N2 traps, 1.6bar merit gauge, ch A: 
* press_cond       - condensing line, 1.6bar merit gauge, ch B: 0.006->0bar
* press_1K         - 1K pot, 60mbar merit gauge, ch C: 10.63V->overload
* press_cell_panel - cell pressure, 1.6bar merit gauge, ch D: 0.036->0bar
* press_still      - still pressure, log!
* press_misc       - pirani gauges (started at RUN3)

#### "Green" connector
* IVC heater 77 Ohm, green 23-24
* He boiler 110 Ohm, green 21-22
* Pot filling line heater, 145 Ohm, 19-20
* demag PS heater 138 Ohm green 3-4

#### NMR RF coils
* T1E - I9
* T2E - I10
* T3E - I11
* T4E - I12
* T1S - R coax line  140
* T2S - G coax line  140
* T3S - B coax line  -   -> MCTF
* T4S - Y coax line  140
