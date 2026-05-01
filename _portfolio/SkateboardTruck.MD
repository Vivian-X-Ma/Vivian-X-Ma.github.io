---
title: "Electric Skateboard Truck"
excerpt: "An electric skateboard truck printed with SLS printing and designed in Fusion 360 with generative design"
header:
    image: /assets/img/powder2_thumb.jpg
    teaser: /assets/img/thumbnail_gd.png
gallery:
    - url: /assets/img/alu1.png
      image_path: assets/img/alu1.png
      alt: "skateboard_gallery_image 1"
    - url: assets/img/alu2.png
      image_path: assets/img/alu2.png
      alt: "skateboard_gallery_image 2"
    - url: /assets/img/steel_1.png
      image_path: assets/img/steel_1.png
      alt: "skateboard_gallery_image 3"
    - url: assets/img/steel2.png
      image_path: assets/img/steel2.png
      alt: "skateboard_gallery_image 4"
    - url: assets/img/powder3.jpg
      image_path: assets/img/powder3.jpg
      alt: "skateboard_gallery_image 5"
    - url: assets/img/powder2.jpg
      image_path: assets/img/powder2.jpg
      alt: "skateboard_gallery_image 6"
    - url: assets/img/powder1.jpg
      image_path: assets/img/powder1.jpg
      alt: "skateboard_gallery_image 7"
    - url: assets/img/powder4.jpg
      image_path: assets/img/powder4.jpg
      alt: "skateboard_gallery_image 8"
    - url: assets/img/powder5.jpg
      image_path: assets/img/powder5.jpg
      alt: "skateboard_gallery_image 9"
---

## Project Description

For the final project in my Additive Manufacturing class, I designed and printed an electric skateboard truck in Fusion 360. The truck was designed using generative design and printed using powder bed fusion with SLS printing. This truck can be attached to the board and is connected to the motor with a belt that allows for rotation of the wheels.

<div style="display:flex; gap:10px; flex-wrap:wrap; align-items:flex-start;">
  <img src="/assets/img/assembly1.jpg" alt="Assembly 1" style="width:320px; max-width:48%; height:auto;" />
  <img src="/assets/img/assembly2.jpg" alt="Assembly 2" style="width:320px; max-width:48%; height:auto;" />
</div>

## Design

To design the truck, I used Fusion's generative design feature, which requires different load cases to represent the forces that the truck might experience. Below is the following table of the forces I used in the generative design model:

| Name of Force             | Magnitude | Location of Application                                                                | Rational                                                                                                                                                                                                                                                                                                                                              |
| ------------------------- | --------- | -------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Weight of Rider           | 500 N     | On both axles and the pivot point                                                      | I used a bearing load to represent the weight of the rider on the axles and the full magnitude of the rider weight because the rider may lean to one side, which would place the full weight on that side. It is also present on the pivot point, as the rider's weight is distributed across the board and when centered, the weight will rest there |
| Weight of Motor           | 8.34 N    | On the bottom edge of the circles in the motor mount where the motor would be attached | This force was calculatd based on the motor's weight, and I used a remote force to represent the weight since the motor is hanging off to the side a bit. The weight is going to be pressed down on the contact holes with the motor mount.                                                                                                           |
| Turning Force             | 150 N     | On the center of the axles in opposite directions                                      | The skateboard may experience force going forward on one axle and force going backward on the other axle during turning, and this shear force allows the skateboard to turn when the rider is leaning on one side.This force is usually about 1/3 of the rider weight.                                                                                |
| Bump Impact Force         | 500 N     | On both axles vertically upward                                                        | This force represents the impact when the skateboard goes over a bump, which will go through the wheels to the axles.                                                                                                                                                                                                                                 |
| Curb Impact Force         | 1300 N    | On both axles                                                                          | This force represents the impact when the skateboard is moving forward and hits a curb, so both axles will experience about 2 - 3 times the rider's weight of impact force coming from the front (the curb).                                                                                                                                          |
| Rotation of Motor         | 5 Nm      | On the Motor Mount                                                                     | This force, applied as a moment on the face of the motor mount, represents the torque of the motor rotating as the rider moves forward. The maximum torque for the Flipsky is about 5 Nm                                                                                                                                                              |
| Reverse Rotation of Motor | 5 Nm      | On the Motor Mount                                                                     | This force, applied as a moment on the face of the motor mount, represents the torque of the motor rotating as the rider brakes. The maximum torque for the Flipsky is about 5 Nm. It can also be reverse direction.                                                                                                                                  |

A structural constraint was applied to the kingpin area to represent the fixed support to ensure stable results. Outcomes were generated with the goal of minimizing mass and maintaining a safety factor of 2 (allowing the part to handle 2 times the applied forces). The generative design was allowed to be unrestricted to allow for the most exploration of different designs.

### Proper Load Cases

It is extremely important to apply proper load cases, as these simulate the real forces that your design will experience in real life. The generative design process utilizes these load cases to determine where material is needed in order to handle various forces, such as impace, rotation of the skateboard, etc. If the load cases are not accurate, then the printed part will likely not be able to handle the forces, and it might break. For example, if the part handles much higher forces than what is applied in the load cases, it will probably break. At the same time, if you overcompensate and put much higher forces, then our goal to minimize mass and create a lightweight and less bulky part will be challenging to reach, as the generative design process will add additional unnecessary material to handle the higher forces.

To improve this process, you should first do research on what forces the part may experience. Then, through iterative design, you can print the part, measure the actual forces the part experiences in different situations, and modify your design and load cases. Through this iterative process, you will get much more accurate representation of the forces.

To determine which forces to apply to my model, I included the main forces that the skateboard truck would experience, such as the weight of the rider, turning, motor rotation, motor weight, and impact forces. I just thought about some of the main potential impact forces, such as going over a bump or hitting a curb. To determine the magnitude of the forces, I found the actual weight of the motor, for example, and estimated impact and turning forces based on what is typically experienced from the rider's weight.

## CAD Models

### ALSi10Mg Outcome

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028118800554db65b916d?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### 17-4 PH Outcome

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028119a5c0c5d73c8997b?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### Comparison of ALSi10Mg and 17-4 PH Outcomes

The aluminum outcome is much bulkier, as can be viewed, than the stainless steel outcome. Since aluminum is less strong than stainless steel, it needed more material to reach the safety factor requirement of 2 in order to still handle the various forces that the skateboard might experience. The aluminum outcome also has more mass of 1.397 kg as opposed to the stainless steel version with a mass of 1.091 kg.

## Gallery

{% include gallery caption="The first pictures show a rendering of the completed assembly with the aluminum truck design, and the next picture shows the assembly with the stainless steel truck design. The other pictures show other angles of the powder printed part." %}

## Assembly and Testing

View the following to see the truck installed on the skateboard deck. The first GIF shows the truck turning with enough clearance around the pivot point with a zoomed-in version, and the next GIF shows the motor rotating the wheel through the belt connection. The rotation around the pivot point is for turning when the rider leans to one side, and the motor rotation is important (shown in both directions) for the skateboard to move forward and brake. Both functions correctly work on the actual model, and the part fits on the actual skateboard. In a future iteration, I would probably increase the clearance, as it currently fits tighter than I would like.

<img src="/assets/img/rotate1.gif" alt="Skateboard truck turning GIF" width="640" />
<video width="640" height="360" controls playsinline>

  <source src="/assets/img/rotate2.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<img src="/assets/img/motor.gif" alt="Skateboard truck motor belt GIF" width="640" />

## Discussion

### Real World Application of Generative Design and Powder Bed Fusion

Generative design and powder bed fusion are a great and unique combination that can be used for various applications. The reason why they work so well together is because generative design usually creates very complex geometries that can be hard to manufacture with traditional manufacturing methods. Powder bed fusion allows for very accurate representations of these designs, as it does not require support and can still have internal lattices and organic shapes and be printed. This allows for the full potential of generative design to be reached, as it can create intricate designs that meet the goals we set, such as minimizing mass while still meeting safety requirements. This also means that instead of assembling multiple separate parts, we can print a part as one piece that is lightweight and connects with the rest of our design (like the skateboard truck). This can reduce assembly time and more efficiency.

The combination of generative design and powder bed fusion is highly beneficial in both automotive and aerospace industries. One example of its use in a car component for a Formula student competition shows how useful the approach was for using generative design to have "weight reduction of 40 % per component and three times higher load capacity," according to this [article](https://www.sciencedirect.com/science/article/pii/S1526612522003723). Essentially, for the international racing competitions, there are many car components, such as brake, suspension, chassis, and more that can be developed more efficiently with generative design and still manufactured with powder bed fusion that would have been much more challenging to manufacture with traditional methods like milling.

Another example in aerospace can be seen in this very recent [news](https://www.lockheedmartin.com/en-us/news/features/2026/Accelerating-Operational-Readiness-with-Laser-Powder-Bed-Fusion-Additive-Manufacturing.html?st_source=ai_mode) from Lockheed Martin. Since powder bed fusion allows for layer by layer creation of parts, it can reduce "expensive and time-intensive tooling," which means that small intricate components can reach the market faster. These parts can still meet strict aerospace requirements for safety, performance, heat handling, and weight. The result of this from the news is that "Lockheed Martin’s use of laser powder-bed fusion’s generative design and optimization solutions deliver a 15-20 percent reduction in overall system weight while boosting heat dissipation efficiency by 10-15 percent," which shows how useful the combination of generative design and powder bed fusion can be. In addition to regular aircraft, it is also used for efficient, reliable and scalable production of platforms like the UH-60M BlackHawk, and PrSM.

### Critique of Generative Design

Generative design seems very useful when first introduced, as it can create designs, and we just have to give it load cases and obstacle/preserve geometries. You might initially think that you can use it for any design and it can minimize mass and meet a safety factor rather than us having to do it manually. While it is great at determining what material can be removed and coming up with very intricate geometries that meet the goals we set, it has drawbacks as well.

First of all, when you want a simple design, generative design often creates complex geometries that can be very hard to manufacture. With powder printing, we can get accurate representations of these geometries, but other manufacturing methods may not be able to easily create these designs. Secondly, if load cases are not correctly applied or the initial conditions given are not accurate, then the generative design will not function correctly. This can be dangerous if used without proper testing and it is just directly trusted. Lastly, if you are trying to find what part of the generative design is failing and modify that, it can be hard to tell, especially if the part design is very strange.

Generative design is most useful when you want to create lightweight parts or need very complex geometries, such as in aerospace, automotive industries, and for medical implants. The benefit of using generative design in these areas is that it can create many geometries that humans may not think of while still meeting safety requirements, for example.
