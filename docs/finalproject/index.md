
# Final Project – Week 1

## Automatic Dog Feeder

## Objective

The objective of this project is to design and manufacture a functional prototype that solves a real-world problem using at least two manufacturing technologies. The project follows the Spiral Design Process to develop, test, and improve the design.

For my final project, I chose to design an automatic dog feeder that uses an Arduino-controlled servo motor to release food into a bowl.

## 1. Research

### Spiral Design Process

The Spiral Design Process is an iterative approach that allows a design to be improved through repeated cycles.

- **Planning:** Identify the problem, establish requirements, and develop possible solutions.
- **Risk Analysis:** Identify potential problems with the design, materials, or manufacturing process.
- **Engineering:** Create models, manufacture prototypes, and develop the mechanism.
- **Evaluation:** Test the prototype, identify improvements, and use the results to guide the next iteration.

I will use this process to develop the feeder, test the sliding mechanism, and make improvements based on how well the parts fit and function.

### FDM Anisotropy

FDM printing creates parts by depositing layers of melted filament. Because the bonding between layers is generally weaker than the material within each layer, printed parts are anisotropic.

For my project, this could affect the sliding gate, servo mount, and other components that experience forces during operation.

I plan to orient the parts so that the main forces act along the printed layers when possible. I will also consider wall thickness, infill, and print orientation to improve strength.

### SLA Shrinkage

SLA printing uses light to cure liquid resin into solid parts. Resin can shrink during printing and post-curing, affecting dimensional accuracy.

Shrinkage varies depending on the resin, part geometry, orientation, and curing conditions. Small dimensional changes can affect the fit of moving parts.

If I use SLA for a precision component, I will print a test piece, measure its actual dimensions, and adjust the CAD model as needed.

### Laser Cutting Kerf

Laser cutting removes a small amount of material as the laser passes through the sheet. This removed material is called the kerf.

Kerf affects the dimensions of cut parts and the fit of interlocking joints.

For the feeder stand, I plan to measure the material thickness and test the fit of laser-cut joints before manufacturing the final frame. I can adjust the slot dimensions to compensate for kerf.


## 2. Problem Definition

### Problem 1: Inconsistent Dog Feeding Times

Next semester, I have a heavy class schedule, which will make it difficult to always be home to feed my dog, Dixie Mae, on time. I want to find a way to make sure she is fed consistently, even when I am away.

One possible solution is an automatic dog feeder that uses an Arduino-controlled mechanism to release food into her bowl at scheduled times.

### Problem 2: Grocery Bags Moving Around While Driving

Whenever I go grocery shopping, my bags tend to slide around or tip over in my car while I am driving. This causes groceries to spill out and makes unloading everything more difficult.

One possible solution is a removable grocery bag holder that keeps the bags upright and secured while driving. I could design adjustable supports or hooks to hold the bags in place.

### Problem 3: Folding Shelf That Will Not Stay Up

I have a folding shelf that is supposed to stay in an upright position when not in use. However, it does not stay up on its own and keeps falling back down.

One possible solution is a locking bracket or latch that holds the shelf securely in its folded position but can easily be released when I need to use it.

## 3. Problem Selection

I selected the problem of inconsistent dog feeding times.

My goal is to design an automatic feeder that stores dry dog food and releases it into a bowl using an Arduino-controlled servo motor.

I chose this project because it solves a practical problem while allowing me to combine mechanical design, manufacturing, and programming.

## 4. Concept Development

### Initial Design

My initial concept consists of a raised stand with a food storage container at the back and a dog bowl at the front.

A sloped chute connects the food container to the bowl. When the servo motor opens a sliding gate underneath the container, food is released onto the chute and travels down into the bowl.

The design includes:

- Food storage hopper
- Raised support frame
- Sloped food chute
- Sliding gate mechanism
- Servo motor 
- Arduino controller
- Removable dog bowl

The dog bowl has a diameter of approximately 8 inches, which was used to help determine the size of the stand.

### Manufacturing Methods

**FDM Printing:** I plan to use FDM printing for the sliding gate, guide rails, and other mechanical components.

**Laser Cutting:** I plan to use laser cutting for the main support frame and structural panels.

**SLA Printing (Optional):** SLA may be used for a small precision component like the gear for the motor.


## 4. SolidWorks CAD Design and Manufacturing

I began designing my automatic dog feeder in SolidWorks by modeling each component separately before combining them into an assembly. The design uses both laser cutting and FDM printing to manufacture the different parts.

The feeder consists of a raised frame, food storage container, removable lid, sloped food slide, and a bowl positioned at the front. The goal is to allow food to travel from the container down the slide and into the bowl using gravity.

### Base – Laser Cutting

I modeled the base in SolidWorks to support the feeder structure. I added a curved opening to accommodate the 8-inch dog bowl, allowing it to be easily accessed and removed.

The base also includes rectangular slots for connecting the side panels and mounting holes for additional components.

**[INSERT FIGURE 1: BASE SOLIDWORKS MODEL]**

*Figure 1: SolidWorks model of the laser-cut base showing the bowl opening, mounting holes, and assembly slots.*

### Side Panels – Laser Cutting

I modeled two identical side panels that will be manufactured using the laser cutter. These panels support the upper structure of the feeder and connect to the base using interlocking tabs and slots.

**[INSERT FIGURE 2: SIDE PANEL SOLIDWORKS MODEL]**

*Figure 2: SolidWorks model of one of the two laser-cut side panels showing the interlocking features.*

### Food Slide – FDM Printing (PLA)

I modeled a sloped food slide in SolidWorks that will be 3D printed using PLA. The slide directs the dog food from the storage container down into the bowl using gravity.

I added raised edges to prevent food from spilling off the sides and a support underneath to help keep the slide in position.

**[INSERT FIGURE 3: FOOD SLIDE SOLIDWORKS MODEL]**

*Figure 3: SolidWorks model of the PLA food slide with raised edges and support.*

### Food Holder – FDM Printing (PLA)

I modeled the food holder using loft and shell features in SolidWorks. The container has a wide rectangular opening at the top that gradually narrows toward the bottom to direct the dog food toward the dispensing mechanism.

This part will be 3D printed using PLA and positioned above the food slide. A servo-controlled sliding gate will eventually be added underneath to control when food is released.

**[INSERT FIGURE 4: FOOD HOLDER SOLIDWORKS MODEL]**

*Figure 4: SolidWorks model of the PLA food holder showing the tapered design and bottom outlet.*

### Food Holder Lid – FDM Printing (PLA)

I modeled a removable lid in SolidWorks that will be 3D printed using PLA. The lid fits over the top of the food holder to keep the dog food contained while allowing easy access for refilling.

I used the Shell feature to create a recessed underside that fits over the container. I also plan to mount the Arduino on top of the lid to keep the electronics separate from the food.

**[INSERT FIGURE 5: FOOD HOLDER LID SOLIDWORKS MODEL]**

*Figure 5: SolidWorks model of the PLA food holder lid with a recessed underside.*

### Food Holder Support – Laser Cutting

I modeled the top support panel in SolidWorks, which will be manufactured using the laser cutter. This piece supports the food holder and has a circular opening that allows food to pass from the container into the slide below.

I also added rectangular slots along the edges so the panel can connect to the two side supports.

**[INSERT FIGURE 6: FOOD HOLDER SUPPORT SOLIDWORKS MODEL]**

*Figure 6: SolidWorks model of the laser-cut top support panel showing the food opening and assembly slots.*

### Manufacturing Summary

| Component | Manufacturing Method | Quantity |
|---|---|---|
| Base | Laser Cutting | 1 |
| Side Panels | Laser Cutting | 2 |
| Food Slide | FDM – PLA | 1 |
| Food Holder | FDM – PLA | 1 |
| Food Holder Lid | FDM – PLA | 1 |
| Food Holder Support | Laser Cutting | 1 |
| **Total** | | **7** |

### Design Progress

So far, I have modeled six different components in SolidWorks that will make up the main structure of the automatic dog feeder.

The next step is to finish designing the Arduino-controlled sliding gate mechanism, including the gate, guide rails, servo mount, and linkage. Once these parts are completed, I will test their fit and movement before manufacturing the final prototype.

## 5. Testing Critical Features

### Laser Cutting Kerf and Fit Testing

For this project, I used my Lab 9 kerf and fit testing results to help design the interlocking connections for my automatic dog feeder.

### Material Thickness

I measured the plywood thickness at three locations using digital calipers.

| Measurement | Thickness (mm) |
|---|---|
| Location 1 | 2.69 |
| Location 2 | 2.68 |
| Location 3 | 2.70 |
| **Average** | **2.690** |

The average thickness of **2.690 mm** was used as a reference when designing the laser-cut connections.

<img src="https://github.com/user-attachments/assets/889aa9d3-1eac-49ef-98d2-7afe2ed465c3" alt="Material thickness measurement" width="350" />

*Figure X: Measuring plywood thickness using digital calipers.*

### Kerf Testing

We cut a 20 × 20 mm square and measured the finished dimensions to determine the material removed during laser cutting.

| Measurement | Value (mm) |
|---|---|
| Designed Square | 20.00 |
| Measured X | 18.94 |
| Measured Y | 18.95 |
| **Average Dimensional Reduction** | **1.055** |

Average reduction = [(20 - 18.94) + (20 - 18.95)] / 2 = **1.055 mm**

These measurements helped me understand how laser cutting affects dimensional accuracy.

<img width="242" height="263" alt="image" src="https://github.com/user-attachments/assets/87213f0e-26d6-4598-8a2a-721210c0b275" />

*Figure X: Laser-cut kerf test coupon from Lab 9.*

### Fit Testing

We tested five different slot widths to determine which provided the best connection.

| Slot Width (mm) | Result |
|---|---|
| 2.45 | Too tight |
| 2.60 | Too tight |
| 2.75 | Too loose |
| 2.90 | Too loose |
| 3.05 | Too loose |

We selected **2.60 mm** for our Lab 9 project because it provided a tighter connection.

<img width="350" alt="Fit Test Coupon" src="https://github.com/user-attachments/assets/082d86ae-ffd5-49b5-9a84-cf8f0a93f904" />

*Figure X: Laser-cut fit coupon used to test different slot widths.*

### Application to My Final Project

I used the **2.690 mm material thickness** and **2.60 mm slot width** as references when designing the feeder's base, side panels, and top support.

Since the 2.60 mm slot produced a tight fit, I will test the final connections before assembly and adjust them if needed.

I also plan to test the servo-controlled sliding gate to ensure it opens, closes, and releases food without jamming.

## 6. Initial Design Evaluation

The initial SolidWorks model establishes the overall layout of the feeder, including the food storage container, support frame, chute, and bowl placement.

The next step is to complete the sliding gate mechanism and determine how the servo motor will connect to it.

One concern is that food may become stuck between the gate and hopper opening. I will need to test different clearances and possibly adjust the opening to improve reliability.

Another consideration is controlling the amount of food dispensed. The initial design uses a timed gate opening, but additional testing will be needed to determine whether this provides consistent portions.

## 7. Video Presentation

For my final project, I introduced my dog, Dixie, and explained the problem I am trying to solve. With my heavy class schedule next semester, I want to make sure she is fed consistently, even when I am not home.

<video width="100%" controls>
 <source src="/kaileigh-hill-lab-portfolio/finalproject/Dixie_Mae_Feeder_Introduction.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

*Video 1: Introducing Dixie and explaining the problem my automatic dog feeder will solve.*

## 8. Next Steps

During the next stage of the project, I plan to finish the SolidWorks assembly, manufacture the sliding gate, and test the mechanism.

I will use the results to improve the design before manufacturing and assembling the final prototype.
