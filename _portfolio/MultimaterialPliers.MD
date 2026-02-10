---
title: "MultiMaterial Pliers"
excerpt: "3D printed needle nose pliers capable of picking up through-hole resistors with a flexible component"
header:
    image: /assets/img/stabilizer.png
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

o Description of the project with a blurb about print-in-place parts. Perform external
research to determine other applications print-in-place has been used (link specific
examples). What combination of materials work well for print-in-place?
o About the design and iterative process (e.g., how was the spring component
created and how is it retained in the model, materials used)

## Project Summary

**What it is:**  
[1–2 sentence overview of the pliers and their purpose.]

**Print‑in‑place overview:**  
[Brief blurb on print‑in‑place (PIP) parts and why it matters here.]

**External examples of print‑in‑place (PIP):**

- [Example 1 — linked](https://example.com)
- [Example 2 — linked](https://example.com)
- [Example 3 — linked](https://example.com)

**Material pairings for PIP:**  
| Rigid Material | Flexible Material | Why it works | Notes |
|---|---|---|---|
| [e.g., PLA] | [e.g., TPU] | [Reason] | [Clearance/adhesion tips] |
| [ ] | [ ] | [ ] | [ ] |

---

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811e4d09a38ca2d68f0?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

---

## Design & Iteration

### Key design decisions

- **Spring component:** [How it was created and retained in the model.]
- **Print‑in‑place joints:** [Clearances, orientations, and tolerances.]
- **Material choices:** [Why you chose each material.]

### Iteration timeline

| Iteration | Change made | Result | Next step |
| --------- | ----------- | ------ | --------- |
| V1        | [ ]         | [ ]    | [ ]       |
| V2        | [ ]         | [ ]    | [ ]       |
| V3        | [ ]         | [ ]    | [ ]       |

---

## Specifications

| Specification | Value     |
| ------------- | --------- |
| Jaw length    | 59.585 mm |
| Jaw capacity  | 20.6 mm   |

---

## Rigid Part PLA Print Settings

| Setting | Value

|---|---|
| Printer | Voron Filament 3D printer |
| Nozzle size | [0.6 mm] |
| Infill | 31% Gyroid Fill |
| Vertical Shells | 7 |
| Horizontal Shells | 0 |
| Supports | No |
| Print temperature | 210 - 215 °C |
| Bed temperature | 65°C |

## Flexible Part TPU95A Print Settings

| Setting | Value

|---|---|
| Printer | Voron Filament 3D printer |
| Nozzle size | [0.6 mm] |
| Infill | 25% Grid Fill |
| Extrusion Width | 250% |
| Vertical Shells | 7 |
| Horizontal Shells | 0 |
| Supports | No |
| Print temperature | 230 - 235 °C |
| Bed temperature | 60°C |

---

## Gallery

![1st pliers](assets/img/plier_iter1.png)
![1st tolerance fit](/assets/img/tolerance1.jpg)
![2nd pliers](assets/img/plier_iter2.png)
![2nd tolerance fit](/assets/img/tolerance2.jpg)
{% include gallery caption="The first picture shows the first iteration of the pliers, and next to it the join between the flexible and rigid components. The next two pictures show the same thing for the next iteration (final design)" %}

---

## Demo GIF

Below you can see 2 demos of picking up resistors with the pliers I designed. The first iteration comes together at a single point, so it is able to pick up one resistor, and after modifying the angle that the plier jaws came together at, more resistors can be picked up with the final design.

![1st iteration](/assets/img/1_resistor_iter1.gif)
![final design](/assets/img/3_resistor.gif)
