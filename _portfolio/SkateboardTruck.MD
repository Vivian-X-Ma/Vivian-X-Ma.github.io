---
title: "Electric Skateboard Truck"
excerpt: "An electric skateboard truck printed with SLS printing and designed in Fusion 360 with generative design"
header:
    image: /assets/img/assembly.png
    teaser: /assets/img/steel_1.png
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
    - url: assets/img/powder1.jpg
      image_path: assets/img/powder1.jpg
      alt: "skateboard_gallery_image 5"
    - url: assets/img/powder2.jpg
      image_path: assets/img/powder2.jpg
      alt: "skateboard_gallery_image 6"
    - url: assets/img/powder3.jpg
      image_path: assets/img/powder3.jpg
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

<img src="/assets/img/assembly1.jpg" alt="Assembly 1" width="640" />
<img src="/assets/img/assembly2.jpg" alt="Assembly 2" width="640" />

## Design

To design the truck, I used Fusion's generative design feature, which requires different load cases to represent the forces that the truck might experience. Below is the following table of the forces I used in the generative design model:

| Name of Force             | Magnitude | Location of Application                                                                | Rational                                                                                                                                                                                                                                                               |
| ------------------------- | --------- | -------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Weight of Rider           | 500 N     | On both axles and the pivot point                                                                          | I used a bearing load to represent the weight of the rider on the axles and the full magnitude of the rider weight because the rider may lean to one side, which would place the full weight on that side. It is also present on the pivot point, as the rider's weight is distributed across the board and when centered, the weight will rest there                                                                                |
| Weight of Motor           | 8.34 N    | On the bottom edge of the circles in the motor mount where the motor would be attached | This force was calculatd based on the motor's weight, and I used a remote force to represent the weight since the motor is hanging off to the side a bit. The weight is going to be pressed down on the contact holes with the motor mount.                            |
| Turning Force             | 150 N     | On the center of the axles in opposite directions                                      | The skateboard may experience force going forward on one axle and force going backward on the other axle during turning, and this shear force allows the skateboard to turn when the rider is leaning on one side.This force is usually about 1/3 of the rider weight. |
| Bump Impact Force         | 500 N     | On both axles vertically upward                                                        | This force represents the impact when the skateboard goes over a bump, which will go through the wheels to the axles.                                                                                                                                                  |
| Curb Impact Force         | 1300 N    | On both axles                                                                          | This force represents the impact when the skateboard is moving forward and hits a curb, so both axles will experience about 2 - 3 times the rider's weight of impact force coming from the front (the curb).                                                           |
| Rotation of Motor         | 5 Nm      | On the Motor Mount                                                                     | This force, applied as a moment on the face of the motor mount, represents the torque of the motor rotating as the rider moves forward. The maximum torque for the Flipsky is about 5 Nm                                                                               |
| Reverse Rotation of Motor | 5 Nm      | On the Motor Mount                                                                     | This force, applied as a moment on the face of the motor mount, represents the torque of the motor rotating as the rider brakes. The maximum torque for the Flipsky is about 5 Nm. It can also be reverse direction.                                                   |

## CAD Models

### ALSi10Mg Outcome

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028118800554db65b916d?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### 17-4 PH Outcome

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028119a5c0c5d73c8997b?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Gallery

{% include gallery caption="The first pictures show a rendering of the completed assembly with the aluminum truck design, and the next picture shows the assembly with the stainless steel truck design. The other pictures show other rendering angles of the powder printed part." %}

## Assembly and Testing

View the following to see the truck installed on the skateboard deck. The first GIF shows the truck turning with enough clearance around the pivot point with a zoomed-in version, and the next GIF shows the motor rotating the wheel through the belt connection.

<img src="/assets/img/rotate1.gif" alt="Skateboard truck turning GIF" width="640" />
<video width="640" height="360" controls playsinline>

  <source src="/assets/img/rotate2.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<img src="/assets/img/motor.gif" alt="Skateboard truck motor belt GIF" width="640" />

## Discussion

### Real World Application of Generative Design and Powder Bed Fusion

### Proper Load Cases

### Drawbacks of Generative Design

• A discussion (750 words) on:
o The unique pairing of powder bed fusion and generative design and their
applications in either aerospace or automotive industries. Please research a
specific commercial example (not on the slides), where generative design has
been used to reduce the number of components in an assembly. Citation should
be included as a hyperlink.
o The importance of applying the proper load cases and how to improve this
process. How did you determine which forces to apply to the model?
o A comparison between the ALSi10Mg and 17-4 PH outcomes.
o Critique generative design. How useful is it really? What are the drawbacks?
What applications would generative design be most useful in?

The GitHub writeup includes the following:

Thoughtful reflection on the unique pairing of powder bed fusion and generative design and their applications in either aerospace or automotive industries.
An honest assessment of the utility and drawbacks of generative design.
The GitHub writeup should be at least 750 words in length.
