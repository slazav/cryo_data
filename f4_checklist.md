## F4 Checklist

RUN20 09.2022

#### magnets
* HS          134  +
* Shield      1080 +
* MC          2066 +

#### top boxes
* w1bh -  I1 - V1 +
* w2bh -  I2 - V2 +
* w1ta -  I3 - V3 +
* w2ta -  I4 - V4 +
* w1c  -  I5 - V5 + (!)
* w2c  -  I6 - V6 + (!)
* w1bt -  I7 - T1 ?
* w2bt -  I8 - T2 ?
* w1a  -  I9 - T3 ?
* w2a  - I10 - T4 ?
* w1b  - I11 - T5 ? (!)
* w2b  - I12 - T6 ? (!)

* HSS magnet leads + V8
* HS magnet  leads + V9
* w2d  - V11 - V12 + (!)

#### resistance bridge
* R1K     -- CH1  48.422 +
* RSTILL  -- CH2  109.24 +
* R20K    -- CH3  55.886 +
* RHE02   -- CH4  49.426 +
* RHE04   -- CH5  49.202 +
* RHE06   -- CH6  50.094 +
* RHE08   -- CH7  49.179 +
* RHE10   -- CH8  49.562 +
* RMC     -- CH9  65.111 +
* RMC2    -- CH10 46.445 +
* GMR1    -- CH13 1153   +
* RSTILL2 -- CH16 39.862 +

#### cryostat heaters and diodes
* Q20MK   -- pair 1 R0=100   +
* QMC1    -- pair 2 R0=132.2 +
* QMC2    -- pair 3 R0=115.5 -
* QHSS    -- pair 4 R0=317   +
* QSTILL1 -- pair 7 R0=131   +
* QSTILL2 -- pair 8 R0=122 R=900 +
* DSTILL  -- pair 6          +
* DBATH

#### cell heaters
* Q1 200R  +
* Q2 200R  - wire broken
* Q3 200R  +
* Q4 200R  +

#### multiplexer (bath resistors, level meter, demag)
* RBATH01  +
* RBATH02  +
* RBATH03  +
* RBATH04  +
* RBATH05  +
* RBATH06  +
* RBATH07  +
* RBATH08  + (He bath bottom)
* RBATH09  + (magnet top)
* RBATH10  + (magnet bottom)
* level meter  +
* demag_v  +
* demag_i  +
* demag_ps  +

#### coax cables
* R+G  W0TA  -
* B+Y  MCTA  +
* W+K  pressure gauge ~17pF +

#### cryostat pressures (measured with RPI computer)
* press_traps      + back of rotary pump, input of N2 traps, 1.6bar merit gauge
* press_cond       + condensing line, 1.6bar merit gauge, 0.006->0bar
* press_1K         + 1K pot, 60mbar merit gauge, 10.63V->overload
* press_cell_panel + cell pressure, 1.6bar merit gauge, 0.036->0bar
* press_still      + still pressure, log!
* press_misc       + pirani gauges (started at RUN3)

#### "Green" connector
* IVC heater 77 Ohm, green 23-24 +
* He boiler 110 Ohm, green 21-22 +
* Pot filling line heater, 145 Ohm, 19-20 +
* demag PS heater 138 Ohm green 3-4 +
