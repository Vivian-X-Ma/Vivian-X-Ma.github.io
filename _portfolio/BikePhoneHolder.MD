---
title: "Adjustable Phone Holder for Bike"
excerpt: "A phone holder designed in Fusion 360 with top-down modeling that can rotate and be mounted to a bike"
header:
    image: /assets/img/render_main.png
    teaser: /assets/img/thumbnail.jpg
gallery:
    - url: /assets/img/phone_holder.jpg
      image_path: assets/img/phone_holder.jpg
      alt: "phone_holder_gallery_image 1"
    - url: assets/img/phone_back.jpg
      image_path: assets/img/phone_back.jpg
      alt: "phone_holder_gallery_image 2"
    - url: /assets/img/side_view.jpg
      image_path: assets/img/side_view.jpg
      alt: "phone_holder_gallery_image 3"
    - url: assets/img/working.jpg
      image_path: assets/img/working.jpg
      alt: "phone_holder_gallery_image 4"
---

## Introduction

In this project, I created a phone holder that can be mounted on a bike's handlebar and is able to rotate with a detent mecahnism. I created this with top-down modeling, which is a different way of modeling in Fusion 360 as compared to a regular bottom-up assembly. In a bottom-up assembly, you create different Fusion files and then you link each component in an assembly file. In top-down modeling, you directly can create all your components in one file. You anchor one component, and the rest can be built in place. The benefit of this is that you can effectively design components in relation to each other, as you can align them and see their relationship to one another. This also prevents the need to continuously update linked references in a traditional approach. Using as-built joints, you can directly model parts in place, and you can simulate the movement of parts. You can also directly select one component and modify the sketch, or features of that specific part. 

## Design

For my design, I used 3 main top-down components and some off the shelf-parts, including compression springs, extension springs, one ball bearing, and some m5 heat set inserts and bolts. The first component is a clamp that goes around the handlebar that can be tightened with bolts going into heat set inserts. This piece has an opening to fit a gear shape (the second component) that allows for the detent mecahnism. 

![Component 1](/assets/img/component1.png)
![Another picture of component 1](/assets/img/component1_2.png)

To implement the detent mechanism, the first and second components work together. One is held in place, and the other can rotate. The second component has what kind of looks like a gear that is placed next to the ball bearing and spring that fit into the slot in the first component. The ball bearing is locked in place when in one of the gear's notches, and when rotated, the compression spring allows for the ball bearing to pop out of the notch and into the next one, so the phone can be rotated from a vertical to a horizontal orientation. 

![Component 2](/assets/img/component2.png)
![Detent](/assets/img/detent.png)

The second component's gear piece is attached to the actual main phone holding block as well. This consists of two arms on both the left and right side that hold the phone in place, as well as one piece below that keeps the phone from falling out. 

![Another picture of component 2](/assets/img/component2_2.png)

The final top-down component is a piece that attaches to the second component by clearance fit. There is a vertical slot in the second component, and the third piece slides into the slot and serves as the top piece to hold the phone in place in the front. In the back, an m5 bolt serves as a spring attachment piece for one side of an extension spring. The other side is wrapped around a bolt on the second piece. This allows for the holder to adjust for different phone sizes, as the spring can stretch up to hold taller phones and it will snap back on top of the phone to hold it in place. In my design, I felt that it was a bit loose, so in the future, I would probably have a tighter fit or incorporate some way of keeping the 3rd component from wobbling. 

![Component 3](/assets/img/component3.png)

I did not end up having to change any dimensions to account for 3D printing, as the parts fit together, but in doing another iteration, I would definitely make some modifications to the tolerances, such as a bit of a tighter fit for the detent mechanism, and also some adjustments for the bolt holes. The heat inserts fit fine with a 6.4 mm hole for m5, so I would not change that. 

## CAD Model

View the CAD model here: 

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028115fdacca41d302737?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Assembly and Use

Take the clamp part and slide it onto the handlebars. Use 2 m5 bolts to tighten the clamp around the handlebar by screwing it in to the heat set inserts. Place a spring and ball bearing into the small slot on the first side of the first component and align one notch of the gear with the ball. Then, use a long m5 bolt to screw the second component to the first component. Test rotating the second part. Lastly, slide the third component into the vertical slot on the second component and use an m5 bolt with an extension spring wrapped around its threads to screw into the hole on the third component. Wrap the other side around the bolt on the second component. Place your phone in the holder and rotate it to test it. 

Take a look at how it works: 

![Rotating Phone Mechanism](/assets/img/phone_work.gif)


## 3D Printing

I used regular filament printing for this project for each part. This was the fastest way for me to iterate based on the printing resources available. If I were to do this again, I would most likely use powder printing for the detent mechanism, so the rotation could be cleaner. I might use TPU for the clamp part, as it allows for some flexibility, and I might also use that for the phone holding area, so it can also offer some tolerance for different phone sizes. 

## Gallery

{% include gallery caption="These pictures show different views of the piece when it is assembled and holding the phone" %}
