EXP-6

DATE:

                      SCHEMATIC ENTRY AND CIRCUIT SIMULATION OF A CMOS INVERTER
                          TWO INPUT NAND GATE  AND TWO INPUT NOR GATE

**AIM:**
To create,simulate the design of CMOS inverter,NAND,NOR from schematic using cadence.

**APPARATUS REQUIRED:**

cadence

PROCEDURE:
## Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
          i)	tcsh
          ii)	source /home/install/cshrc
          iii)	virtuoso 
## Procedure for Schematic simulation using Cadence
1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
          i)	Create a New Library
          ii)	Create Schematic Cell view.
          iii)	Create the Symbol for schematic Cell view.
          iv)	Create the test Cell view.
          v)	Analog simulation by spectre
## Procedure for Creating New Library.
a)	File –New – Library
b)	Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing technology library, Click OK
c)	Attach the library to the technology library gpdk045.Click OK
## Create Schematic Cell view.
a)	Go to 1st window i.e virtuoso(CIW)
b)	File-New-Cell view
c)	Setup the new file form, Library: Select the one you a created. Cell : Give the experiment name Ex: Inverter View: Schematic
d)	Type: Schematic press OK
e)	Add the required components from the libraries and make the connections.
f)	Go to instance fixed menu or use shortcut key “I” from keypad to go instances Click on browse. This opens the library browser ow select the appropriate library for components like Gpdk045,nmos, pmos
g)	Analog library	Vdd, Gnd, Vcc, Vpulse, Vsin
h)	Make the connections by using fixed narrow wire key
i)	Click Check and Save button


## Creating the Symbol for schematic Cell view
a.	In the schematic window, execute
          Crate – Cell view – From Cell view
          The cell view from cell view window appears
          Check Lib Name, Cell Name, From View name must be schematic Press ok
b.	Now Symbol generation form appears. Click Ok If No changes required
c.	A new window with with default symbol is created.
d.	Edit the symbol if you want to give actual symbol shape else continue.
          i.	Execute Create-Cell view-from cell view
          ii.	Library Name and Cell Name must be same which you have used for schematic. Press OK
          iii.	Check for the position of pin side.Prss OK
          iv.	Edit for the shape by Create-Shape-Choose required options to edit.
## Creating the new test cell view

a)	Go to CIW window, Execute File-New-Cell view
b)	Setup the new file form
Library: Select the one you a created.
          Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
          View: Schematic
          Type: Schematic  press OK
## Analog simulation by SPECTRE.
a.	In test cell view window
i.	Launch – ADE L(Analog Design Environment)
b.	Execute Setup—Simulation/directory/Host A new window opens
c.	Set the simulation window to spectre and click ok
d.	Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and section type as stat then press OK.
e.	Execute Analysis – Choose. A window opens.
f.	Select the type and set the specifications and press OK
g.	Execute Output s—to be plotted – Select on Schematic
h.	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
i.	Execute Simulation -- Net list and Run

**INVERTER SCHEMATIC:**

![2021-inverter-design-in-cadence](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/799e47d7-0302-4ea2-9ac3-aabaf81cd7e6)

![image](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/da0e4d07-c05f-421b-b5f3-bc061983226e)

**Specifications:**
Vpulse 

    V1 = 0	       
   
    V2 = 1
    
    td = 0,tr=tf=1 n, ton= 100n ,T=200n
    
    Vdc = 1

Simulation Settings

Setup for transient analysis:

   Stop time =400n

Setup for D.C analysis

Component to be selected in schematic is for d.c analysis

    Start = -1 Stop = 1 resp.

Expected Waveform:

**Transient Analysis:**

![output cad](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/eb121860-25a3-4dd3-82d3-be7852279d3d)

**DC Analysis:**
![out](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/1247eda1-1aa4-4a66-a502-1e3ddcc98ec3)

**NAND SCHEMATIC :**

![image](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/bc8d71ff-d898-4fd6-aa39-5fac4be18417)

![image](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/dcae4c10-4436-43df-8be5-aaf72a756c93)


**Specifications:**

Vpulse 

Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse width = 10ns

Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse width = 20ns

Vdc = 1

Expected Waveform:

**Transient Analysis:**

![nand](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/f6e4e117-f164-46f3-8102-2fc13e7582d1)

**NOR SCHEMATIC:**

![image](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/e3de188c-07e2-45c7-8365-a735b98ab1b3)

![image](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/a1ab54fb-65a2-4650-834b-660332d549f1)

**Specifications:**

Vpulse 

Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse width = 10ns

Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse width = 20ns

Vdc = 1

Expected Waveform:

**Transient Analysis:**

![nor](https://github.com/nithin2134/VLSI-LAB-EXP-6/assets/160302970/6aceaa60-8283-4cdc-a250-642f737d597e)


**RESULT:**

Thus, the design,simulation and verification of the CMOS inverter,NAND,NOR from schematic using cadence was successfully completed.
