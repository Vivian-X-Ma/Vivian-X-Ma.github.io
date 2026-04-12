---
title: "Microfluidic Device"
excerpt: "A microfluidic device designed to separate particles based on size using pinch flow fractionation (PFF) with a resin-printed mold"
header:
    image: /assets/img/cover_pin_microfluidic.png
    teaser: /assets/img/microfluidic_2.jpg
gallery:
    - url: /assets/img/microfluidic_1.jpg
      image_path: assets/img/microfluidic_1.jpg
      alt: "microfluidic_gallery_image 1"
    - url: assets/img/Plasma-Treating-Image.jpg
      image_path: assets/img/Plasma-Treating-Image.jpg
      alt: "microfluidic_gallery_image 2"
    - url: /assets/img/microfluidic_mold.jpg
      image_path: assets/img/microfluidic_mold.jpg
      alt: "microfluidic_gallery_image 3"
    - url: assets/img/microfluidic_2.jpg
      image_path: assets/img/microfluidic_2.jpg
      alt: "microfluidic_gallery_image 4"
   
---

## Introduction

Pinch Flow Fractination (PFF) is a passive technique used in microfluidics to separate very small particles based on size. For it to work, there are two sections within the microfluidic device, a pinched and broad section. The large width difference between the two sections causes particles to spread and separate by size as they flow from the narrow to the broad section. In the wide section, flow forces act differently based on particles of different size, and in the narrow section, the center of the larger particle will be lower than that of the small particle, as they will be pressed against one side of the wall. When they reach the broad section, smaller particles move outward, and large particles stay inward, allowing for separation.

Some alternative approaches include active and hybrid approaches. According to this [paper](https://www.sciencedirect.com/science/article/pii/S0255270124004252), "Active methods use external fields to separate particles, while passive methods depend on interactions between particles, channel structure, and flow, making them energy-efficient." Some active methods will use magnetic fields to separate magnetic materials and can generally offer good separation efficiency. Hybrid methods combine both methods for improved results. However, the benefit of PFF is that it allows for separation without external forces, so more parameters, such as flow rate, viscosity, and particle size, can be adjusted.

Another traditional method is filtration: using a filter to separate particles. This has some limitations, as it cannot be adjusted for different particle sizes. With PFF, by controlling the flow rate, particles of different sizes can be separated, and separation will be more effective for very small particles, which is one of the main benefits of choosing PFF over other methods.

### What is PFF used for?

One real-world application of PFF is in the biomedical field, where it can be used to separate cells, blood components, and more. This can be helpful for detecting illnesses, by isolating viruses, for instance. One specific example of a biomedical application was the use of PFF for genotyping single nucleotide polymorphisms, showing the usefulness of accurate separation in identifying mutations. You can read more about this in this [paper](https://pubs.rsc.org/en/content/articlelanding/2008/lc/b802268b). Another application is in the environmental field, where it can be used to identify pollutants and find contamination in the water sources.

## Design

Two studied approaches for PFF include a symmetric approach and asymmetric approach. I chose a symmetric approach, which was slightly easier to design, as we only had one attempt. I did consider an asymmetric approach, but I thought it would be more challenging to design and to calculate the flow of the particles. After reading several papers, I also saw the most resources and diagrams on the symmetric flow, so I decided to try that.

To decide where to place the outlet boundaries for our two particle sizes (small: 125-150 um, large: 425-500 um), I used the following equation to calculate where the particles would end up after fanning out in the broad section:

Y_0 = ((w_p - D/2) * (w_b / w_p))

Here are a few images with the dimensions of my design:

![Pinched Section](/assets/img/pff_inlet_dims.png)

![Broad Section and Outlet Channels](/assets/img/pff_outlet_dims.png)

I used a pinched width of 650 um and a broad width of 25 mm. I wanted to ensure that there was enough room for the large particle to go through the pinched section with tolerance. Using the earlier equation, I calculated the y-position for the small and large particles based on the width of my pinched and broad section and the average diameter of both the small and large particles. In the image, you can see the dotted line that indicates where the particles will flow. I used a parameterized variable to set the y-positions, so it would adjust with any change in the broad and pinched dimensions. To ensure that the out channels would be large enough to fit the particles, I also added some tolerance to account for size variation in the particles.

I tried to maximize the difference between the pinched and broad width to increase particle separation. Based on the y-position calculation equation, it can be seen that the larger the difference, the greater the difference in the particles y-positions. To ensure that the tubing could fit on the outlets, I made sure there was enough room between each outlet, which somewhat limited how wide I could make the broad section. To get the outlet channels to reach the positions of the outlet, I created a curve for the smallest particles. If I were to iterate on this design, I would try to use a smoother curve, as currently, I have a pretty sharp angle where the delta for the small particle goes to the outlet channel. This can lead to air bubbles, so I would try to modify that.

The height of the channels was 850 microns. I gave it some additional tolerance, as I thought that it might get a bit compressed during the bonding process, but I kept it under 1 mm to prevent particle stacking that would affect the flow paths.

## CAD Model

Feel free to look through the CAD model here:

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028112f56fab0c4119e8d?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### Testing my Design

During testing, I set the flow rate to be the width of the delta for each outlet section divided by the entire width of the broad section, as that was how much flow to be expected to go to each outlet. This approximately ended up being about 50% for the buffer, 21% for the small particle outlet, and 29% for the large particle outlet.

Here is a video from testing my design. We can see some separation of the particles, but it does not appear to be enough. The purple large particles appear to have a lower flow path than the small orange particles, which are taking the higher path. Slight shaking of the device and tubes would affect the flow rate, which caused some of the orange particles to have a lower flow path.

<video controls width="800">
  <source src="/assets/img/vivian.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

Some hypothetical applications for my microfluidic device could include separating out contaminants, such as microplastics and small sediment particles. It could also be used for sorting for nanoparticles or small beads.

## Instructions and Resin Printing Process

Here is a detailed overview of the steps I took to create my microfluidic device:

- First, I designed my device in Fusion360. I calculated the outlet y-positions and the width of the pinched and broad sections. I adjusted slightly for resistance.
- Then, using a Form 4 resin printer, I printed the mold with clear resin. It was important to keep the bottom of the mold flat, so it needed to be printed parallel to the resin vat. Resin-printing is a good choice for this process over other manufacturing techniques, as it allows for high detail and a relatively smooth finish. Filament printing, on the other hand, would not be able to reach the minimum feature size needed to create the device and often has a rough finish.
- After the print was completed, it needed to be post-processed (IPA washing, drying, and curing). Take care not to cure it for too long, as it will cause warping.
- Prior to curing, the resin molds needed to be coated with parylene because photoinitiators in the resin can prevent full curing of the PDMS, which would lead it to be sticky. This would not be good for the device, so the parylene prevents this inhibiting reaction, allowing for a full cure and easy removal, as it is also very smooth and can increase durability.
- From the mold to the actual device, we used PDMS to cast the device. The heat cure times are included here:
    - 24 hours at 23°C, or 4 hours at 65°C, or 1 hour at 100°C, or 15 minutes at 150°C
- The PDMS was then bonded with glass slides to create the actual flow sections.
- For testing, we had a polyethylene beads of two sizes suspended in a 3% tween solution. The beads kept sinking, so we had to shake them, as they are very sensitive to temperature. The larger beads were more sensitive, so it was hard to get them to flow through the device. This mixture was sent into the device inlets, and we set the outlet flow rates connected to the outlets with syringe pumps.

See the below images of the results of creating the mold and device, as well as the set-up process we had for testing:

## Gallery

{% include gallery caption="The first picture shows the set-up for testing our microfluidic devices. The next picture is an image of the process for the plasma treating process for creating the PDMS mold. The last two images show the resin-printed mold and actual microfluidic device." %}

---

## Future Improvements

In a future iteration, I would most likely try either an asymmetric design or a design with an enhanced separator. One way to create enhanced separation is to separate the broad section as well ([paper](https://pubs.aip.org/aip/apl/article-abstract/93/20/203507/336137/Separation-enhancement-in-pinched-flow?redirectedFrom=fulltext)) As the particles flow upward, the larger particles will still be slightly lower than the smaller particles, and as they both flow into the top part of the broad section, by creating a separator that causes the top of the broad section to become wider, the larger particles will be pulled down more, creating greater separation. Looking at this video clip of one device with the enhanced separation, we can see that with more modifications, this could have more potential success with improved separation between the large and small particles compared to my design. Lastly, I would also try to balance the resistance and be more meticulous with the flow rate calculations for the outlet channels. When testing, it is important not to shake any parts, as that also affects the flow of the particles.

To handle a larger range of particle sizes, I can adjust the pinched width. By increasing the size of the pinched width, it will allow for larger particles to flow through, but this can lead to some particle stacking. By increasing the width of the broad section, there will be more separation of the particles. One other variable to change is the flow rate. If we adjust the flow rate calculations, we can use the same device for a wide range of particle sizes.

The lower limit on the particle size that can be separated with pinch flow fractionation is definitely affected by the minimum feature that we can print, as if we cannot make the channels small enough for microscopic particles, then there will likely be a lot of particle stacking, which will affect the flow path of the particles in the broad section.

<video controls width="800">
  <source src="/assets/img/kathleen.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## Additional References

Here are some additional resources that I looked through when trying to design my device:

- Cui Q, Tian G, Zhou T, Shen Y, Feng S, Li M, Li W, Hosokawa Y, Yalikun Y, Zhang T. Design advances in pinched flow fractionation for enhanced particle separation in microfluidics. Lab Chip. 2025 Aug 19;25(17):4290-4308. doi: 10.1039/d5lc00497g. PMID: 40747581.
    - [link](https://pubmed.ncbi.nlm.nih.gov/40747581/)
- Seyed Nezameddin Ashrafizadeh, Mahdi Zare, Mahdi Khatibi,
  A comprehensive review of pinch flow fractionation in microfluidics: From principles to practical applications,
  Chemical Engineering and Processing - Process Intensification, Volume 208, 2025, 110087, ISSN 0255-2701, https://doi.org/10.1016/j.cep.2024.110087. - [link](https://www.sciencedirect.com/science/article/pii/S0255270124004252)
- [Pinched Flow Fractionation: Continuous Size Separation of Particles Utilizing a Laminar Flow Profile in a Pinched Microchannel](https://arxiv.org/abs/0710.5840)
- [Microfluidic Reviews](https://elveflow.com/microfluidic-reviews/flow-resistance/)
