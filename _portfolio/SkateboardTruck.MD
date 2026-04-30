---
title: "Electric Skateboard Truck"
excerpt: "An electric skateboard truck printed with SLS printing and designed in Fusion 360 with generative design"
header:
    image: /assets/img/assembly.png
    teaser: /assets/img/teaser.png
gallery:
    - url: /assets/img/pickle1.png
      image_path: assets/img/pickle1.png
      alt: "pickleball_gallery_image 1"
    - url: assets/img/pickle-face.png
      image_path: assets/img/pickle-face.png
      alt: "pickleball_gallery_image 2"
    - url: /assets/img/tpu_handle.png
      image_path: assets/img/tpu_handle.png
      alt: "pickleball_gallery_image 3"
    - url: assets/img/pickleball.jpg
      image_path: assets/img/pickleball.jpg
      alt: "pickleball_gallery_image 4"
---

## Project Description

For the final project in my Additive Manufacturing class, I designed and printed an electric skateboard truck in Fusion 360. The truck was designed using generative design and printed using powder bed fusion with SLS printing. This truck can be attached to the board and is connected to the motor with a belt that allows for rotation of the wheels.

## Design

To design the truck, I used Fusion's generative design feature, which requires different load cases to represent the forces that the truck might experience. Below is the following table of the forces I used in the generative design model:

| Name of Force      | Magnitude | Location of Application | Rational                                                                                                                                               |
| ------------------ | --------- | ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Weight of Rider    | 200 lbs   | Center of the truck     | This is the main force that the truck will experience, as it needs to support the weight of the rider.                                                 |
| Acceleration Force | 50 lbs    | Rear of the truck       | This force represents the acceleration of the skateboard when the motor is engaged. It is applied at the rear of the truck where the motor is located. |
| Turning Force      | 30 lbs    | Front of the truck      | This force represents the lateral forces experienced during turning. It is applied at the front of the truck where the pivot point is located.         |


## CAD Models

Here is the CAD model of the design for the Aluminum truck:

Here is the CAD model of the design for the Stainless Steel truck:

### ALSi10Mg Outcome


### 17-4 PH Outcome


## Gallery

{% include gallery caption="The first picture shows a rendering of the completed assembly with the aluminum truck design, and the second shows the assembly with the stainless steel truck design. The other pictures show other rendering angles,the fully assembled skateboard, and the powder printed part." %}


## Assembly and Testing

View the following GIFs to see the truck installed on the skateboard deck. The first GIF shows the truck turning with enough clearance around the pivot point, and the second GIF shows the motor rotating the wheels. 

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
