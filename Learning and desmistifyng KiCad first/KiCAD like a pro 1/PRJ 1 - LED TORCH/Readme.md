# LED Torch Project
This is my first project using KiCad. The goal is to design a simple LED torch circuit and overally to learn the basics of KiCad, including schematic capture and PCB layout.
## Components
- 1 x LED
- 1 x Resistor (220 Ohm)
- 1 x 9V Battery
- 1 x Battery Clip
- 1 x Switch
## Schematic
Below is a simple schematic representation of the LED torch circuit:

![Schematic.png](Schematic.png)

From this schematic, I learnt the following features of KiCad:
- How to set up a new project and configure the environment(including grid settings)
- How to place components on the schematic
- How to wire components together
- How to annotate the schematic
- How to run electrical rules checks (ERC)

The problem and I still haven't figured out is whether the warning about the unplaced unit is something I need to address before moving on to the PCB layout.Is it that big deal. In this case , the sinlge pole switch had unplaced unit B as shown below :

but , it's the beginning and I have time to figure it out.

## PCB Layout
Below is the PCB layout for the LED torch circuit:

![PCB_layout.png](PCB_layout.png)

From this layout, I learnt the following features of KiCad:
- How to import the schematic into the PCB layout
- How to place components on the PCB
- How to route traces between components
- How to define board edges and cutouts
- How to generate Gerber files for manufacturing
The thing I found challenging was the routing process, especially ensuring that all traces were properly connected and that there were no unintentional shorts. Again here I realised their is a minimum distance between traces that I need to adhere to.

The PCB layout process was quite intuitive, and I appreciate the visual feedback KiCad provides while routing traces. I still need to learn more about design rules and how to ensure my layout is manufacturable, but I'm excited to continue this journey.
Below is a 3D view of the PCB layout:
![3D_view.png](3D_view.png)
THE END