# Laser Cutting Lab: Parametric Construction Kit

## Objective

The objective of this lab is to design, manufacture, and assemble a parametric construction kit using laser cutting. The project focuses on measuring material thickness, accounting for laser kerf, and testing clearances to create reliable connections.

## Team Members

- Kaileigh Hill
- Austin Williams
- Sebastian Kohler

## Design

### Design Concept

Our team explored different design concepts for a laser-cut construction kit before deciding to design and manufacture a three-dimensional flower using laser-cut plywood. Our goal was to create something functional and visually appealing that demonstrated how flat, two-dimensional pieces could be assembled into a three-dimensional structure using interlocking connections without glue or tape.

The flower consists of 16 total pieces and 8 unique part types:

- 2 different circular base pieces
- 2 different stem pieces
- 2 identical leaves
- 1 petal base hub
- 1 petal hub cap
- 8 identical petals

The design uses press-fit connections to assemble the flower without glue, tape, or additional fasteners. The individual components were designed in SolidWorks and arranged for laser cutting.

Our main design considerations were material thickness, laser kerf, connection clearances, and ensuring that the assembled flower would remain stable. The goal was to create a functional assembly while demonstrating the importance of accurate measurements and parametric design.

### Material Thickness

Before beginning the design, our team measured the material thickness using digital calipers at three different locations.

| Measurement | Thickness (mm) |
|---|---|
| Location 1 | 2.69 |
| Location 2 | 2.68 |
| Location 3 | 2.70 |
| **Average Thickness** | **2.690** |

The average material thickness was 2.690 mm. This value was used as a reference when designing the connections.

#### Material Thickness Measurement

We used calipers to measure the thickness of the plywood before laser cutting.

<img src="https://github.com/user-attachments/assets/889aa9d3-1eac-49ef-98d2-7afe2ed465c3" alt="Material thickness measurement" width="350" />

*Figure 1: Measuring the plywood thickness using calipers.*

### Kerf Testing

Our team used a 20 mm × 20 mm square test coupon to measure the laser kerf. After cutting the square, we measured the finished dimensions in both the X and Y directions using digital calipers.

| Measurement | Value (mm) |
|---|---|
| Designed Square | 20.00 |
| Measured X | 18.94 |
| Measured Y | 18.95 |
| Kerf X | 1.06 |
| Kerf Y | 1.05 |
| **Average Kerf** | **1.055** |

The kerf was calculated by subtracting the measured dimensions from the original designed dimensions.

- Kerf X = 20.00 - 18.94 = 1.06 mm
- Kerf Y = 20.00 - 18.95 = 1.05 mm
- Average Kerf = (1.06 + 1.05) / 2 = 1.055 mm

The measured kerf values were very similar in both directions, with a difference of only 0.01 mm. 

#### Kerf Test Coupon

The square coupon was cut from our plywood sheet to determine how much material was removed during laser cutting.

<img width="242" height="263" alt="image" src="https://github.com/user-attachments/assets/87213f0e-26d6-4598-8a2a-721210c0b275" />

*Figure 2: Laser-cut square coupon and the remaining plywood sheet.*

### Fit Testing and Clearance Selection

After measuring the laser kerf, our team laser cut a test coupon with five different slot widths to determine which connection would provide the best fit. Each slot was tested using a separate plywood piece to compare how tightly the parts connected.

<img width="350" alt="Fit Test Coupon" src="https://github.com/user-attachments/assets/082d86ae-ffd5-49b5-9a84-cf8f0a93f904" />

*Figure 3: Laser-cut clearance test coupon with five different slot widths.*

| Slot | Slot Width (mm) | Fit Result |
|---|---|---|
| 1 | 2.45 | Too tight in both directions |
| 2 | 2.60 | Too tight in both directions |
| 3 | 2.75 | Too loose |
| 4 | 2.90 | Too loose |
| 5 | 3.05 | Too loose |

#### Fit Test Results

Our team found that the smaller slot widths created tighter connections, while the larger slots allowed too much movement between the pieces. We decided to use a tighter press fit for our final flower design to prevent the parts from moving or coming apart during assembly.

<img width="242" alt="Fit Test Results" src="https://github.com/user-attachments/assets/e1cf76bb-5f1d-4269-85c6-354b0923ed00" />

*Figure 4: Testing the tab and slot connections using the laser-cut coupon.*

This testing helped us select a connection that would keep the flower stable without requiring glue, tape, or additional fasteners.

### Parameter Table

| Variable Name | Value | Units | Source | What It Controls |
|---|---|---|---|---|
| Material Thickness | 2.690 | mm | Measured | Material and tab thickness |
| Kerf | 1.055 (pending verification) | mm | Calculated from measurements | Laser cutting allowance |
| Clearance | -0.090 (nominal) | mm | Calculated | Interference between tab and slot |
| Slot Width | 2.60 | mm | Selected from fit testing | Press-fit connections |
| Additional Parameters | TBD | TBD | SolidWorks model | Final flower dimensions |

Our team selected a 2.60 mm slot width based on the fit testing results. Compared to the measured material thickness of 2.690 mm, this creates a nominal interference of 0.090 mm. We chose a tighter press fit to reduce movement and keep the flower securely assembled without glue or tape.

### Parametric CAD Design

Our team designed eight unique parts in SolidWorks, resulting in a total of 16 individual pieces used to assemble the three-dimensional flower. Each component was designed separately with interlocking connections to allow the flower to be assembled without glue, tape, or additional fasteners.

The main design considerations were material thickness, press-fit clearances, stability, and ensuring that all the pieces could be laser cut from a flat sheet of plywood.

#### Leaf Design

We designed two identical leaves to add detail to the flower. Each leaf has a decorative shape with vein details and a tab at the bottom for attaching it to the stem. The tab allows the leaves to connect using a press fit.

<img width="1918" height="1128" alt="image" src="https://github.com/user-attachments/assets/c34dda93-7f1e-4d66-9587-feaed0db3505" />

*Figure 5: SolidWorks model of the leaf showing the decorative shape and connection tab.*

#### Petal Design

We designed eight identical petals to create the flower head. Each petal has a rounded shape with two tabs at the bottom that connect to the center hub. The press-fit connections help keep the petals securely in place and evenly positioned around the flower.

<img width="1917" height="1129" alt="image" src="https://github.com/user-attachments/assets/78cc5937-d178-4452-9bce-b635abc5c352" />

*Figure 6: SolidWorks sketch of the flower petal showing its rounded profile and connection tabs.*

#### Petal Hub Design

The petal hub was designed as a circular piece with eight connection locations around the outside for attaching the petals. A cross-shaped opening in the center allows the hub to connect to the interlocking stem pieces. This design helps position the petals evenly around the flower head.

<img width="1914" height="1131" alt="image" src="https://github.com/user-attachments/assets/0b212af7-ea1b-401b-8d41-e8dd5dba0763" />

*Figure 7: SolidWorks model of the petal hub showing the petal slots and center opening.*

#### Stem Design

We designed two different stem pieces that interlock to create a cross-shaped vertical support for the flower. One stem has a slot extending from the bottom, while the other has a slot extending from the top, allowing them to slide together. Both pieces also have connection tabs for attaching the base and flower head.

<img width="1918" height="1129" alt="image" src="https://github.com/user-attachments/assets/4c87c42a-ddf0-4135-9742-034f90d62bb2" />

*Figure 8: SolidWorks model of Stem Part 1 showing the bottom slot and connection tabs.*

<img width="1918" height="1123" alt="image" src="https://github.com/user-attachments/assets/2b26e2a2-35df-4ce0-9dfb-07f0d7df4f5c" />

*Figure 9: SolidWorks model of Stem Part 2 showing the top slot and connection tabs.*

#### Base Design

We designed two different-sized circular bases to support the flower and keep it standing upright. Both bases have cross-shaped openings in the center that connect to the interlocking stem pieces. The larger base provides additional stability, while the smaller base helps support the stem. We also adjusted the openings to create tighter connections and reduce movement.

<img width="1918" height="1123" alt="image" src="https://github.com/user-attachments/assets/f935e332-38d8-42df-a685-fc27850700e4" />

*Figure 10: SolidWorks model of the smaller circular base.*

<img width="1918" height="1110" alt="image" src="https://github.com/user-attachments/assets/de94c625-b0bf-456d-a52c-c192242398be" />

*Figure 11: SolidWorks model of the larger circular base.*

#### Hub Cover Design

The final component was a circular hub cover designed to hold the petal hub securely in place on the stem. The cover has a square opening in the center that fits over the stem connection. This helps prevent the flower head from moving or sliding off during assembly.

<img width="1918" height="1105" alt="image" src="https://github.com/user-attachments/assets/0e948226-84ec-482e-af12-1a60b5b3d9df" />

*Figure 12: SolidWorks model of the hub cover showing the center opening.*

#### Final Assembly

The final flower consists of 16 individual laser-cut plywood pieces assembled using press-fit connections. The two stem pieces interlock to create the vertical support, while the circular bases help keep the flower standing upright. The leaves attach to the stem, and the eight petals connect to the circular petal hub. The hub cover helps secure the flower head in place.

This design demonstrates how multiple flat components can be combined to create a three-dimensional structure without glue or additional fasteners.

<img width="350" alt="image" src="https://github.com/user-attachments/assets/3e7af856-2eb7-4276-a34f-5d626a3cd839" />

*Figure 13: Final assembled laser-cut plywood flower.*

## Manufacturing

### Process Research

Laser cutting is a manufacturing process that uses a focused laser beam to cut through material along a programmed path. It is useful for producing accurate two-dimensional shapes, including tabs, slots, and other interlocking features.

Compared with FDM 3D printing, laser cutting can be faster for producing flat parts because it does not require building the object layer by layer. However, laser cutting is limited mainly to sheet materials, while FDM printing can produce more complex three-dimensional shapes. Laser cutting was a good manufacturing method for our flower because the individual parts could be cut from a flat sheet and assembled afterward.

### Laser Cutting Setup

Our team used an Epilog laser cutter to manufacture our three-dimensional flower from plywood. We started by cutting a kerf test coupon and a five-slot fit test coupon to determine the appropriate dimensions for our press-fit connections. After testing the pieces, we selected a tighter fit to prevent movement in the final assembly.

The plywood was positioned on the laser bed, and the cutting layouts were arranged to reduce material waste.

### Laser Process Record

Our team used an Epilog CO₂ laser cutter to manufacture our plywood flower. The cutting settings were obtained from the laser cutter's Job Manager print history on October 27, 2026.

| Setting | Value |
|---|---|
| Laser Cutter | Epilog CO₂ Laser |
| Material | Plywood |
| Material Preset | 3 mm |
| Measured Material Thickness | 2.690 mm |
| Vector Cutting Speed | 20% |
| Vector Cutting Power | 100% |
| Vector Frequency Setting | 20% |
| Engraving Speed | 50% |
| Engraving Power | 100% |
| Cutting Method | CO₂ Vector Cutting |
| Cutting Date | October 27, 2026 |
| Cutting Time | 12:34 PM |

The laser cutter was programmed using a 3 mm material preset, although our measured plywood thickness was 2.690 mm. The vector cutting settings were 20% speed, 100% power, and a 20% frequency setting. The engraving settings were 50% speed and 100% power.

These settings were used to manufacture the individual components that were later assembled into our three-dimensional flower.

### Laser Cutting and Assembly

After completing the kerf and clearance tests, our team laser cut the individual components for our three-dimensional flower. The final design consisted of 16 pieces, including two circular bases, two interlocking stem pieces, two leaves, eight petals, a petal hub, and a hub cover.

The pieces were assembled using press-fit connections without glue or tape. We selected tighter connections to help keep the flower stable and prevent movement between the parts.

### Laser Cutting Process

<div style="display: flex; gap: 10px; justify-content: center; align-items: center; width: 100%;">

  <video style="width: 32%;" autoplay muted loop playsinline>
    <source src="/kaileigh-hill-lab-portfolio/Labs/L09/IMG_2106.mp4" type="video/mp4">
  </video>

  <video style="width: 32%;" autoplay muted loop playsinline>
    <source src="/kaileigh-hill-lab-portfolio/Labs/L09/IMG_2107.mp4" type="video/mp4">
  </video>

  <video style="width: 32%;" autoplay muted loop playsinline>
    <source src="/kaileigh-hill-lab-portfolio/Labs/L09/IMG_2111.mp4" type="video/mp4">
  </video>

</div>

*Figure: Laser cutting process showing the manufacturing of the flower components.*

### Layout and Nesting

Our team arranged the individual components on the plywood sheet before laser cutting. The initial test coupons were positioned near the edge of the material to conserve space for the final design.

<img width="350" alt="image" src="https://github.com/user-attachments/assets/94ff28bf-102f-4f4d-ab06-c19d3fcee0eb" />

*Figure: Layout of the flower components after removed from laser cutting.*


### Edge Quality and Cutting Observations

After laser cutting, we noticed darkened edges on the plywood where the laser had passed through the material. The pieces were cut into their individual shapes and assembled using press-fit connections. Our earlier clearance testing helped us choose tighter connections to keep the flower stable without glue or tape.

## Lessons Learned


### Process Log

| Step | What Happened | Decision or Change Made |
|---|---|---|
| Material Measurement | Measured plywood thickness at three locations | Used the 2.690 mm average thickness |
| Kerf Testing | Cut and measured a 20 mm square coupon | Calculated a 1.055 mm average dimensional difference |
| Fit Testing | Tested five different slot widths | Selected 2.60 mm for a tighter press fit |
| Design | Designed eight unique parts in SolidWorks | Created 16 total pieces for the flower |
| Laser Cutting | Cut the flower components using the Epilog laser cutter | Corrected overlapping petal designs that caused multiple laser passes |
| Troubleshooting | The leaves were too loose during assembly | Recut the leaves multiple times and adjusted the connections |
| Final Assembly | Assembled the flower using the laser-cut plywood pieces | Completed the flower without glue, tape, or additional fasteners |


### Mistakes and Troubleshooting

One challenge was determining the correct clearance for the press-fit connections. During testing, we found that the smaller slots were too tight, while the larger slots allowed too much movement. We decided to use a 2.60 mm slot width to create tighter connections and keep the flower stable.

While laser cutting the petals, we accidentally had the designs copied directly on top of each other in the cutting file. This caused the laser to make multiple passes over the same pieces instead of cutting them once. We corrected the overlapping designs to prevent unnecessary cutting.

We also had to recut the leaves multiple times because the original connections were too loose. We adjusted the connection dimensions to create a tighter fit so the leaves would stay securely attached to the stem.

Overall, these mistakes showed us how important it is to check the cutting layout and test the connections before manufacturing the final pieces.

### Resources Used

| Resource | Description |
|---|---|
| Material | Plywood |
| Sheet Size | 12 × 12 in |
| Average Material Thickness | 2.690 mm |
| Laser Cutter | Epilog CO₂ Laser |
| Measurement Tool | Digital Calipers |
| CAD Software | SolidWorks |
| Assembly Method | Press-fit tabs and slots |
| Additional Fasteners | None |
| Adhesives | None |

### Reflection

**1. Where did your measured values differ from what you assumed?**

The plywood measured an average thickness of 2.690 mm, which was slightly smaller than the 3 mm material preset. We also found that different slot widths created very different fits, showing why testing the actual material was important.

**2. How does Taguchi's quality loss function relate to a joint that works but is not on target?**

Taguchi's quality loss function shows that even if a joint works, it can still lose quality when it differs from the intended dimensions. A connection that is too tight or too loose may still assemble, but it can affect the stability and overall quality of the flower.

**3. What real product uses cut sheet parts joined by tabs and slots?**

Flat-pack furniture is a good example because individual panels are cut separately and assembled using interlocking connections. Our flower uses a similar idea by combining flat pieces into a three-dimensional structure.

**4. If you had one more cut, what would you change and why?**

If we had one more cut, I would focus on improving the fit between the stem, base, and flower head. Small adjustments to the connection dimensions could make the flower easier to assemble while still keeping the parts securely connected.

### Total Time Spent

Our team spent approximately 4 hours completing the laser cutting lab, from 9:00 AM to 1:00 PM. This included measuring the material, testing clearances, designing the flower, laser cutting, troubleshooting, and assembling the final product.

| Task | Time Spent |
|---|---|
| Material Measurement | 15 minutes |
| Kerf and Fit Testing | 30 minutes |
| SolidWorks Design | 1 hour 15 minutes |
| Laser Cutting | 45 minutes |
| Troubleshooting and Recutting | 45 minutes |
| Final Assembly | 30 minutes |
| **Total Time Spent** | **4 hours** |

Overall, the most time-consuming parts were designing the individual components in SolidWorks and making adjustments during manufacturing. The additional cutting and troubleshooting helped us improve the fit and stability of the final flower.
