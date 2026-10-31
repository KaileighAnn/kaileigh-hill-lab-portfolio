
### Laser Cutting Process

<div style="display: flex; gap: 10px; justify-content: center; width: 100%;">

  <video width="30%" controls autoplay muted loop playsinline>
    <source src="/kaileigh-hill-lab-portfolio/Labs/L09/IMG_2106.MOV" type="video/quicktime">
  </video>

  <video width="30%" controls autoplay muted loop playsinline>
    <source src="/kaileigh-hill-lab-portfolio/Labs/L09/IMG_2107.MOV" type="video/quicktime">
  </video>

  <video width="30%" controls autoplay muted loop playsinline>
    <source src="/kaileigh-hill-lab-portfolio/Labs/L09/IMG_2111.MOV" type="video/quicktime">
  </video>

</div>

*Figure: Laser cutting process showing the manufacturing of the flower components.*



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

The flower consists of 16 total pieces and 6 unique part types:

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

The average material thickness was 2.690 mm. This value will be used as a parameter in our CAD model to help ensure accurate connections between parts.

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

The measured kerf values were very similar in both directions, with a difference of only 0.01 mm. We will verify the original square dimensions and cutting scale before using this value in our final CAD model.

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

<img width="1152" height="1536" alt="image" src="https://github.com/user-attachments/assets/3e7af856-2eb7-4276-a34f-5d626a3cd839" />

*Figure 13: Final assembled laser-cut plywood flower.*

## Manufacturing

### Process Research

Laser cutting is a manufacturing process that uses a focused laser beam to cut through material along a programmed path. It is useful for producing accurate two-dimensional shapes, including tabs, slots, and other interlocking features.

Compared with FDM 3D printing, laser cutting can be faster for producing flat parts because it does not require building the object layer by layer. However, laser cutting is limited mainly to sheet materials, while FDM printing can produce more complex three-dimensional shapes. Laser cutting is a good manufacturing method for our construction kit because the individual parts can be cut from a flat sheet and assembled afterward.

### Laser Cutting Setup

Our team used an Epilog laser cutter to cut the test coupons from a 12 × 12 inch plywood sheet. We positioned the material on the laser bed and arranged the test pieces near the edge of the sheet to conserve material for the final construction kit.

<!-- Insert laser cutter setup photo here -->

*Figure 5: Plywood sheet positioned inside the Epilog laser cutter before cutting.*

### Laser Process Record

| Setting | Kerf Coupon | Fit Coupon | Final Cut |
|---|---|---|---|
| Laser Cutter | Epilog | Epilog | TBD |
| Material Type | Plywood | Plywood | TBD |
| Nominal Thickness | TBD | TBD | TBD |
| Measured Thickness (Mean) | 2.690 mm | 2.690 mm | TBD |
| Speed | TBD | TBD | TBD |
| Power | TBD | TBD | TBD |
| Frequency/PPI | TBD | TBD | TBD |
| Number of Passes | TBD | TBD | TBD |
| Focus Method and Confirmation | TBD | TBD | TBD |
| Air Assist On? Exhaust On? | TBD | TBD | TBD |
| Origin and Alignment | TBD | TBD | TBD |

### Laser Cutting and Assembly

Our team completed the initial kerf and clearance test cuts. These tests will help us determine the correct dimensions before manufacturing the final construction kit.

The final cutting process, assembly, and results will be documented after the design is completed.

<!-- Insert continuous laser cutting video here -->

### Layout and Nesting

The initial test coupons were placed near the edge of the plywood sheet to reduce material waste and preserve space for the remaining parts.

The final nesting layout will be documented after the construction kit is designed.

### Edge Quality and Cutting Observations

The test pieces show darkened edges from the laser cutting process. We will document any soot, charring, or other cutting issues and describe any adjustments made to improve the final parts.

Air assist and exhaust observations will be added after confirming the machine settings.

## Lessons Learned

### Process Log

| Date and Time | Time Spent | Step | What Happened | Decision or Change Made |
|---|---|---|---|---|
| TBD | TBD | Material Measurement | Measured plywood thickness at three locations | Used 2.690 mm as the average thickness |
| TBD | TBD | Kerf Testing | Cut and measured a 20 mm square coupon | Calculated 1.055 mm average kerf; verification pending |
| TBD | TBD | Fit Testing | Cut a five-slot test coupon and tested a separate piece | Final clearance selection pending |
| TBD | TBD | Design | TBD | TBD |
| TBD | TBD | Final Manufacturing | TBD | TBD |

**Total Time Spent:** TBD

### Mistakes and Troubleshooting

To be completed as the project progresses.

### Resources Used

| Resource | Description |
|---|---|
| Material | Plywood |
| Sheet Size | 12 × 12 in |
| Average Material Thickness | 2.690 mm |
| Number of Sheets | TBD |
| Laser Cutter | Epilog |
| Measurement Tool | Calipers |
| CAD Software | TBD |
| Assembly Tools | TBD |
| Consumables and Cleanup Tools | TBD |

### Reflection

**1. Where did your measured values differ from what you assumed?**

To be completed after verifying the kerf measurements and final dimensions.

**2. How does Taguchi's quality loss function relate to a joint that works but is not on target?**

To be completed after testing the final connections.

**3. What real product uses cut sheet parts joined by tabs and slots?**

To be completed.

**4. If you had one more cut, what would you change and why?**

To be completed after the final assembly.
