# Breadboard Power supply
## Overview
This is the second project I've done.It was inspired by the project in the book "Kicad like a pro" by Peter Dalmaris under a chapter called "Part 9:Project-Design a simple breadboard power supply PCB".This was a project to design a simple breadboard power supply PCB,to provide power to circuits implemented on a mini breadboard, which is a core part of electronics prototyping.The inspiration for the design of the PCB came from creating small eletronics for his(Peter Dalmaris') Arduino and ESP32 courses. When the circuit he was building on the breadboard needed more power than the MCU could provide, he settled on this project.

 For the breadboard power supply,we needed something that:
 1. Plugs directly on the breadboard;therefore, there are no wires.
 2. Have an on/off switch.
 3. Can provide 5V and 3.3V power.
 4. Can draw power from a range of wall power supplies,from 6V to 12V.

 The breadboard connects to the PCB through two sets of pin headers.Two double screw terminals are added to provide additional way to output power via jumper wires instead pins.

 From this project I learnt the following: 
 - How to import and use footprints and parts from external libraries.
 - How to use vias in routing to connect the B.copper to F.copper routes.
 - How to use copper fills and their importance.

 And other things, I already learnt them in other subsequent projects or I'm yet to.
 ## Bill of Materials
 Here is the generated B.O.M
 ![B.O.M](https://github.com/plochoidysis-ojwege/PCB-design-Projects/blob/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Breadboard%20Power%20supply/bom/the%20generated%20B.O.M.png)
 This was not the bill of materials used in KiCad like a pro,I used my own switch instead of the digikey one used in the book.And also assigned a footprint that is compartible as you can see.
## Schematic
Here is the schematic design, from it ,you can infer the bill of materials:
![Schematic design](https://github.com/plochoidysis-ojwege/PCB-design-Projects/blob/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Photos/Schematic.png)

As you can see,I was unable to use the parts and footprints from the digikey library as used in the Peter's book.But still Im working on that, I'll update the next version.For that reason , this repository has two branches ,the main branch just for the projects as I did them, which may include things I couldnt figure out , and then the master branch containing the corrected versions of the projects.

I made sure the Electrical Rules Check was clean:-[ERC](https://github.com/plochoidysis-ojwege/PCB-design-Projects/blob/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Breadboard%20Power%20supply/ERC.rpt)

 ## PCB Layout 
 At this stage,I learnt a lot and used some of the features for the first time.To me , this is the most crucial part of the PCB design.I learnt the following;
 - Using vias for the first time to connect the F.copper and the B.copper routes where routing was not possible due to routes on same copper layer having to cross over each other.
 - Using the "lock" feature helped me to avoid unnecessarily moving a footprints to ensure accuracy and precision.In this case , the distance between J6 and J4 needs to fixed during this whole entire process.I only unlocked after the whole process.
 - How to use copper fills and their importance.I created a 
copper fill in the bottom copper layer and connected it to the GND net.This resulted in a fully routed board. Even though I had fully routed the footprints including the grounds , even if I  didn't route the grounds, using copper fills and connecting it to the GND generally results into a fully routed board.
---
Below is the PCB Layout;
This is how it looked before the copper fills , you can see I used the vias.

![PCB front view](https://github.com/plochoidysis-ojwege/PCB-design-Projects/blob/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Photos/front%20view-b4%20copper%20fill.png)

---
The bottom view ,the vias makes it easier to connect the two routes as you can see.
![PCB bottom view](https://github.com/plochoidysis-ojwege/PCB-design-Projects/blob/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Photos/back%20view-b4%20copper%20fill.png)

---
The copper fill is so important, here I connected it with the GND net, the board was complete as shown;

![PCB after the routing complete](https://github.com/plochoidysis-ojwege/PCB-design-Projects/blob/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Photos/after%20the%20hatch(copper%20fill%20the%20bottom).png)
 And in 3D ;

 ![3D after hatch](https://github.com/plochoidysis-ojwege/PCB-design-Projects/blob/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Photos/back%20view%203D%20%20after%20copper%20fill.png)

 And I made sure the Design Rules check was clean. You can check it here
 [DRC](https://github.com/plochoidysis-ojwege/PCB-design-Projects/blob/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Breadboard%20Power%20supply/DRC.rpt)

 ---
 This project was mainly for learning new things and I did.
 I have included the files for this project in this directory-

[Here](https://github.com/plochoidysis-ojwege/PCB-design-Projects/tree/main/Learning%20and%20desmistifyng%20KiCad%20first/KiCAD%20like%20a%20pro%201/Prj%202%20-%20Breadboard%20Power%20Supply/Breadboard%20Power%20supply)
