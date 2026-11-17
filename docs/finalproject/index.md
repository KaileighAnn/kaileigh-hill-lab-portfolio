
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

Feeding a dog at consistent times can be difficult when school, work, and other responsibilities interfere with a normal schedule. Delayed feeding can disrupt a dog's routine.

An automatic feeder could help maintain a more consistent feeding schedule.

### Problem 2: Dog Food Spilling Around the Bowl

When pouring food into a dog bowl, kibble can spill onto the floor. This creates a mess and wastes food.

A controlled dispensing system with a chute could help direct the food into the bowl.

### Problem 3: Inconsistent Food Portions

It can be difficult to dispense the same amount of food every time, especially when feeding quickly.

A controlled dispensing mechanism could help regulate the amount of food released.

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
- Servo motor and mounting bracket
- Arduino controller
- Removable dog bowl

The dog bowl has a diameter of approximately 8 inches, which was used to help determine the size of the stand.

### Manufacturing Methods

**FDM Printing:** I plan to use FDM printing for the sliding gate, guide rails, servo mount, and other mechanical components.

**Laser Cutting:** I plan to use laser cutting for the main support frame and structural panels.

**SLA Printing (Optional):** SLA may be used for a small precision component if additional dimensional accuracy is needed.

### Initial SolidWorks Model

I began developing the feeder in SolidWorks by modeling the main structure, food container, and sloped chute.

The current design positions the food storage container above the chute so gravity can move the food toward the bowl.

**[INSERT FIGURE 1: Initial SolidWorks assembly]**

*Figure 1: Initial SolidWorks model of the automatic dog feeder.*

### Sliding Gate Concept

After developing the initial assembly, I selected a servo-operated sliding gate to control food release.

The gate will move horizontally underneath the hopper opening. When closed, it prevents food from leaving the container. When opened, food can fall onto the chute.

A servo motor will operate the gate using a mechanical linkage.

**[INSERT FIGURE 2: Sliding gate concept or CAD model]**

*Figure 2: Proposed servo-operated sliding gate mechanism.*

## 5. Testing Critical Features

The main feature that needs testing is the sliding gate mechanism.

I plan to test:

- Clearance between the sliding gate and guide rails
- Ability of the servo to open and close the gate
- Whether kibble jams inside the mechanism
- Whether food travels down the chute into the bowl
- Whether the gate closes completely

I will first manufacture a small test section of the sliding mechanism before producing the final components.

**[INSERT TEST RESULTS AFTER MANUFACTURING]**

**[INSERT FIGURE 3: Sliding gate test piece]**

*Figure 3: Initial sliding gate prototype used to evaluate fit and movement.*

## 6. Initial Design Evaluation

The initial SolidWorks model establishes the overall layout of the feeder, including the food storage container, support frame, chute, and bowl placement.

The next step is to complete the sliding gate mechanism and determine how the servo motor will connect to it.

One concern is that food may become stuck between the gate and hopper opening. I will need to test different clearances and possibly adjust the opening to improve reliability.

Another consideration is controlling the amount of food dispensed. The initial design uses a timed gate opening, but additional testing will be needed to determine whether this provides consistent portions.

## 7. Video Presentation

**[INSERT 30-SECOND VIDEO EXPLAINING THE PROBLEM]**

The video will explain the difficulty of maintaining consistent feeding times, introduce the automatic feeder concept, and demonstrate how the food will travel from the storage container into the bowl.

## 8. Next Steps

During the next stage of the project, I plan to finish the SolidWorks assembly, manufacture the sliding gate, and test the mechanism.

I will use the results to improve the design before manufacturing and assembling the final prototype.
