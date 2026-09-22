# Lab #5 - Design a Snap Fit

## Design

### Objective

The objective of this assignment was to design and 3D print a two-component snap-fit assembly. The connection must use elastic deformation so that one component can flex during assembly and return to its original position to lock the two parts together.

For my design, I created a wall-mounted keychain holder. The assembly consists of a stationary base and a removable keychain insert. The keychain uses two flexible cantilever arms with snap protrusions. When the keychain is inserted into the base, the arms flex inward and then return outward to lock into place. The arms can be squeezed inward again to remove the keychain.

### Design Concept

I wanted to make a snap-fit that was functional instead of only demonstrating the mechanism. I chose a keychain holder because the snap-fit can be used to quickly attach and remove a set of keys from a wall-mounted base.

My design was inspired by the mechanism used in plastic backpack buckles. These buckles use flexible arms that bend inward during insertion and spring back outward after passing the retaining features.

The final design has two components:

- **Base:** Rigid component that can remain mounted to a wall and contains the retaining features for the snap-fit.
- **Keychain:** Removable component containing two flexible arms, snap protrusions, and an attachment point for keys.

### How the Snap-Fit Works

During insertion, the angled faces on the snap protrusions contact the base and force the two flexible arms inward. The arms behave like cantilever beams and elastically deform as the keychain enters the base.

Once the protrusions pass the retaining features, the arms return toward their original positions and lock the keychain into the base.

To remove the keychain, the two flexible arms are squeezed inward until the snap protrusions clear the retaining features. The keychain can then be pulled out of the base.


# Modeling

## Research

### PLA Material Properties

I chose PLA because it is commonly used for FDM printing and was available for this project. I researched the mechanical properties of PLA before completing the flexure calculations.

The material properties used were:

- **Young's Modulus:** 3,250 MPa ≈ 471,000 psi
- **Yield Strength:** 52.5 MPa ≈ 7,615 psi
- **Safety Factor:** 3.5

Using the required safety factor:

σ_allow = σ_y / SF

σ_allow = 7,615 / 3.5

**σ_allow = 2,176 psi**

Source:

[UltiMaker PLA Technical Data Sheet](https://um-support-files.ultimaker.com/materials/2.85mm/tds/PLA/Ultimaker-PLA-TDS-v5.00.pdf)

### Design Loads

I selected loads within the ranges required for the assignment.

- **Transverse load:** 0.25 lbf
- **Axial load:** 5 lbf

I selected the minimum required loads because the final part is a small keychain holder and is not intended to support a large structural load.


## Engineering Analysis

The flexible arms of the keychain were modeled as cantilever beams. During insertion, the snap features contact the base and cause the arms to bend inward. Once the snap features pass the retaining edge, the arms return toward their original position and lock the keychain into place.

### Design Values

- Material: PLA
- Safety Factor: 3.5
- Young's Modulus: 471,000 psi
- Yield Strength: 7,615 psi
- Allowable Stress: 2,176 psi
- Flexible Arm Length: 5.00 in
- Flexible Arm Width: 0.50 in
- Part Thickness: 0.95 in
- Snap Protrusion: 0.60 in
- Transverse Load: 0.25 lbf
- Axial Load: 5 lbf

### Area Moment of Inertia

For the rectangular cross-section of one flexible arm:

I = bh³ / 12

Using:

b = 0.95 in  
h = 0.50 in

I = (0.95)(0.50)³ / 12

**I = 0.00990 in⁴**

### Cantilever Beam Deflection

The cantilever beam equation for a concentrated load at the free end is:

δ = FL³ / 3EI

where:

- δ = deflection
- F = transverse force
- L = flexible arm length
- E = Young's modulus
- I = area moment of inertia

Using:

F = 0.25 lbf  
L = 5.00 in  
E = 471,000 psi  
I = 0.00990 in⁴

δ = (0.25)(5.00)³ / [3(471,000)(0.00990)]

**δ = 0.00224 in**

The calculated elastic deflection of one arm under the selected transverse load is approximately **0.00224 in**.

### Flexure Length Equation

The cantilever beam equation can also be rearranged to solve for the required flexure length:

L = ∛(3EIδ / F)

The final design uses a **5.00 in flexure length**. The length, width, and thickness were kept as design parameters so the flexure geometry could be adjusted while maintaining the same beam relationship.

### Bending Stress

The maximum bending stress in one flexible arm was calculated using:

σ = Mc / I

where:

M = FL  
c = h / 2

Using:

F = 0.25 lbf  
L = 5.00 in  
h = 0.50 in  
I = 0.00990 in⁴

M = (0.25)(5.00)

M = 1.25 lbf·in

c = 0.50 / 2

c = 0.25 in

σ = (1.25)(0.25) / 0.00990

**σ_b = 31.6 psi**

The allowable stress is:

σ_allow = 7,615 / 3.5

**σ_allow = 2,176 psi**

Since:

31.6 psi < 2,176 psi

the calculated bending stress is below the allowable stress for PLA under the assumed loading.

### Axial Stress

The snap-fit must support an axial load of **5 lbf**. Since the design has two flexible arms, I assumed the load is divided equally between them.

F_arm = 5 / 2

**F_arm = 2.5 lbf**

The cross-sectional area of one arm is:

A = bh

A = (0.95)(0.50)

**A = 0.475 in²**

The axial stress is:

σ_axial = F / A

σ_axial = 2.5 / 0.475

**σ_axial = 5.26 psi**

Since:

5.26 psi < 2,176 psi

the calculated axial stress is below the allowable stress for PLA under the assumed loading.

### Average Shear Stress

The snap protrusions hold the keychain inside the base. Since there are two snap features, I assumed the 5 lbf axial load is divided equally between them.

F_hook = 5 / 2

**F_hook = 2.5 lbf**

Using the snap protrusion dimensions:

A_shear = (0.95)(0.99)

**A_shear = 0.9405 in²**

The average shear stress is:

τ_avg = F / A

τ_avg = 2.5 / 0.9405

**τ_avg = 2.66 psi**

The calculated average shear stress in each snap protrusion is **2.66 psi**.


## Free Body Diagrams

### Flexure Component FBD

For the flexure FBD, one flexible arm is modeled as a cantilever beam fixed at the bottom. A transverse load of **0.25 lbf** acts at the free end of the arm. The flexure length is **5.00 in**.

**ADD FLEXURE FBD IMAGE HERE**

### Axial / Snap-Fit FBD

For the axial FBD, the total axial load is **5 lbf**. Because the design contains two snap features, the load is assumed to divide equally between them, giving **2.5 lbf per snap feature**.

**ADD AXIAL FBD IMAGE HERE**


# Parametric Design

## Parameters

I designed the components parametrically in Creo using dimensions and constraints so that important dimensions could be changed without completely rebuilding the models.

The main design parameters were:

| Parameter | Value | Purpose |
|---|---:|---|
| Flexure Length | 5.00 in | Controls the length of each flexible arm |
| Flexure Width | 0.50 in | Controls arm stiffness and bending stress |
| Part Thickness | 0.95 in | Controls the cross-section of the keychain |
| Snap Protrusion | 0.60 in | Creates the locking feature |
| Hook Dimension | 0.99 in | Controls the snap feature geometry |
| Slot Length | 5.00 in | Creates the flexible arm region |
| Slot Width | 1.10 in | Provides room for the arms to flex |
| Large Chamfer | 0.50 in | Guides the snap into the base |
| Small Chamfer | 0.11 in | Removes sharp edges |
| Keychain Loop Radius | 0.50 in | Rounds the key attachment feature |
| Base Depth | 2.00 in | Controls overall base thickness |
| Base Cavity Depth | 1.50 in | Provides space for the keychain |

### Why I Chose These Parameters

I chose the flexure length, width, and thickness because these dimensions directly affect how much the arms bend and the stress produced during bending.

The snap protrusion and chamfer dimensions control how the keychain engages with the base. The cavity and slot dimensions control the fit and provide enough space for the flexible arms to move.

### Parameter Changes

The values changed throughout the CAD process as I reviewed how the two components would interact. I adjusted the snap-fit geometry to provide more room for the arms to flex inward, added chamfers to make insertion smoother, and added rounded ends to the slots to reduce sharp stress concentrations.

I also removed the unnecessary center section of the final keychain. The dimensions of the two flexible arms remained unchanged, so the arm dimensions used in the engineering calculations remained the same.


## CAD Design Process

I created both components parametrically in Creo. I designed the base first and then created the keychain insert to fit inside the base and use two flexible arms as the snap-fit mechanism.

### Step 1 - Create the Base

I started by sketching a rectangle and extruding it **2.00 in** to create the main body of the base.

<img width="960" height="600" alt="Base Extrusion" src="https://github.com/user-attachments/assets/b95bbc9d-e179-4e6c-bedd-097398c2a21d" />

### Step 2 - Create the Inside Opening

Next, I sketched the area that I wanted to remove from the base. I dimensioned the opening and used **Delete Segment** to make the sketch one continuous shape.

<img width="960" height="600" alt="Base Opening Sketch" src="https://github.com/user-attachments/assets/1038af79-adfc-4b07-889b-785819cb6ee8" />

<img width="960" height="600" alt="Base Opening Dimensions" src="https://github.com/user-attachments/assets/e42dd664-e0c9-4666-b301-6c748a66398c" />

I then used **Remove Material** to cut **1.50 in** into the base and create the cavity where the keychain will fit.

<img width="960" height="600" alt="Base Cavity" src="https://github.com/user-attachments/assets/c165d967-c7b2-4b55-9167-f6ac9e56cf36" />

### Step 3 - Finish the Base Shape

I added another extrusion to close the part and finish the main shape of the base.

<img width="960" height="600" alt="Finished Base Shape" src="https://github.com/user-attachments/assets/8490e170-6bb2-4eaf-979f-d217443487eb" />


## Keychain Design

### Step 4 - Create the Keychain Body

I started the keychain with an extruded rectangle. I used a depth of **0.95 in**, making the keychain thinner than the inside depth of the base so that it can fit inside.

<img width="960" height="600" alt="Keychain Body" src="https://github.com/user-attachments/assets/14dff1c0-e5c8-4fda-a7c7-7b092c5b0148" />

### Step 5 - Create the Flexible Arms

I sketched and removed material to create the flexible sections of the keychain. These outside sections became the two flexible arms used for the snap-fit.

<img width="960" height="600" alt="Flexible Arm Sketch" src="https://github.com/user-attachments/assets/40a1d210-502f-4793-adf9-5e1a975205af" />

I dimensioned and constrained the flexible sections so that the two arms would remain the same size.

<img width="960" height="600" alt="Flexible Arm Dimensions" src="https://github.com/user-attachments/assets/1cef699d-88e1-48fa-a6c2-c7913676d95b" />

### Step 6 - Add the Snap-Fit Features

I added an extrusion to the end of each flexible arm to create the snap-fit features. I made these features extend past the outside of the base so they can be pushed inward by hand when the keychain needs to be removed.

<img width="960" height="600" alt="Snap Features" src="https://github.com/user-attachments/assets/9411e9b0-1393-4ae1-b60f-48e75b27eba9" />

<img width="960" height="600" alt="Snap Feature Dimensions" src="https://github.com/user-attachments/assets/c475e01d-9061-44d8-aa1d-3064d16a3f4d" />

### Step 7 - Add Chamfers

I added **0.50 in chamfers** to the snap features. The angled surfaces help guide the arms inward as the keychain is inserted into the base.

<img width="960" height="600" alt="Large Chamfers" src="https://github.com/user-attachments/assets/ac6866c7-4dd7-4da1-9eb1-aa58aa28de9b" />

After reviewing the design, I made adjustments so that the flexible arms had enough room to move inward.

<img width="960" height="600" alt="Snap Adjustment" src="https://github.com/user-attachments/assets/6459b932-d634-48e9-b2c0-911f282f5a2b" />

I then added smaller **0.11 in chamfers** to the other edges to remove sharp edges and make the snap-fit smoother.

<img width="960" height="600" alt="Small Chamfers" src="https://github.com/user-attachments/assets/829cd8e4-8c76-45aa-a0d8-eda289de36cf" />

### Step 8 - Reduce Stress Concentrations

I added circular ends to the flexure slots instead of leaving sharp inside corners. This creates a smoother transition at the end of each slot and helps reduce stress concentration when the arms bend.

<img width="960" height="600" alt="Rounded Flexure Ends" src="https://github.com/user-attachments/assets/b2030d59-0110-498f-a0d2-c2e89a5fc739" />

### Step 9 - Add the Keychain Loop

I added a loop to the bottom of the keychain so that a set of keys can be attached to the part.

<img width="960" height="600" alt="Keychain Loop" src="https://github.com/user-attachments/assets/1e2f46a3-8ffc-4090-866b-7742df7647ee" />

I then rounded the loop with a **0.50 in radius** to remove the sharp edges and create a smoother final shape.

<img width="960" height="600" alt="Rounded Keychain Loop" src="https://github.com/user-attachments/assets/14a0789f-179b-43b5-b687-e980b280b795" />


## Final Base Features

### Step 10 - Personalize the Base

I went back to the base and added an extruded **K** for my name.

<img width="960" height="600" alt="Personalized Base" src="https://github.com/user-attachments/assets/e26e7e35-1ea2-4086-9f31-564f2a679a48" />

### Step 11 - Add Wall Mounts

Finally, I added two loops to the top of the base so that it can be mounted to a wall. The holes provide locations for nails or screws to hold the base in place.

<img width="960" height="600" alt="Wall Mounts" src="https://github.com/user-attachments/assets/6e6820e0-658c-4418-9b32-926208f7ed5b" />


## Final CAD Designs

After completing the design process and making the necessary adjustments, I finalized both components of the snap-fit keychain system. The final design consists of a wall-mounted base and a removable keychain insert.

### Final Base

The final base contains the internal opening and retaining features for the snap-fit mechanism. I added a **K** to personalize the design and two mounting loops at the top so the base can be attached to a wall.

<img width="960" height="600" alt="Final Base" src="https://github.com/user-attachments/assets/ff76e60e-5f8b-4a03-afa7-ca69881ee880" />

### Final Keychain

After reviewing the completed design, I decided that the solid center section of the keychain was unnecessary. I removed this material to simplify the design and reduce the amount of filament required.

The final keychain uses two flexible cantilever arms connected at the bottom. Each arm contains a snap protrusion that engages with the base. The rounded ends of the opening reduce sharp stress concentrations and allow the arms to flex inward during insertion and removal.

Removing the center section did not change the dimensions of the flexible arms used in my engineering calculations.

<img width="960" height="600" alt="Final Keychain" src="https://github.com/user-attachments/assets/3b1a7ec8-70bd-4da7-b581-3a4cd5c7903d" />


# 3D Printing and Testing

## Build Orientation Research

FDM parts do not have the same strength in every direction because they are manufactured one layer at a time. Research on FDM-printed PLA found that build orientation affects the mechanical properties of the finished part, with flat and on-edge specimens generally performing better than upright specimens for strength and stiffness.

Because the snap-fit arms need to bend during insertion and removal, I printed the keychain flat. This keeps the bending primarily within the printed layers instead of depending on the weaker bonds between layers. Therefore, my chosen orientation is consistent with the research for a component subjected to bending.

**Source:**  
[Chacón et al. - Additive Manufacturing of PLA Structures Using Fused Deposition Modelling](https://www.sciencedirect.com/science/article/pii/S0264127517303143)


## Build Orientation and Preprocessing

I positioned both components flat on the build plate. The keychain was printed flat so that the flexible snap-fit arms were formed within the print layers. The base was also positioned flat to provide a stable surface on the build plate.

I arranged both components on the same build plate so they could be produced during the same print.

### Supports

The assignment required one component to use support material. The base contains overhanging features, so I used **paint-on support enforcers** only in the areas where support was necessary.

I chose paint-on supports because they gave me control over exactly where the support material was generated. This reduced unnecessary material, print time, and cleanup.

The keychain did not require supports.

<img width="960" height="600" alt="Paint-On Supports" src="https://github.com/user-attachments/assets/02810fac-f780-4ec9-9c78-d3122153f6cb" />

### Print Settings

- **Printer:** Prusa CORE One
- **Nozzle:** 0.4 mm
- **Material:** PLA
- **Layer Height:** 0.20 mm
- **Infill:** 20%
- **Supports:** Paint-on support enforcers only
- **Estimated Print Time:** 37 minutes

I selected a 0.20 mm layer height as a balance between print quality and print time. I used 20% infill because the parts did not need to be completely solid, while still providing enough internal structure for the functional prototype.

<img width="960" height="600" alt="PrusaSlicer Setup" src="https://github.com/user-attachments/assets/c5ab00b1-bb2b-44a6-aac9-e561822b7a50" />


## Printing and Testing

Both components were printed together using PLA on **Printer #10**. After printing, I removed the support material from the base and added a metal key ring to the keychain.

### Final Print Information

- **Printer:** Printer #10
- **Material:** PLA
- **Layer Height:** 0.20 mm
- **Infill:** 20%
- **Actual Print Time:** 44 min 35 sec
- **Material Used:** 19 g PLA
- **Supports:** Paint-on support enforcers on the base

<p align="center">
  <img width="400" alt="Final Print Information" src="https://github.com/user-attachments/assets/6e04b9f0-8292-40cb-9ee6-2bec3234e64d" />
</p>

### Print Results

Both components printed successfully. The flexible arms and snap features printed without breaking, and the support material was successfully removed from the base.

<p align="center">
  <img width="400" alt="Printed Snap-Fit" src="https://github.com/user-attachments/assets/cc84e60a-90d2-4296-be7f-1118d5114466" />
</p>

### Snap-Fit Test

I tested the assembly by pushing the keychain into the base. The two flexible arms bend inward as the snap features pass through the opening. Once inserted, the arms return outward and hold the keychain inside the base.

The final design successfully snaps into the base and stays in place. The keychain can also be removed by squeezing the flexible arms inward to release the snap features.

<p align="center">
  <img width="350" alt="Printed Components" src="https://github.com/user-attachments/assets/e852a734-d989-4911-824e-d40c37ca99c1" />
  <img width="350" alt="Final Assembly" src="https://github.com/user-attachments/assets/39824390-c788-42e6-90f9-5c692d889cd5" />
</p>


## Design Changes and Iteration

Several changes were made during the design process before printing the final parts.

- I added chamfers to the snap features so they could slide into the base more easily.
- I adjusted the snap-fit geometry to give the flexible arms more room to bend inward.
- I added rounded ends to the flexure openings to reduce sharp corners and stress concentrations.
- I removed the unnecessary center section of the keychain. This reduced material and gave the final design a simpler shape while keeping the two flexible arms.
- I added a rounded key ring loop to make the design functional as an actual keychain.
- I used paint-on supports only where necessary on the base to reduce support material and cleanup.

The first physical print successfully snapped together, so another print iteration was not necessary. The CAD changes made before printing were enough for the two components to function together.


## Lessons Learned

This project helped me better understand how snap-fit designs use elastic deformation to connect two parts. I learned that the dimensions of the flexible arms, chamfers, rounded corners, and print orientation all affect how well a snap-fit mechanism works.

I also learned how to use **paint-on supports in PrusaSlicer**. I struggled with getting the supports where I wanted them at first, but I learned how to use support enforcers to place support only where it was needed instead of supporting the entire part. This helped reduce unnecessary material and cleanup.

Another thing I learned was the importance of reducing sharp corners around a flexure. Adding rounded ends to the slots created a smoother transition where the arms bend. I also learned that small geometry changes, such as adding chamfers and providing enough room for the arms to move inward, can make a large difference in whether a snap-fit can be inserted and removed successfully.

Overall, this project helped me better understand how engineering calculations, parametric CAD, material properties, and 3D printing settings work together to create a functional design.


## Resources

1. **UltiMaker - PLA Technical Data Sheet**  
   Used to research the mechanical properties of PLA, including Young's modulus and yield strength.  
   https://um-support-files.ultimaker.com/materials/2.85mm/tds/PLA/Ultimaker-PLA-TDS-v5.00.pdf

2. **Chacón et al. - Additive Manufacturing of PLA Structures Using Fused Deposition Modelling**  
   Used to research how FDM build orientation affects the mechanical properties of printed PLA parts.  
   https://www.sciencedirect.com/science/article/pii/S0264127517303143

3. **PrusaSlicer**  
   Used to prepare the models for printing, select the build orientation, apply paint-on supports, and determine the print settings.


## Time Spent

- Research and planning: **30 minutes**
- Engineering calculations: **1 hour**
- CAD modeling: **2 hours**
- PrusaSlicer setup and supports: **30 minutes**
- Printing and testing: **45 minutes**
- Portfolio documentation: **1 hour**

**Total Time: 5 hours 45 minutes**
