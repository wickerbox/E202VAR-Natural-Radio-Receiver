# E202VAR Natural Radio Receiver 
####Based on the Explorer E202

Renato Romero put plans online for a Very Low Frequency (VLF) receiver capable between "a few Hz to beyond 10 kHz [which] makes it suitable to to receive radio signals of natural origin; signals not generated by human activity but by physical phenomena such as lightning and solar storms. Received signals are heard directly in your headset. The receiver amplifies the electric component of an electromagnetic signal."

His plans are <a href="http://www.vlf.it/romero2/explorer-e202.html">described here</a>. The Explorer E202 is no longer available for sale.

He gave me permission to work from his schematic to design a new layout and make my own units. I am releasing all of my documents and process under the CERN Open Hardware License v1.2.

<a href="http://www.vlf.it/romero2/E202_V1.1.png">Here's the original E202 full-size schematic</a>.

<a href="https://raw.githubusercontent.com/wicker/e202-in-eagle/master/natural-radio-vlf-receiver-v1.png">Here's the E202VAR full-sized schematic</a>

#### Current Project Status

- [x] Get permission and verify that the CERN license is OK.
- [x] Initially verify all the components and build the BOM.
- [x] Create the schematic. 
- [X] Double check the BOM against schematic and available parts.
- [X] Create an Eagle library with all symbols + footprints.
- [X] Release the BOM and library.
- [ ] Figure out what to do about the mechanical assembly + case.
- [ ] Create the board layout to fit the proposed case.
- [ ] Order parts.
- [ ] Order boards.
- [ ] Assemble the boards.
- [ ] Test!

#### Bill of Materials 

Total cost of parts is about $25.

|BNC1-3|3|WM5524-ND|CONN BNC JACK R/A 50 OHM PCB TH|$1.48|
|C3|1|399-8923-ND|CAP CER 8.2PF 50V NP0 RADIAL|$0.51|
|C5,C8,C15|3|BC1015CT-ND|CAP CER 150PF 50V NP0 RADIAL|$0.25|
|C7,C16|2|445-8585-ND|CAP CER 4700PF 50V C0G RADIAL|$0.32|
|C10|1|445-8384-ND|CAP CER 10000PF 50V C0G RADIAL|$0.36|
|C1|1|445-8490-ND|CAP CER 0.033UF 50V C0G RADIAL|$0.48|
|C2|1|445-8532-ND|CAP CER 0.1UF 50V C0G RADIAL|$0.79|
|C4,C6,C12|3|445-8351-ND|CAP CER 10UF 25V X7R RADIAL|$0.63|
|C9,C11,C13|3|445-8441-ND|CAP CER 100UF 6.3V X5R RADIAL|$0.95|
|D1,D2|2|1N4001-TPMSCT-ND|DIODE GEN PURP 50V 1A DO41|$0.10|
|R(KIT)|1|RS125-ND|Resistor Kit|$14.95|
|R7|1|CF14JT10R0CT-ND|RES 10 OHM 1/4W 5% CARBON FILM|$0.10|
|R9,R17|2|CF14JT33R0CT-ND|RES 33 OHM 1/4W 5% CARBON FILM|$0.10|
|R13|1|CF14JT1K00CT-ND|RES 1K OHM 1/4W 5% CARBON FILM|$0.10|
|R12|1|CF14JT2K20CT-ND|RES 2.2K OHM 1/4W 5% CARBON FILM|$0.10|
|R4|1|CF14JT3K30CT-ND|RES 3.3K OHM 1/4W 5% CARBON FILM|$0.10|
|R11|1|CF14JT4K70CT-ND|RES 4.7K OHM 1/4W 5% CARBON FILM|$0.10|
|R8|1|CF14JT10K0CT-ND|RES 10K OHM 1/4W 5% CARBON FILM|$0.10|
|R2,R3,R6(DNP)|2(1)|CF14JT100KCT-ND|RES 100K OHM 1/4W 5% CARBON FILM|$0.10|
|R1,R5|2|CF14JT1M00CT-ND|RES 1M OHM 1/4W 5% CARBON FILM|$0.10|
|J1(A)|0|HOLES|Solder holes for 9V battery connector|$0|
|J1(A)|1|1528-1117-ND|BATTERY CLIP 9V 5.5MM/2.1MM PLUG|$3.00|
|J1(A)|1|None|Standard 9V Battery|Varies|
|J1(B)|1|CP-202BH-ND|CONN PWR JACK 2.5X5.5MM HIGH CUR|$1.16|
|J1(B)|1|1528-1117-ND|BATTERY CLIP 9V 5.5MM/2.1MM PLUG|$3.00|
|J1(B)|1|None|Standard 9V Battery|Varies|
|J1(C)|1|CP-202BH-ND|CONN PWR JACK 2.5X5.5MM HIGH CUR|$1.16|
|J1(C)|1|1528-1116-ND|BATT HOLDER 9V SWITCH 5.5MM PLUG|$3.95|
|J1(C)|1|None|Standard 9V Battery|Varies|
|J2(A)|0|None|0.1" pitch holes to accommodate soldering 24AWG wires|-|
|J2(B)|1|RA11131100-ND|SWITCH ROCKER SPST 10A 125V|$0.52|
|J2(B),P10(B)|1|Varies|24AWG Wire|Varies|
|J3|1|CP1-3523N-ND|CONN JACK STEREO R/A 3PIN 3.5MM|$0.97|
|U1|1|MC7809CTGOS-ND|IC REG LDO 9V 1A TO220AB|$0.45|
|U2|1|296-6548-5-ND|IC VREF GND REF ADJ 8DIP|$1.93|
|U3|1|NJM386D-ND|IC AUDIO PWR AMP LOW VOLT 8-DIP|$0.91|
|D3|1|C503B-BCS-CV0Z0461-ND|LED BLUE CLEAR 3.2V 5MM ROUND T/H|$0.21|
|JUMP1|1|3M9580-ND|SHUNT JUMPER .1" BLACK GOLD|$0.10|
|L1|1|78F3R3J-RC-ND|FIXED IND 3.3UH 575MA 300 MOHM|$0.22|
|P10(A)|0|None|0.1" pitch holes to accommodate soldering 24AWG wires|-|
|P10(B)|1|987-1301-ND|POT 10K OHM 1/5W PLASTIC LINEAR|$0.84|
|P10(B)|1|Adafruit 2048|Potentiometer Knob - Soft Touch T18 - Blue|$.50|
|LAMP(A)|1|A9A-ND|LED NEON WIRE TERMINAL|$0.63|
|LAMP(B)|1|RS Components|4 mm Clear Neon Indicator Lamp, Wire Terminal, 100/120/220/250 V 0.25 mA|-|$0.72|
|U4|1|296-7203-5-ND|IC OPAMP JFET 3MHZ TL081C 8DIP|$0.52|
|Q1,Q2|2|BC547BTACT-ND|TRANS NPN 45V 0.1A TO-92|$0.20|

