---
title: "MultiMaterial Pliers"
excerpt: "3D printed needle nose pliers capable of picking up through-hole resistors with a flexible component"
header:
    image: /assets/img/plier_header.png
    teaser: /assets/img/plier_iter2.jpg
gallery:
    - url: /assets/img/plier_iter1.jpg
      image_path: assets/img/plier_iter1.jpg
      alt: "plier_gallery_image 1"
    - url: assets/img/tolerance1.jpg
      image_path: assets/img/tolerance1.jpg
      alt: "plier_gallery_image 2"
    - url: /assets/img/plier_iter2.jpg
      image_path: assets/img/plier_iter2.jpg
      alt: "plier_gallery_image 3"
    - url: /assets/img/tolerance2.jpg
      image_path: assets/img/tolerance2.jpg
      alt: "plier_gallery_image 4"
---


## Project Summary

**What it is:**  
To complete this project, I designed and 3D printed a pair of pliers by assembling a flexible component with 4 rigid components, the two handles and 2 jaw parts. The pliers should be able to be directly assembled by hand after printing and pick up a through-hole resistor. Essentially, when the handles are squeezed, the flexible piece will flex, causing the jaws to also squeeze and come together to pick up a part. When released, the flexible piece will revert, returning the pliers to the open position. In this page, I will provide an overview of my design process with my first multi-material 3D printing project.

**Print‑in‑place overview:**  
Print-in-place allows for people to print a full piece without needing assembly, which can be very useful when printing something with multiple components or assemblies for specific purposes. Pieces with a lot of detail that may be difficult to assemble or pieces that need different materials can benefit from using print-in-place. 

Some applications of print-in-place include hinges, decorative models and fidget items, containers, and so much more. Here are a few examples:
- [Collapsible basket](https://www.printables.com/model/22400-collapsible-basket-optimized)
- [Planetary Gearhead](https://forum.bambulab.com/t/multi-material-print-in-place-mechanisms/168352)
- [Fidget Lizard](https://www.thingiverse.com/thing:3505006)
- [Hinges](https://www.crealitycloud.com/blog/tutorials/3d-printed-hinge)

Some of the best materials for print-in place parts include PLA, PETG, ABS, and TPU. PLA is easy to print, and I used it for my own project with TPU. ABS is rigid and requires more time to print, but it also works well, and I used it for one of my iterations of the plier design. PETG is rigid, but has a little bit of flexibility, so it is another good option for print-in-place. TPU is probably the best choice for anything that requires flexibility due to its material properties. Some considerations to keep in mind for multi-material prints include the adhesion between materials and their rate of warping. 

---

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811e4d09a38ca2d68f0?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

---

## Design & Iteration

To determine my design, I based it off of some examples that I saw from previous students in my digital fabrication class with one flexible component in the middle that can spring open and close to make the pliers work. Some considerations I thought about for creating this component was how thick and large I wanted to design this piece. In my very beginning design, I tried to use 3 dovetails for each side of the flexible component to connect it to the rigid parts, as they needed to be assembled by hand. Since they needed to stay in place, the tolerance between the parts had to be tested through several iterations. For the dovetail fit, I ended up giving it a steeper angle, so the parts could lock together better, and I also modified my final design to have two larger dovetails instead of three. This allowed for a deeper fit between the pieces, as opposed to having three shallow dovetails. I kept the thickness of the pliers somewhat thin (8 mm) to allow for increased flexibility and ease of squeezing the handles. I also did not use an extremely heavy infill for the same reason, but I did have the piece be medium sized of 40 mm by 40 mm. 

For the rigid parts, I designed the jaws to have a section at the very front that would come together to pick up the resistors. In my first iteration, I did not take into account the angle at which the jaws would come together, so they only met at one point, but following that, I modified the angle so that the jaws would come together between two sections of the jaws at an almost parallel angle, allowing for better grip. One modification I would make in the future would probably be to make the handles at a wider angle, as they currently come together quite closely when the jaws are also meeting. The final design I currently have is relatively easy to use, but I think the jaw angle can also be slightly adjusted by one or two degrees. 

For the fit between the rigid and flexible components, in my original design, I used a 0.2 mm tolerance, which led to a relatively loose fit between the pieces. It still worked, but the joints were not as strong. I modified the tolerance to a 0.07 mm tolerance in my final design, which had an improved fit due to TPU's flexibility, but if I were to try again, I may lower the tolerance even more, as well as fillet the edges of the dovetail. I find the final design still has a little bit of looseness. By filleting the edges of where the TPU and rigid materials join, it can help account for TPU's inability to print very straight edges and create a better fit. 

My first iteration had rigid pieces printed out of ABS and my second iteration was printed out of PLA, but this did not make any significant difference. In the second iteration, there was a little bit of elephant's foot that caused a slight lip on the print, so the fit was not perfect, but the tolerance was still improved. For both iterations, the flexible piece was printed out of TPU95A. Following iterations would likely result in even better fits. 

---

## Specifications

| Specification | Value     |
| ------------- | --------- |
| Jaw length    | 59.585 mm |
| Jaw capacity  | 20.6 mm   |

---

## Rigid Part PLA Print Settings

| Setting           | Value                     |
| ----------------- | ------------------------- |
| Printer           | Voron Filament 3D printer |
| Nozzle size       | [0.6 mm]                  |
| Infill            | 31% Gyroid Fill           |
| Vertical Shells   | 7                         |
| Horizontal Shells | 0                         |
| Supports          | No                        |
| Print temperature | 210 - 215 °C              |
| Bed temperature   | 65 °C                     |

## Flexible Part TPU95A Print Settings

| Setting           | Value                     |
| ----------------- | ------------------------- |
| Printer           | Voron Filament 3D printer |
| Nozzle size       | [0.6 mm]                  |
| Infill            | 25% Grid Fill             |
| Extrusion Width   | 250%                      |
| Vertical Shells   | 7                         |
| Horizontal Shells | 0                         |
| Supports          | No                        |
| Print temperature | 230 - 235 °C              |
| Bed temperature   | 60 °C                     |

---

## Gallery

{% include gallery caption="The first picture shows the first iteration of the pliers, and next to it the join between the flexible and rigid components. The next two pictures show the same thing for the next iteration (final design)" %}

---

## Demo GIF

Below you can see 2 demos of picking up resistors with the pliers I designed. The first iteration comes together at a single point, so it is able to pick up one resistor.

![1st iteration](/assets/img/1_resistor_iter1.gif)

After modifying the angle that the plier jaws came together at, more resistors can be picked up with the final design.
![final design](/assets/img/3_resistor.gif)
