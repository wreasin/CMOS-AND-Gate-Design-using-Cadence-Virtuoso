# CMOS-AND-Gate-Design-using-Cadence-Virtuoso
### 2-input CMOS AND Gate Design and Analysis with Layout using Cadence Virtuoso

---
<!-- Cadence Project (Transient, DC, AC & Noise Response With Layout) -->

I’m really glad to share that, this is my fourth project on __Cadence Virtuoso__. I am designing here a 2-input CMOS AND Gate Design by a NAND & an Inverter, with it's Layout using Cadence Virtuoso.

___Before I start explaining my project in details, you should know a few things !___     

### What is CMOS AND Gate?  
The AND gate is a basic digital logic gate that implements logical conjunction (∧) from mathematical logic – AND gate behaves according to the truth table above. A HIGH output (1) results only if all the inputs to the AND gate are HIGH (1). If not all inputs to the AND gate are HIGH, LOW output results. The function can be extended to any number of inputs.

### The Project details of mine :
Here i have use __gpdk90n__ :-
1. Three pmos1v and Three nmos1v.
2. For vdd i have use vdc (1v)
3. For input i have use two vpulse (1v)
4. Here I am doing four types of Analysis :  
    i ) Transient Response  
    ii ) DC Response  
    iii ) AC Response  
    iv ) Noise Response & Noise Figure  
    N.B. I'm measuring here 2 inputs & output as Voltage and Current (I) in Vout & VDD node.
5. In Layout - Metals Used ( Metal1 ) and Poly Layer
6. The minimum width of metal utilized for routing is 0.12
7. DRC and LVS clean (there are no error)

So I designed a Schematic of the CMOS AND Gate, where the whole thing is based on gpdk90n. I have use 3 pmos for 1v and 3 nmos for 1v. I also designed a symbol of it, so that i can utilise that for further schematic creation.  

The below figure shows a 2-input CMOS AND Gate. For Designing a AND Gate i have use to a NAND Gate and an Inverter. For Inverter Input i have use NAND's Output.

Considering all steps will show that Vout is following the expected value as in 2-input AND Gate Truth Table.

![Scametic](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/Scametic.PNG?raw=true) 
![Symbol](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/Symbol.PNG?raw=true)
![Symbol_Scametic](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/Symbol_scametic.PNG?raw=true)

#### DC, AC, Transient :
_Here I am doing four types of Analysis - DC, AC, Transient and Noise_.  
In DC and Transient Analysis i have measured Va, Vb & Vout as Voltage, and Current (I) in Vout & VDD node. In AC Analysis i have measured Va, Vb & Vout as Voltage Frequency and Current (I) Frequency in Vout & VDD node. For DC and Transient Analysis the plots of _Va_ , _Vb_ and _Vout_ shows the _voltages_, on the otherhand _VDD(I4)_ & _Vout(I4)_ shows the _current (I)_. For AC Analysis the plots of _Va_ , _Vb_ and _Vout_ shows the _voltage frequency_, on the otherhand _VDD(I4)_ & _Vout(I4)_ shows the _current (I) frequency_. 
![output](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/Output.PNG?raw=true)  
![output2](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/Output_2.PNG?raw=true)  
 

#### Noise Figure and Noise Response :  
For measuring of Noise Figure and Noise Response i had to use PORTS instead of Vpulse. For Noise Analysis i have measured input & output noise. In Noise Response the plots shows the input and output noise.  
![noise_figure_scametic](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/noise%20analysis_scametic.PNG?raw=true)
![noise_figure](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/Noise%20Figure.PNG?raw=true)
![noise_output](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/Noise%20Analysis(IN,OUT).PNG?raw=true)

#### Layout :
In Layout i have use  Metal1 and Poly Layer. I have use here X & Y snap spacing is 0.01m and also the minimum width of metal utilized for routing is 0.12.  
![Layout](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/Layout.PNG?raw=true)  

#### Design Rule Check (DRC)  
DRC is clean. There are no error in DRC.
![DRC](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/DRC%20Check.PNG?raw=true)  

#### Layout Versus Schematic (LVS)  
LVS is clean. There are no error in LVS.  
![LVS](https://github.com/wreasin/CMOS-AND-Gate-Design-using-Cadence-Virtuoso/blob/main/images/LVS%20Check.jpg?raw=true)
