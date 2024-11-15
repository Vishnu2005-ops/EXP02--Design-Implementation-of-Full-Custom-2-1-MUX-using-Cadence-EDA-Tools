# EXP02--Design-Implementation-of-Full-Custom-2-1-MUX-using-Cadence-EDA-Tools

### Aim:
To design and implement a 2:1 multiplexer (MUX) circuit using Cadence EDA tools, analyse its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.
Tools Required:
•	Personal Computer
•	Cadence Virtuoso Software

### S C H E M A T I C S I M U L A T I O N
### PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence
1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
### Procedure for Schematic simulation using Cadence

1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”<br>
2.	Close the 2nd window<br>
3.	Use 1st window i.e virtuoso window(CIW) for further processing.<br>
i.	Create a New Library<br>
ii.	Create Schematic Cell view.<br>
iii.	Create the Symbol for schematic Cell view.<br>
iv.	Create the test Cell view.<br>
v.	Analog simulation by spectre<br>


### i)	Procedure for Creating New Library.<br>
•	File –New – Library<br>
•	Name : Give name for ur library Ex: VLSILAB_EXP_1<br>
•	Enable Attach to an existing technology library, Click OK<br>
•	Attach the library to the technology library gpdk045.Click OK<br>
### ii)	Create Schematic Cell view.<br>
•	Go to 1st window i.e virtuoso(CIW)<br>
•	File-New-Cell view<br>
•	Setup the new file form<br>
	  Library: Select the one you a created.<br>
	  Cell : Give the experiment name Ex: Inverter View_Schematic<br>
	  Type: Schematic press OK<br>
•	Add the required components from the libraries and make the connections.<br>
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances<br>
	Click on browse. This opens the library browser<br>
	Now select the appropriate library for components like <br>
	Gpdk45 ------------------------nmos1v,  pmos1v<br>
	Create Input and Output pins<br>
	Make the connections by using fixed narrow wire key<br>
	Click Check and Save button<br>
![IMG_20241018_191647](https://github.com/user-attachments/assets/5315d6b0-a69d-43c1-9d0c-0985c6c4977b)


 
### iii)	Creating the Symbol for schematic Cell view
•	In the schematic window, execute<br>
	Create – Cell view – From Cell view<br>
	The cell view from cell view window appears<br>
	Check Lib Name, Cell Name, From View name must be schematic Press ok<br>
•	Now Symbol generation form appears. Click Ok If No changes required<br>
•	A new window with with default symbol is created.<br>
•	Edit the symbol if you want to give actual symbol shape else continue.<br>
•	Execute Create-Cell view-from cell view<br>
•	Library Name and Cell Name must be same which you have used for schematic. Press OK<br>
•	Check for the position of pin side.Prss OK<br>
•	Edit for the shape by Create-Shape-Choose required options to edit.<br>

![IMG_20241018_191627](https://github.com/user-attachments/assets/807b158a-f033-4e12-8477-447ce7d924dd)


### iv)	Creating the new test cell view
•	Go to CIW window, Execute File-New-Cell view<br>
	Setup the new file form<br>
	Library: Select the one you created.<br>
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test<br>
	View: Schematic<br>
	Type: Schematic press OK<br>
•	Follow the step 3(ii) d to make the required connections<br>
![IMG_20241018_191657](https://github.com/user-attachments/assets/6ba2d02e-1a59-4db9-b733-240e4cd756e6)

### Analog simulation by SPECTRE.
•	In test cell view window<br>
•	Launch – ADE L(Analog Design Environment)<br>
	Execute Setup—Simulation/directory/Host A new window opens<br>
	Set the simulation window to spectre and click ok<br>
	Execute Analysis – Choose. A window opens.<br>
	Select the type and set the specifications and press OK<br>
	Execute Output s—to be plotted – Select on Schematic<br>
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse<br>
•	Execute Simulation -- Net list and Run<br>
![image tran analysis](https://github.com/user-attachments/assets/05c563bd-e84a-4173-82e5-355f19df1276)

For Transient Analysis Settings and Output
![Transient analysis](https://github.com/user-attachments/assets/bae51070-8f75-416f-b85a-00da3d7dcf3f)

![output](https://github.com/user-attachments/assets/7fa60fa5-2fe4-49c8-8e43-977b71ee9773)



 

### Results:
1.	The experiment successfully demonstrated the design and implementation of a 2:1 MUX using Cadence EDA tools. 
2.	The successful verification through schematic, layout, and simulation underscores the effectiveness of using Cadence EDA tools for digital circuit design.
