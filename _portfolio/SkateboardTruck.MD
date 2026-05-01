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

| Name of Force      | Magnitude | Location of Application | Rational                                                                                                                                               |
| ------------------ | --------- | ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Weight of Rider    | 200 lbs   | Center of the truck     | This is the main force that the truck will experience, as it needs to support the weight of the rider.                                                 |
| Acceleration Force | 50 lbs    | Rear of the truck       | This force represents the acceleration of the skateboard when the motor is engaged. It is applied at the rear of the truck where the motor is located. |
| Turning Force      | 30 lbs    | Front of the truck      | This force represents the lateral forces experienced during turning. It is applied at the front of the truck where the pivot point is located.         |

## CAD Models

### ALSi10Mg Outcome

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028118800554db65b916d?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### 17-4 PH Outcome

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028119a5c0c5d73c8997b?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Gallery

{% include gallery caption="The first pictures show a rendering of the completed assembly with the aluminum truck design, and the next picture shows the assembly with the stainless steel truck design. The other pictures show other rendering angles,the fully assembled skateboard, and the powder printed part." %}

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
