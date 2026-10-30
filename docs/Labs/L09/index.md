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

To be completed after selecting the final design and clearance.

We will use parameters to control the material thickness, kerf, clearance, and important dimensions. This will allow the model to update when a variable is changed.

<!-- Insert CAD screenshots and before/after parameter changes here -->

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
