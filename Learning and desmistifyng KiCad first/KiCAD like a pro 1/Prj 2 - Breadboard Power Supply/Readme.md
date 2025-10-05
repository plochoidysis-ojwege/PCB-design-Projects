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
## Schematic
Here is the schematic design, from it ,you can infer the bill of materials:
![Schematic design](https:/photo)

As you can see,I was unable to use the parts and footprints from the digikey library as used in the Peter's book.But still Im working on that, I'll update the next version.For that reason , this repository has two branches ,the main branch just for the projects as I did them, which may include things I couldnt figure out , and then the master branch containing the corrected versions of the projects.

I made sure the Electrical Rules Check was clean:-[ERC](HTTPS )

 ## PCB Layout 
 At this stage,I learnt a lot and used some of the features for the first time.To me , this is the most crucial part of the PCB design.I learnt the following;
 - Using vias for the first time to connect the F.copper and the B.copper routes where routing was not possible due to routes on same copper layer having to cross over each other.
 - Using the "lock" feature helped me to avoid unnecessarily moving a footprints to ensure accuracy and precision.In this case , the distance between J6 and J4 needs to fixed during this whole entire process.I only unlocked after the whole process.
 - How to use copper fills and their importance.I created a 
copper fill in the bottom copper layer and connected it to the GND net.This resulted in a fully routed board. Even though I had fully routed the footprints including the grounds , even if I  didn't route the grounds, using copper fills and connecting it to the GND generally results into a fully routed board.
