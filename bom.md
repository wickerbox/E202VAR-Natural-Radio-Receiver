####Bill of Materials

#####Notes

**Overall** The whole design is intended to be made of through-hole parts and solderable by a hobbyist without any special equipment. The unit cost listed is at Qty=1, which is never the best deal. You don't have to use Digikey, I'm just using them as an example. Feel free to source equivalent parts. 

**Options** I've provided a couple of options for some of the connectors. When you see an option (A) and (B) for a particular PART, then you'll have to choose which option (A or B) you prefer. You'll buy all listed under PART(A) or under PART(B). Don't buy both. 

**BNC connectors** are 50 ohm impedance and right angle. WM5524-ND is by far the cheapest and saves $3 on total board cost over WM5515-ND. I suggest WM5515-ND as alternate. 

**Capacitors** I preferred class 1 capacitors that are very stable in response to environmental conditions. In circumstances where a 5% C0G part was $0.32 each and a 1% C0G was $1.75, I went with the 5% part.  

**Headphone Jack** I provided a 3-pin headphone 3.5MM jack that's a lot cheaper than the other one I was provided/shown. It's wired as suggested here: http://www.circuitbasics.com/how-to-hack-a-headphone-jack/

**Resistors** If you're going to buy one each of these, why not just buy a kit? I specced standard 1/4W carbon film resistors so I highly, highly do recommend a kit. Try this one: <a href="http://www.digikey.com/product-detail/en/RS125/RS125-ND/">RS125-ND</a>

**Inductors** Changed 3uH to 3.3uH because most of the affordable ones had tolerance of 20%. 20% of 3.3uH is 0.66uH, so I think it's probably fine. Let's just see how it goes. If there's a problem, this is a place to look. 

**10K Pot** This is the volume knob and I had a handful of these blue knobs from Adafruit that fit the switch. I've linked them below.

**BJT** BC237 is obsolete but it was replaced by the BC547B. Same manufacturer (Fairchild) and package (TO-92).

###### Board BOM

|Refdes|Qty|Digikey Part Number|Name|Unit Cost|
|------|---|-------------------|----|---------|
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
|R7|1|10.0XBK-ND|RES 10 OHM 1/4W 1% AXIAL|$0.10|
|R9,R17|2|CF14JT33R0CT-ND|RES 33 OHM 1/4W 5% CARBON FILM|$0.10|
|R13|1|CF14JT1K00CT-ND|RES 1K OHM 1/4W 5% CARBON FILM|$0.10|
|R12|1|CF14JT2K20CT-ND|RES 2.2K OHM 1/4W 5% CARBON FILM|$0.10|
|R4|1|CF14JT3K30CT-ND|RES 3.3K OHM 1/4W 5% CARBON FILM|$0.10|
|R11|1|CF14JT4K70CT-ND|RES 4.7K OHM 1/4W 5% CARBON FILM|$0.10|
|R8|1|CF14JT10K0CT-ND|RES 10K OHM 1/4W 5% CARBON FILM|$0.10|
|R2,R3|2|CF14JT100KCT-ND|RES 100K OHM 1/4W 5% CARBON FILM|$0.10|
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
|LAMP(A)|1|289-1223-ND|LAMP INCAND T1.25 WIRE TERM 14V|
|LAMP(B)|1|RS Components|4 mm Clear Neon Indicator Lamp, Wire Terminal, 100/120/220/250 V 0.25 mA|-|$0.72|
|OP1|1|296-7203-5-ND|IC OPAMP JFET 3MHZ 8DIP|$0.52|
|Q1,Q2|2|BC547BTACT-ND|TRANS NPN 45V 0.1A TO-92|
