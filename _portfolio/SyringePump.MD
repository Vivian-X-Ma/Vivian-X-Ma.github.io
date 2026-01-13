---
title: "Syringe Pump Project"
excerpt: "The final project for my rapid prototyping class involving 3D printing, digital logic, assembly, and testing!"
header:
    image: /assets/img/stabilizer.png
    teaser: /assets/img/sp_model.png
gallery:
    - url: /assets/img/sp_actual.png
      image_path: assets/img/sp_actual.png
      alt: "syringe_pump_gallery_image 1"
    - url: assets/img/syringe_pump_thumbnail.png
      image_path: assets/img/syringe_pump_thumbnail.png
      alt: "syringe_pump_gallery_image 2"
    - url: /assets/img/electrical_wiring.png
      image_path: assets/img/electrical_wiring.png
      alt: "syringe_pump_gallery_image 3"
---


For this project, the objective was to design a syringe pump that satisfied several key requirements: compatibility with both 10mL and 20mL diameter syringes, capability to pump liquid at a flow rate from 1 uL / min up to 10 mL / min, and ability to correctly indicate syringe pump state with an LED indicator and start/stop the syringe with a button. Satisfaction of these constraints is very important for a syringe pump to function for various applications, such as administering medication or nutrients to patients, which can also save time for medical personnel. 

To reach the goal, my team designed several 3D printed parts (listed below) that could hold the motor, support the end of the pump, push the plunger forward, hold the flange of the syringe, and hold the front hub of the syringe respectively. To support the two syringe sizes, we designed the syringe barrel stabilizers to have a lower slot in which the smaller syringe would be able to slide down into, and a larger slot that would hold a larger syringe on top while also accomodating for different potential syringe lengths. For our digital logic, we programmed the LED indicator to be green when the pump was running, yellow for when it was paused, and red for when there was no liquid remaining in the syringe based on whether the button was pressed and whether a limit switch was activated (the plunger pusher will hit the switch when the liquid is fully dispensed). We calculated the speed required for the motor to run at a flow rate of x mL / min, so users would be able to input their desired flow rate. To complete the design, we connected the electronic components and secured them within a protective box. Feel free to explore the design in our Fusion360 model embedded below. 


### Operation

There are a few steps to take to operate the pump:
1. Modify the following [arduino code](https://github.com/Vivian-X-Ma/Vivian-X-Ma.github.io/blob/main/assets/code/syringe_pump_code.ino):
  - Set the **flowRate** variable to the desired flow rate for the syringe pump in mL/min.
  - Set the **pumpDiam** variable to the diameter of the syringe body. 
2. Prepare the pump and a compatible syringe by filling it with fluid and removing air bubbles. 
3. Place the syringe barrel between the front and back barrel stabilizers, and the flange (wide back end of the barrel) should be held in the back barrel stabilizer in the proper slot (bottom for 10mL syringe and top for 20mL syringe).
4. Upload the code to the arduino and click the start button (shown in gallery below), which activates the motor and the user can view the indicator light to determine the pump's status. The pump will continue pumping unless the button is clicked again, which pauses the motor, or the syringe is empty (switch triggered). 
5. Turn off the pump and disconnect it from the power source. 


## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028111d35c611cb0d02c3?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


## Components

This syringe pump was built with a variety of parts, including 3D designed pieces. 


#### 3D printed parts

| Part | Description |
|------|-------------|
| Front Barrel Stabilizer | Stabilizes the narrow front hub of the syringe |
| Back Barrel Stabilizer | Holds the flange of the syringe in place with a slot, allowing for the plunger to be pushed forward |
| End Support | Support piece for the linear rod |
| Motor Mounting Plate | Holds the motor |
| Plunger Presser | Presses the plunger forward at a steady rate |
| Box Lid | Covers the electronic components |
| Box for Electronic Components | Protective box designed designated, measured sections on the bottom to keep electronic components in place |


#### Off-the-shelf Parts

| Part | Quantity Required |
|------|-------------------|
| F688ZZ Flanged Ball Bearing | 1 |
| Flexible Coupler | 1 |
| Lead Screw TR8×8 (250 mm) | 1 |
| Limit Switch | 1 |
| Linear Rod | 1 |
| Linear Bearing | 1 |
| Lock Collar for Lead Screw | 1 |
| Lock Collar for Linear Rod | 2 |
| M3 × 8 Thread-Forming Screw | 4 |
| M3 × 10 mm Bolt | 1 |
| M5 Tee Nut | 6 |
| M5 × 8 mm Bolt | 6 |
| TR8×8 Lead Screw Nut | 1 |
| NEMA 17 Motor | 1 |
| Syringe | 1 |
| V-Slot 20 × 40 × 350 mm | 1 |
| LED | 1 | 
| Button | 1 |
| Arduino | 1 |


## Gallery

{% include gallery caption="The first picture shows a green light when the pump is turned on, and the third picture shows a model of some of the electrical wiring." %}
