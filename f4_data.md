## F4 and Aerogel project parameters. 2021..2022


### Cryostat

* Build by DIB and GRP, cryostat: 1984-85, frame and shielded room: 1987, mixing chamber: 1988.

#### Dilution refrigerator
* Circulation pump 1: Ruvac roots WS501, 11732, nom.pumping speed: 505m^3/h, max dP: 80mbar
* Circulation pump 2: Alcatel 2063h s.n. 615141 (2 stages, 60m^3/h)

* Tank volumes: 50+100+150+200 l
* Pump back volume: 7.21 l, blue line volume: 0.135 l.
* Rot.Rump front volume: 6.02 l
* N2 traps volume (in cold state): 10.36 l
* Amount of mixture: 229 L
* 2022.10 - added 9.9l of He3 and (return) 3.5l of He4 from the cell
* Amount of mixture in the fridge when still gets empty: 168l

* MCTF 4K, vacuum:    32682.02 Hz - 0.105 Hz
* MCTF 300K, vacuum:  32727.00 Hz - 0.789 Hz
* MCTA 4K, vacuum: 1094.28 Hz  - 77.8 mHz

Typical circulation regimes:
* Vstill=0.3V, lines 1+4, Pcond = 103.8mbar, ndot =  70.1 umol/s
* Vstill=0.6V, lines 1+4, Pcond = 462.9mbar, ndot = 220.9 umol/s


#### Magnet v1 (1987)
* 8T, Oxford, 1987
* Max current: 71.45A == 8T.
* Bore diameter: 90.5mm
* 0.112 T/A, 18.365 mV/T, 54.45 mT/mV
* Cancellation region: 14.4 cm above field center, 2mm above magnet top flange
* L=23H

#### Dewar v2 (2004)
* Precision Cryogenic Systems, 2004
* total height 83", diameter 24.13"
* He bath diameter 7.5", bottom length 34", belly length 24", top length 20"
* N2 tank: 110 l, He belly: 100 l.


### Wires

#### Resistance bridge and cryostat heater wires (built in 2020)
* previosly "Red" and "Blue" connectors
* 48 twisted pairs in 6 blocks
* Filters: ...

#### Vibrating wire lines
* "White", "Black" and "Yellow" connectors
* 12 "V" pairs, 12 "I" pairs, 6 cold transformers (previously 8)

* Femto LIA-BVD-150H lock-ins, 15pcs in 3 19" blocks, rebuilt in 2020-2022:
  - remove internal power supply, add metal sheilds,
  - new PCB, better coax lines inside lockins,
  - rear-panel connectors for output (LEMO) and power (3 pin XLR)
* Lock-in output cables: 3 cables (one per block)
  - cable: Alpha Wire 10 Pair Screened Multipair Industrial Cable 0.23 mm, RS:1119010
  - LEMO connectors (10pin): EGG.2B.310.CLL / FGG.2B.310.CLAD92Z (RS:1789029 / RS:1788896)
  - 1: orange-black, 2: brown-black, 3: yellow-black, 4: white-black, 5: blue-black
    6: green-black,  7: red-black,   8: blue-red,     9: green-red,  10: white-red
  - Pair grounds are not connected on LEMO side, cable ground connected to lock-in
    ground with a separate connector.
  - There is a mistake in cable 3, pair 8: ground is blue insrterd of red!
* Two Pico ADC-24 devices (adc1, adc2) with 1:3 dividers
  - Divider R1: Vishay 10k Metal Film Resistor 0.125W 0.1% PTF5610K000BYEK, RS:8307422
  - Divider R2: Vishay 40k Metal Film Resistor 0.125W 0.1% PTF5640K000BYEK, RS:8498985
* lockin output - cable-pair - ADC input
  - 01X -- 1-01 -- ADC1-01  06X -- 2-01 -- ADC1-11  06X -- 2-01 -- ADC2-05
  - 01Y -- 1-02 -- ADC1-02  06Y -- 2-02 -- ADC1-12  06Y -- 2-02 -- ADC2-06
  - 02X -- 1-03 -- ADC1-03  07X -- 2-03 -- ADC1-13  07X -- 2-03 -- ADC2-07
  - 02Y -- 1-04 -- ADC1-04  07Y -- 2-04 -- ADC1-14  07Y -- 2-04 -- ADC2-08
  - 03X -- 1-05 -- ADC1-05  08X -- 2-05 -- ADC1-15  08X -- 2-05 -- ADC2-09
  - 03Y -- 1-06 -- ADC1-06  08Y -- 2-06 -- ADC1-16  08Y -- 2-06 -- ADC2-10
  - 04X -- 1-07 -- ADC1-07  09X -- 2-07 -- ADC2-01  09X -- 2-07 -- ADC2-11
  - 04Y -- 1-08 -- ADC1-08  09Y -- 2-08 -- ADC2-02  09Y -- 2-08 -- ADC2-12
  - 05X -- 1-09 -- ADC1-09  10X -- 2-09 -- ADC2-03  10X -- 2-09 -- ADC2-13
  - 05Y -- 1-10 -- ADC1-10  10Y -- 2-10 -- ADC2-04  10Y -- 2-10 -- ADC2-14
* Shielded twisted pairs with TinyXLR connectors: 1:+ 2:gnd 3:-

* Generators ...
* Drive boxes ...

#### Coaxial lines
* 6 lines: R G B Y B K

#### Magnet lines
* original MCTA magnet line + two extra lines (HS and NMR)
* Filters: ...

#### "Green" connector

#### Level meter

#### Main magnet leads


### Devices

#### on the rack
* Cryogenic PS120A demag power supply
* Cryogenic HGL200 He level meter
* Keysight 34972A multiplexer [mult1] -- bath resistors, demag ps, level meter
* Tenma 72-2540 power suppliees [pst1..pst4] -- pst3 broken (06.2022), pst1 have broken comp.control
* LakeShore AC370 resistance bridge [rbridge] with 16ch switch -- also Still heater and other heaters
* Agilent E3631A power supply for Femto lock-ins
* EasyTester ET1091 LCR meter [] -- for measuring pressure gauge
* Keysight 33521A generators [gen1..gen4]
* Agilent 33220A generators [gen5..gen10]
* Sigent  SDG1032X generators [gen11..gen16]
* Keysight 34410A multimeter [mult1] -- bath diode and other measurements
* computer [f4b]
* UPS, MGE pulsar evolution 500 -- for computer and network switch
* network switch, Netgear, 24 ports -- internal network
* small DC power supply +5,+12V -- for USB hubs
* SR830 lock-in amplifiers [lockin1, lockin2]
* PicoScope 4262 (16bit, with generator) [osc1]
* PicoScope 4224 (12 bit) [osc2]
* PicoLog ADC [adc1, adc2] -- for measuring Femto lock-ins

#### on the cryostat flange
* Femto LIA-BVD-150-H lock-in amplifiers 5x3pcs
* Drive boxes


### Cell for Aerogel experiment (2020), upper part

#### Mixing chamber heat exchangers
* 6 sinter plates
* Size: 15x40x2mm (1mm of sinter on each side, 0.1 silver plate).
* Silver foil: Goodfellow AG000350/33, thickness: 0.1mm, purity: 99.95+%, temper: as rolled.
* Silver wire: Goodfellow AG005160/45, diameter 1.0mm, purity 99.99%, temper: annealed.
* Annealing of plate+wire: 18h, 800C, 3.8e-2 mbar of air.
* Powder: 50nm, 99.95% purity, Inframat Adv.Mat. 47MN-03, geometric surface area 10.9m^2/g
* Sinter weight: 6 g per plate.
* Sinter baking: 15..35 min at 152..158 C in vacuum/nitrogen.
* Sinter area: 25..30 m$^2$ per plate (measured with BET method).

#### Heat links
* Material: silver wire, Goodfellow AG005160/45, diameter 1.0mm, purity 99.99%, temper: annealed.
* Annealing: 18h, 800C, 3.8e-2 mbar of air, wires for welding to the heat switch was annealed second
    time: 18h, 850C, 3.8e-2 mbar of air.
* RRR: 23 before annealing, 452 after annealing.
* Resistance at 4K, after annealing: 0.483 $\mu\Omega$/cm
* Resistance of spot-welded connection, 4K: 1.43 $\mu\Omega$
* Resistance of spot-welded connection to Al, 4K: 1.13 $\mu\Omega$

#### Heat switch
* Material: aluminium, 99.999% purity, Goodfellow AL007920/26
* Dimensions: cylinder D=14mm, L=9.5mm, with 2mm-wide cylindrical groove in the center to D=6mm,
  halves are splitted into 6 and 8 parts by longitudinal cuts..

####Heat switch magnet
* Dimensions: Dout=24mm, L=26mm.
* Wire: 54S43(mu), 54 NbTi cores, Cu clad, Dcore=0.013mm, Dclad=0.152mm, Dinsul=0.178mm.
* 6 layers, 806 turns (136,136,132,132,134,136), glued with Stycast-1266.
* Nb shield: Din=28mm, Dout=30mm, L=30mm, ordered in Firmetal.
* Calculated field in the center: Bz = 146.74 G/A
* Calculated inductance: 14.2mH
* Time constant with 10R shunt: 1.42ms
* Quench current 4166mA @ 20mK

#### NMR thermometers (T1..T4) -- removed in 2021:
* Probe material: 99.99+% Goodfellow CU000570/3 0.1mm copper foil.
* 24 foils ~2.5x15mm, welded together, annealed, separated with stycast paper.
* Pick-up coil former: GRP, L=10 mm, ID=5 mm (bore 4 mm), OD=8 mm
* Pick-up coil: 50 um copper wire, 1600 turns (~110 Ohm, 11 mH)  (0.2T/A???)
* Excitation coil: 50 um copper wire, 20+20 turns (~10 Ohm, ~2 uH) (6mT/A???)

#### NMR thermometer magnet:
* Dimensions: L=47mm, D=52mm.
* wire: 54 NbTi cores (7um) in copper clad, 102um insulated (setting 107..110um on the machine)
* 6 layers, 2557 turns, glued with Stycast-1266.
* Nb shield: L=60mm, OD=58mm, ID=56mm, ordered in Firmetal -- removed in 2021.
* Calculated field: 11.1 mT/A (57.2 mT/A in the outer area)
* Calculated inductance: 0.37H
* Time constant with 10R shunt: 37ms
* calculated NMR frequency (for copper gyromagnetic ratio 71.118e6 rad/s/T): 125.6kHz/A
* Quench current 1590mA @ 4K, 1900mA @ 20mK
* 2022-03-02: CuNi short, 2.5 R.

#### Heaters-v1 (Feb-Nov 2021)
* Wire: Eureca, 46swg, 167 Ohm/m
* Leads: Supercon 387M-2A3D1, single core NbTi in CuNi clad, 0.127mm
* H1: 378 Ohm through heater, 37 Ohm through leads
* H2: 384 Ohm through heater, 37 Ohm through leads
* H3: 389 Ohm through heater, 36 Ohm through leads
* H4: 385 Ohm through heater, 36 Ohm through leads

#### Heaters-v2 (Nov 2021)
* Wire: Eureca, 40um.
* Coils: 20 turns, D=8mm, ~200 Ohm each.
* Leads (same as before): Supercon 387M-2A3D1, single core NbTi in CuNi clad, 0.127mm, 16.5-17.0 Ohm/wire at room T.

#### Heater on HS Nb shield (01.03.2022)
* 40um constantan wire, 317 R.
* leads: single-core supercond. in CuNi clad, 12.8 R/wire.
* For annealing the shield apply 10V for 10..20s while measuring voltage on HS magnet.

####Mu-metal shield around HS Nb shield (01.03.2022)
* Unknown grade, from storage
* Five plates 25x30x1mm covered with kapton tape.



### Cell for Aerogel experiment (2020), He3 volume

#### Nuclear stage plates
* Material: OFE (CW009A) copper, 1mm plate.
* Plate dimensions: 10x70x1mm with 1mm bevel on one long side.
* Annealing: 900C, 24h, 3.8e-2 mbar of air.
* Silvering: Nushine silvering fluid.
* Powder: Inframat Adv.Mat. 47MN-03, 50nm, 99.95% purity, geometric surface area 10.9m^2/g
* Sinter baking: 15..35 min at 152..162 C in vacuum/nitrogen.
* Weight of copper: ~5.4 g/plate, Weight of silver: ~0.65 g/plate.
* Microscopic surface area: ~3.4 m2/plate.

#### Nuclear stage blocks
* Inner cells: four 8-plate blocks, two in each cell.
  - inner1: 8 plates, m_Cu=42.32g, m_Ag=5.50g, S=28.76m$^2$, V=5.25cm$^3$ cell1
  - inner2: 8 plates, m_Cu=43.05g, m_Ag=5.00g, S=25.84m$^2$, V=5.28cm$^3$ cell2
  - inner3: 8 plates, m_Cu=42.43g, m_Ag=5.25g, S=27.38m$^2$, V=5.24cm$^3$ cell1
  - inner4: 8 plates, m_Cu=42.95g, m_Ag=5.00g, S=27.39m$^2$, V=5.27cm$^3$ cell2
  - cell1: blocks 1+3: m_Cu=84.75g, m_Ag=10.75g, S=56.08m$^2$, V=10.49cm$^3$
  - cell2: blocks 2+4: m_Cu=86.00g, m_Ag=10.00g, S=53.23m$^2$, V=10.55cm$^3$
* Outer cell: four 4-plate blocks + two 2-plate blocks:
  - outer: 20 plates m_Cu approx. 106g, m_Ag approx 13g, S approx 68 m$^2$, V approx 13.1cm$^3$.
* Weights are measured for each plate before and after sintering.
* Microscopic surface areas of each inner cell block measured with BET method.
* Volumes are calculated from material densities (Cu: 8.96 g/cm$^3$, Ag: 10.49 g/cm$^2$).
* Paper spacers: 68x11mm, 7 pcs per block.
* Paper weight: 67.75 g/m$^2$, 0.355 g per block.
* Paper thickness: 80 $\mu$m.
* Paper microscopic surface area: 53 m$^2$ per 1 $m^2$ of paper, 0.278 m$^2$ per block.

#### Aerogel sample:
* Material: Nafen-72, 72 mg/cm$^3$, (material: Al$_2$O$_3$, 4g/cm^3).
* Aerogel density: 98.2% (calculated from material density).
* Dimensions (approx): 50x11x7mm, 3.85 cm$^3$.
* Weight: 0.33g (re-measure before putting to the cell!)
* Micoscopic area: 40.65 m$^2$ (BET measurements)
* Microscopic volume: 0.083 cm$^3$ (based on weight and material density)

#### Inner cells:
* Material: paper with Stycast 1266, 2 layers, 294 g/m$^2$ (same paper as for NS spacers)
* Dimensions: 76x31x12 mm.
* He volume: 17.8 cm$^3$ per cell.

#### Outer cell:
* Material: glass-reinforced nylon (GRP).
* Dimensions: Lin=84 mm, Din=40 mm, Dout=50 mm.
* Similar cell was tested at T=77K, P=35 bar.
* He volume: 36.0 cm^3

#### Filling lines:
* Copper capillary, Goodfellow CU007100 99.9%, temper: as drawn.
* Dimensions: Dout=0.5 mm, Din=0.22 mm, L=1 m each.
* R(room)=0.135 Ohm/m, RRR=7.3.
* Four lines, L=1m each: two between inner cells and outer cell, two from the outer cell (filling line + pressure gauge).
* Pumping time constant at 4K, low pressure: 5.22h, high pressure 0.23h
* Pumping time constant at 300K: low pressure: 5.18h, high pressure: 0.42h
* Filling lines outside the cell were changed in 01.2022 (same capillary)

####Amount of He3:
*2019: 86 l, after condensing 42 l
*2022: 63 l, after condensing 18 l (24l taken to Fridge2)

#### Vibrating wires:
* W0TA: 127um Ta wire, 0.7 Ohm
* W1TA: 127um Ta wire, 0.6 Ohm
* W2TA: 127um Ta wire, 0.6 Ohm
* W0UM: 4.5um NbTi wire, 144.2 Ohm
* W1UM: 4.5um NbTi wire, 134.2 Ohm
* W2UM: 4.5um NbTi wire, 164.7 Ohm
* W1NM: 450nm NbTi wire, approx 5 kOhm
* W2NM: 450nm NbTi wire, 6.4 kOhm  -- broken in Aug 2021

#### Vibrating wire leads:
* Wire: NbTi wire in CuNi clad. Single core 0.062mm, wire 0.102mm, isolation 0.127mm.
* Single twisted pair in fising line. Two pairs from each vibratng wire.

#### Vibrating wires, vaccuum freq and width at 10mK
* w0ta: f = 1737.0936, w = 53.6e-3 + 0.01162*B^2 - 2.9077*B^4
* w1ta: f = 2050.1370, w = 47.9e-3 + 0.01341*B^2 - 1.0158*B^4
* w2ta: f = 2031.4429, w = 32.2e-3 + 0.01242*B^2 - 2.5899*B^4
* w0um: f = 3131.5088, w = 0.4278 + 7.952*B^2
* w1um: f = 3142.5142, w = 0.3248 + 6.563*B^2
* w2um: f = 1741.0714, w = 0.1966 + 4.604*B^2
* w1nm: f = 4333.2925, w = 0.8446 + 77.37*B^2

#### Drive box calibration (Irms/Vpp), measured 2022-05-03
* w0ta:  I2V(100R) = 142.619, I2V(1k) = 39.0522, I2V(10k) = 5.21989 [uArms/Vpp]
* w1ta:  I2V(100R) = 142.215, I2V(1k) = 38.9449, I2V(10k) = 5.21494 [uArms/Vpp]
* w2ta:  I2V(100R) = 144.540, I2V(1k) = 39.0085, I2V(10k) = 5.20364 [uArms/Vpp]
* I2V(100k) approx 0.543 [uArms/Vpp], I2V(1M) approx 54.5 [nArms/Vpp]


### Cell for Aerogel experiment (2022)

#### New shield protection magnet

* Supercon NbTi wire in Cu clad (mu-mu), 54 cores, 7um, isolation 0.102mm.
* L1=L2=6mm, D1=D2=32mm, N1=1500, N2=250  R=1.05k
* Calculated current: -1A.  short wire: top view ccw; + field up

#### Outer cell

* Araldite, machined in the university workshop
* Dimensions: ID=40.6, OD=52, IL=84
* NS blocks: 4, 4, 4+3, 4+3 plates on silver wires + 2 hanging plates.
  24 plates, 128g of copper, 13g of silver, area: 72m^2, NS volume 15.8cm^3
* Measured He volume of assembled cell (inner+outer): 60.9cm^3
* Estimated He volume of outer cell: 25.3cm^3
* A few wooden and Araldite spacers inside to reduce volume
  Volume: 108.75 (outer,geom) - 15.8 (outer NS) - 21.04 (inner NS) - 60.9 (empty) = 11.0 (spacers)

#### Inner cells

* Same dimensions and material as old ones:
* Material: paper with Stycast 1266, 2 layers, 294 g/m$^2$
* Dimensions: 76x31x12 mm.
* He volume: 17.8 cm^3 per cell.
* Filling lines: Copper capillary, Goodfellow CU007100 99.9%, Dout=0.5 mm, Din=0.22 mm, L=0.4 m each
  (taken from some an old cell). Shorter then before!

* Use old NS blocks, re-measure surface area
  - #1: S = 21.40 m^2  (old: 28.76)
  - #2: S = 24.17 m^2  (old: 25.84)
  - #3: S = 24.91 m^2  (old: 27.38)
  - #4: S = 24.16 m^2  (old: 27.39)
  - cell1: blocks 1+3: m_Cu=84.75g, m_Ag=10.75g, S=46.31m$^2$, V=10.49cm$^3$
  - cell2: blocks 2+4: m_Cu=86.00g, m_Ag=10.00g, S=48.33m$^2$, V=10.55cm$^3$
* Silver wires: Alfa Aesar 1.0mm wire Premion, 99.999% (much better then in the old cell).
  Annealing: 400deg/h to 850 deg, 18h

#### Bolometers and vibrating wires

* Bolometer boxes:7x9x5mm with 0.5mm hole in 100um PET wall. Estimated time constant 1.0s
* 13.5um + 4.5um wires in each bolometer
* Hole in bolometer 1 covered with a cup: D=4mm circle of 0.10mm PET with 0.21mm Stycast paper spacers

* + w0ta - tantalum wire in the outer cell

* + w1ta - tantalum wire in the inner cell 1
* + w1bh - bolometer heater in cell 1 (13.5um) -- copper color legs
* + w1bt - bolometer thermometer in cell 2 (4.5um) -- white legs
* + w1a  - 4.5um -- white legs
* + w1b  - 0.315um -- copper legs
* + w1c - 0.390um on pcb
* + w1d - 0.180um on pcb  -- broken!

* + w2ta - tantalum wire in the inner cell 2
* + w2bh - bolometer heater in cell 1 (13.5um)
* + w2bt - bolometer thermometer in cell 2 (4.5um)
* + w2a  - 4.5um -- white legs
* + w2b  - 0.180um -- copper legs
* + w2c  - 0.315um on pcb
* + w2d  - 0.180um on pcb

#### Cell heaters

* Wire: Eureca, 40um.
* Coils: 20 turns, D=8mm, ~200 Ohm each.
* Leads (same as before): Supercon 387M-2A3D1, single core NbTi in CuNi clad, 0.127mm, 16.5-17.0 Ohm/wire at room T.
* 10nF capacitors on each twisted pair in the connector.
* Resistances 1..4: (2xleads/(2xleads+heater)): 30.3/227.4 30.3/210.3 29.6/211.5 29.3/232.6
* Resistances 1..4: 197.1, 180.0, 181.9, 203.3 (TODO: measure with Res.Bridge)

#### Heat leaks
* Leak to cell1 at small field: 1.2nW after 10 days, 0.5nW after 30 days
* 6.5 mW/(T/s)^2  -- measured during magnetization after R22D03. This corresponds to 80pW at 1mA/s
* Leak to cells at full field: 2.2nW, 2.9nW (measured at 6.1mK for 5 hours, after ~40 days of running, after ~10 days of precooling)

### He3 sample

* Purified 2022-10. Purity 99.9506% (re-measured 2023-05-22)

