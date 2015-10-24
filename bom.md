####Bill of Materials

#####Notes

Overall: the whole design should be through hole soldering by a hobbyist. No fancy soldering equipment required.   

BNC connectors: 50 ohm impedance, right angle. WM5524-ND by far the cheapest. save $3 on total board cost over WM5515-ND. Suggest WM5515-ND as alternate. 

Capacitors: prefer class 1 capacitors that are very stable in response to environmental conditions. In circumstances where a 5% C0G part was $0.32 each and a 1% C0G was $1.75, I went with the 5% part.  

Overall: Cost is at quantity=1, which is rarely the best deal.

Overall: You don't have to use Digikey, I'm just using them as an example. Feel free to source equivalent parts.

###### BOM

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
||1|ON HAND|On/Off switch on hand|
||1|HOLES|Solder holes for 9V battery connector|
||1|MC7809CTGOS-ND|IC REG LDO 9V 1A TO220AB|
||1|296-6548-5-ND|TLE2426 2V 20mA VREG 8DIP|
||2|BC547BTACT-ND|TRANS NPN 45V 0.1A TO-92|
||1|296-7203-5-ND|IC OPAMP JFET 3MHZ 8DIP|
||1|NJM386D-ND|IC AUDIO PWR AMP LOW VOLT 8-DIP|
||1|CP-3502MJ-ND|CONN AUDIO JACK 3.5MM MONO|
||1|ON HAND|20mA RED LED 2V TH|
||1|HOLES|JUMPER SWITCH FOR HIGH PASS FILTER|
||1|289-1223-ND|LAMP INCAND T1.25 WIRE TERM 14V|

BC237B
|1|CP1-3535NG-ND|CONN JACK STEREO R/A 5PIN 3.5MM|

Surface Mount Version

|Qty|Digikey Part Number|Name|
|---|-------------------|----|
|2|1N4001-TPMSCT-ND|1N4001 Diode|
|3|WM5515-ND|CONN BNC JACK R/A 50 OHM PCB TH|
|1|ON HAND|On/Off switch on hand|
|1|HOLES|Solder holes for 9V battery connector|
|1|MC7809CD2TGOS-ND|IC REG LDO 9V 1A D2PAK|
|1|296-1345-1-ND|TLE2426 2V 20mA VREG 8SOIC|
|2|BC847BLT1GOSCT-ND|TRANS NPN 45V 0.1A SOT23|
|1|296-15001-1-ND|IC OPAMP JFET 3MHZ 8SOIC|
|1|LM386MX-1/NOPBCT-ND|IC AMP AUDIO PWR .325W AB 8SOIC|
|1|CP1-3535NG-ND|CONN JACK STEREO R/A 5PIN 3.5MM|
|1|HOLES|JUMPER SWITCH FOR HIGH PASS FILTER|

Neon - transorb?

P1  10k Pot

R13 1K
R5  10M
R1  10M
R1  100k
R4  3.3k
R3  100k
R8  10k
R11 4.7n
R7  10
R9  33
R12 2.2k
R17 33  

L1  3uH

C3  8.2p
C5  150p
C16 4.7n
C7  4.7n
C10 10n
C14 22n
C15 22n
    33nF 
C2  100n
C6  10u
C12 10u
C4  10u
C11 100uF
C9  100u
C13 100u

