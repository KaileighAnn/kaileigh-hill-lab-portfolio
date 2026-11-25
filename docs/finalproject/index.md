# Final Project – Automatic Dog Feeder

<div style="background-color:#E92063; color:white; padding:20px; border-radius:8px; margin-top:25px;">
  <h2 style="color:white; margin:0;">Week 1: Initial Design & Development</h2>
  <p style="margin-bottom:0;">Final Project 1/2</p>
</div>

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

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/a598f658-869d-4c19-b28f-fe8e500b43d8" />

*Figure 1: SolidWorks model of the laser-cut base showing the bowl opening, mounting holes, and assembly slots.*

### Side Panels – Laser Cutting

I modeled two identical side panels that will be manufactured using the laser cutter. These panels support the upper structure of the feeder and connect to the base using interlocking tabs and slots.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/17ca313e-3e3e-4ea6-8861-db00e044ad5b" />

*Figure 2: SolidWorks model of one of the two laser-cut side panels showing the interlocking features.*

### Food Slide – FDM Printing (PLA)

I modeled a sloped food slide in SolidWorks that will be 3D printed using PLA. The slide directs the dog food from the storage container down into the bowl using gravity.

I added raised edges to prevent food from spilling off the sides and a support underneath to help keep the slide in position.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/1107ca60-6f76-4162-b96c-a4e250d821ba" />

*Figure 3: SolidWorks model of the PLA food slide with raised edges and support.*

### Food Holder – FDM Printing (PLA)

I modeled the food holder using loft and shell features in SolidWorks. The container has a wide rectangular opening at the top that gradually narrows toward the bottom to direct the dog food toward the dispensing mechanism.

This part will be 3D printed using PLA and positioned above the food slide. A servo-controlled sliding gate will eventually be added underneath to control when food is released.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/27fd67b1-451b-4754-9224-f0a4f0ff0912" />

*Figure 4: SolidWorks model of the PLA food holder showing the tapered design and bottom outlet.*

### Food Holder Lid – FDM Printing (PLA)

I modeled a removable lid in SolidWorks that will be 3D printed using PLA. The lid fits over the top of the food holder to keep the dog food contained while allowing easy access for refilling.

I used the Shell feature to create a recessed underside that fits over the container. I also plan to mount the Arduino on top of the lid to keep the electronics separate from the food.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/7192d240-fa44-4f0b-b46b-7c163a5fabad" />

*Figure 5: SolidWorks model of the PLA food holder lid with a recessed underside.*

### Food Holder Support – Laser Cutting

I modeled the top support panel in SolidWorks, which will be manufactured using the laser cutter. This piece supports the food holder and has a circular opening that allows food to pass from the container into the slide below.

I also added rectangular slots along the edges so the panel can connect to the two side supports.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/287e9d92-3237-458a-b571-fc3f84d13ee4" />

*Figure 6: SolidWorks model of the laser-cut top support panel showing the food opening and assembly slots.*

### Sliding Gate Mechanism – FDM Printing (PLA) and SLA

For the food dispensing mechanism, I found an existing rack-and-pinion gate design that I could modify for my automatic dog feeder.

The mechanism consists of a sliding gate, pinion gear, and motor support. The motor will rotate the gear, moving the gate horizontally to open and close the food holder's outlet.

I imported the original parts into SolidWorks and modified the sliding gate to fit over the opening of my food holder. The remaining components will be tested and adjusted as needed.

**Original Design:** https://makerworld.com/en/models/1742712-automatic-sliding-gate-sg90-servo?utm_source=chatgpt.com#profileId-1852158

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/29e505f2-33c5-41b0-9eaa-87e49117abe7" />

*Figure X: Original sliding gate, motor support, and pinion gear imported into SolidWorks.*

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/580c611f-eccb-4ec7-bba5-c112f04826c1" />

*Figure X: Modified sliding gate designed to cover the food holder opening.*

### Manufacturing Summary

| Component | Manufacturing Method | Quantity |
|---|---|---|
| Base | Laser Cutting | 1 |
| Side Panels | Laser Cutting | 2 |
| Food Slide | FDM – PLA | 1 |
| Food Holder | FDM – PLA | 1 |
| Food Holder Lid | FDM – PLA | 1 |
| Food Holder Support | Laser Cutting | 1 |
| Sliding Gate | FDM – PLA | 1 |
| Motor Mount/Support | FDM – PLA | 1 |
| Pinion Gear | SLA – Resin | 1 |
| **Total** | | **10** |

### Design Progress

So far, I have modeled six different components in SolidWorks that will make up the main structure of the automatic dog feeder.

The next step is to finish designing the Arduino-controlled sliding gate mechanism, including the gate, guide rails, servo mount, and linkage. Once these parts are completed, I will test their fit and movement before manufacturing the final prototype.

### SolidWorks Assembly

After modeling the individual components, I combined them into a SolidWorks assembly to check how everything fits together.

The assembly includes the base, side panels, food slide, food holder, lid, top support, and 8-inch dog bowl. This helped me visualize the final design and check the positioning of each component before manufacturing.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/a58dd45a-fa1f-44bb-8b22-0f8809490ac5" />

*Figure X: SolidWorks assembly of the automatic dog feeder showing the overall design and component placement.*

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

<img width="1152" height="1536" alt="image" src="https://github.com/user-attachments/assets/bec27201-0f91-4379-afa5-ee2903f97ef9" />

---

<div style="background-color:#E92063; color:white; padding:20px; border-radius:8px; margin-top:25px;">
  <h2 style="color:white; margin:0;">Week 2: Prototype Refinement & Final Presentation</h2>
  <p style="margin-bottom:0;">Final Project 2/2</p>
</div>

## Objective

During the second week of my final project, I focused on
refining my initial design, incorporating peer feedback,
manufacturing the final components, and testing the
functionality of my automatic dog feeder.

## Peer Feedback & Individual Reflections

After presenting my initial design for Dixie's Automatic Dog Feeder, I received feedback from three of my peers. Their feedback helped me identify potential improvements regarding functionality, manufacturing tolerances, safety, and durability.

---

### Peer Feedback #1 – Candy

<p align="center">
  <img width="40%" alt="Candy's feedback - Front" src="https://github.com/user-attachments/assets/9f830393-98eb-4897-84da-3855c9f762a9" />
  <img width="40%" alt="Candy's feedback - Back" src="https://github.com/user-attachments/assets/41bd6539-81d3-4539-b3c2-eccb38275d39" />
</p>

<p align="center">
  <em>Figure 1: Front and back of Candy's peer feedback worksheet.</em>
</p>

#### Individual Reflection

Candy's feedback made me think more about manufacturing tolerances, specifically the kerf of the laser-cut components and how everything would fit together. She also brought up the importance of making sure the opening mechanism would not hurt Dixie. This encouraged me to pay closer attention to the overall dimensions and safety of my design.

---

### Peer Feedback #2 – Ameer

<p align="center">
  <img width="40%" alt="Ameer's feedback - Front" src="https://github.com/user-attachments/assets/403aa212-3cbd-411b-ab53-395962a20085" />
  <img width="40%" alt="Ameer's feedback - Back" src="https://github.com/user-attachments/assets/4c8621e7-4468-4eb1-b4f7-2e3ac067b887" />
</p>

<p align="center">
  <em>Figure 2: Front and back of Ameer's peer feedback worksheet.</em>
</p>

#### Individual Reflection

Ameer's feedback focused on making sure all the components worked together properly and that the correct amount of food could fit into the bowl. During testing, I realized that my original gate opening was larger than necessary and that my pinion gear was sitting at an angle. I redesigned the sliding gate to reduce the opening size and identified the gear alignment as another area that needed improvement.

---

### Peer Feedback #3 – Austin

<p align="center">
  <img width="40%" alt="Austin's feedback - Front" src="https://github.com/user-attachments/assets/40e97381-a6a1-44dc-b93b-b731de1938f0" />
  <img width="40%" alt="Austin's feedback - Back" src="https://github.com/user-attachments/assets/13fd149f-f1e7-4882-b4ed-0e97958534d9" />
</p>

<p align="center">
  <em>Figure 3: Front and back of Austin's peer feedback worksheet.</em>
</p>

#### Individual Reflection

Austin brought up a concern that I had not really considered, which was Dixie potentially destroying the feeder to get to the food. This made me think more about the durability of my design and how I could prevent unwanted access to the food. A locking mechanism would be a good improvement to consider in a future iteration.

---

### Overall Feedback Reflection

Overall, receiving feedback from my peers helped me look at my design from different perspectives. It allowed me to identify potential issues with functionality, safety, and manufacturing that I may not have considered on my own. I used this feedback, along with my own testing, to guide the refinement of my prototype.

---
