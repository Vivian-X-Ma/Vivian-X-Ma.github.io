---
title: "Pickleball Paddle"
excerpt: "A 3D-printed pickleball paddle that survived a real game of pickleball"
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

For this project, I designed and 3D printed the parts of a pickleball paddle. I followed the standard pickleball [guidelines ](https://usapickleball.org/docs/rules/USAP-Official-Rulebook.pdf) for my design, ensuring that:
- The paddle's combined length and width does not exceed 24 inches, and the length is less than 17 inches.
- The paddle's hitting surface is as smooth and flat as possible (with 3D printing).
- The paddle is made of rigid material.


### 3D Printing

Since our 3d printer is limited by size with a 300 x 300 mm build plate, I printed the paddle in separate components. The first component was the face of the paddle, and I added two holes in the bottom for 2 M5 heat inserts for attachment to the handle. The second part, a handle, was built with a hollow bottom and holes in the middle for M5 bolts to attach to the heat inserts. The idea for the bottom of the handle was a TPU grip that would slide onto the handle, providing it with a stronger grip component that would also cap the hollow bottom of the handle. This TPU grip could be interchangeable if printed multiple times. 

I printed the rigid parts out of PLA, and the TPU grip out of TPU95A. I printed with a lower infill to decrease the weight of the paddle to provide more agility and control for the player. I did make the paddle somewhat thicker to provide more support, and I had the handle hold the paddle in place on both sides to provide reinforcement. 


## CAD Model

View the CAD model here:

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811cd14a63fe024f44c?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Assembly 

Place 2 M5 bolts through the holes in the handle through the bottom, so they stick out through the holes in the top of the handle. Screw them into the heat inserts in the bottom of the paddle face. Slide the TPU grip onto the handle.

## Gallery

{% include gallery caption="The first 3 pictures show each component of the pickleball paddle that I designed in Fusion 360, and the last image shows the assembled paddle after playing one game. Unfortunately, I forgot to get a picture of it assembled before the game, and it was slightly damaged due to low infill afterwards." %}

## Testing 

To test the paddle, I played a real game of pickleball on the courts with my class. After the game, the paddle was still working and it survived, although the handle had some damage, and high impact from the ball hitting it led to some cracking of the support pieces on the handle. This is likely due to PLA being a weaker material and the ball hiting in the direction of the layer lines that caused it to easily crack. 

## Future Improvements

In the future, if I were to create another iteration of this design, I would probably print with a more durable plastic, such as PETG and use a higher infill to increase rigidity. I might change the infill pattern to a honeycomb pattern, as I see that is typical for most pickleball paddles. I would also modify the handle grip to have ridges for better grip and add an edge guard for the face of the paddle to protect it from hitting the ground. 
