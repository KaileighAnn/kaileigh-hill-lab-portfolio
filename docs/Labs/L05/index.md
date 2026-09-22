# Lab #5 Design a Snap Fit

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

## CAD Design Process

I created both components parametrically in Creo. I designed the base first and then created the keychain insert to fit inside the base and use two flexible arms as the snap-fit mechanism.

### Step 1 - Create the Base

I started by sketching a rectangle and extruding it **2.00 in** to create the main body of the base.

<img width="960" height="600" alt="l41" src="https://github.com/user-attachments/assets/b95bbc9d-e179-4e6c-bedd-097398c2a21d" />


### Step 2 - Create the Inside Opening

Next, I sketched the area that I wanted to remove from the base. I dimensioned the opening and used **Delete Segment** to make the sketch one continuous shape.

<img width="960" height="600" alt="l42" src="https://github.com/user-attachments/assets/1038af79-adfc-4b07-889b-785819cb6ee8" />

<img width="960" height="600" alt="l44" src="https://github.com/user-attachments/assets/e42dd664-e0c9-4666-b301-6c748a66398c" />

I then used **Remove Material** to cut **1.50 in** into the base and create the cavity where the keychain will fit.

<img width="960" height="600" alt="l43" src="https://github.com/user-attachments/assets/c165d967-c7b2-4b55-9167-f6ac9e56cf36" />

### Step 3 - Finish the Base Shape

I added another extrusion to close the part and finish the main shape of the base.

<img width="960" height="600" alt="l45" src="https://github.com/user-attachments/assets/8490e170-6bb2-4eaf-979f-d217443487eb" />


## Keychain Design

### Step 4 - Create the Keychain Body

I started the keychain with an extruded rectangle. I used a depth of **0.95 in**, making the keychain thinner than the inside depth of the base so that it can fit inside.

<img width="960" height="600" alt="l46" src="https://github.com/user-attachments/assets/14dff1c0-e5c8-4fda-a7c7-7b092c5b0148" />

### Step 5 - Create the Flexible Arms

I sketched and removed material from both sides of the keychain to separate the outside sections from the center body. These sections become the flexible arms used for the snap-fit.

<img width="960" height="600" alt="l47" src="https://github.com/user-attachments/assets/40a1d210-502f-4793-adf9-5e1a975205af" />

I dimensioned the flexible sections so that the arms would be the same size on both sides.

<img width="960" height="600" alt="l48" src="https://github.com/user-attachments/assets/1cef699d-88e1-48fa-a6c2-c7913676d95b" />

### Step 6 - Add the Snap-Fit Features

I added an extrusion to the end of each flexible arm to create the snap-fit features. I made these features extend past the outside of the base so they can be pushed inward by hand when the keychain needs to be removed.

<img width="960" height="600" alt="l49" src="https://github.com/user-attachments/assets/9411e9b0-1393-4ae1-b60f-48e75b27eba9" />

<img width="960" height="600" alt="l410" src="https://github.com/user-attachments/assets/c475e01d-9061-44d8-aa1d-3064d16a3f4d" />

### Step 7 - Add Chamfers

I added **0.50 in chamfers** to the snap features. The angled surfaces help guide the arms inward as the keychain is inserted into the base.

<img width="960" height="600" alt="l411" src="https://github.com/user-attachments/assets/ac6866c7-4dd7-4da1-9eb1-aa58aa28de9b" />

After reviewing the design, I made adjustments so that the flexible arms had enough room to move inward.

<img width="960" height="600" alt="l413" src="https://github.com/user-attachments/assets/6459b932-d634-48e9-b2c0-911f282f5a2b" />

I then added smaller **0.11 in chamfers** to the other edges to remove sharp edges and make the snap-fit smoother.

<img width="960" height="600" alt="l414" src="https://github.com/user-attachments/assets/829cd8e4-8c76-45aa-a0d8-eda289de36cf" />

### Step 8 - Reduce Stress Concentrations

I added circular ends to the flexure slots instead of leaving sharp inside corners. This creates a smoother transition at the end of each slot and helps reduce stress concentration when the arms bend.

<img width="960" height="600" alt="l415" src="https://github.com/user-attachments/assets/b2030d59-0110-498f-a0d2-c2e89a5fc739" />

### Step 9 - Add the Keychain Loop

I added a loop to the bottom of the keychain so that a set of keys can be attached to the part.

<img width="960" height="600" alt="l416" src="https://github.com/user-attachments/assets/1e2f46a3-8ffc-4090-866b-7742df7647ee" />

I then rounded the loop with a **0.50 in radius** to remove the sharp edges and create a smoother final shape.

<img width="960" height="600" alt="l417" src="https://github.com/user-attachments/assets/14a0789f-179b-43b5-b687-e980b280b795" />


## Final Base Features

### Step 10 - Personalize the Base

I went back to the base and added an extruded **K** for my name.

<img width="960" height="600" alt="l418" src="https://github.com/user-attachments/assets/e26e7e35-1ea2-4086-9f31-564f2a679a48" />

### Step 11 - Add Wall Mounts

Finally, I added two loops to the top of the base so that it can be mounted to a wall. The holes provide locations for nails or screws to hold the base in place.

<img width="960" height="600" alt="l419" src="https://github.com/user-attachments/assets/6e6820e0-658c-4418-9b32-926208f7ed5b" />

## Final CAD Designs

After completing the design process and making the necessary adjustments, I finalized both components of the snap-fit keychain system. The final design consists of a wall-mounted base and a removable keychain insert.

### Final Base

The final base contains the internal opening and retaining features for the snap-fit mechanism. I added a **K** to personalize the design and two mounting loops at the top so the base can be attached to a wall.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/ff76e60e-5f8b-4a03-afa7-ca69881ee880" />

### Final Keychain

After reviewing the completed design, I decided that the solid center section of the keychain was unnecessary. I removed this material to simplify the design and reduce the amount of filament required.

The final keychain uses two flexible cantilever arms connected at the bottom. Each arm contains a snap protrusion that engages with the base. The rounded ends of the opening reduce sharp stress concentrations and allow the arms to flex inward during insertion and removal.

Removing the center section did not change the dimensions of the flexible arms used in my engineering calculations.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/3b1a7ec8-70bd-4da7-b581-3a4cd5c7903d" />

## Engineering Analysis

The flexible arms of the keychain were analyzed as cantilever beams. When the keychain is inserted into the base, the snap features contact the sides of the base and cause the arms to bend inward. Once the snap features pass the retaining edge, the arms return toward their original position and lock the keychain into place.

For the calculations, PLA was used as the material and a safety factor of **3.5** was applied.

### Design Values

- Material: PLA
- Safety Factor: 3.5
- Flexible arm length: 5.00 in
- Flexible arm width: 0.50 in
- Part thickness: 0.95 in
- Snap protrusion: 0.60 in
- Transverse load: 0.25 lbf
- Axial load: 5 lbf

### Cantilever Beam Deflection

The snap-fit arms must flex inward during insertion. I modeled each flexible arm as a cantilever beam with a concentrated load applied near the free end.

The cantilever beam deflection equation is:

δ = FL³ / 3EI

where:

- δ = deflection
- F = transverse force
- L = flexible arm length
- E = Young's modulus of PLA
- I = area moment of inertia

### Area Moment of Inertia

For the rectangular cross-section of one flexible arm:

I = bh³ / 12

Using:

b = 0.95 in  
h = 0.50 in

I = (0.95)(0.50)³ / 12

I = 0.00990 in⁴

### Cantilever Beam Deflection

The deflection of one flexible arm was calculated using:

δ = FL³ / 3EI

Using:

F = 0.25 lbf  
L = 5.00 in  
E = 435,000 psi  
I = 0.00990 in⁴

δ = (0.25)(5.00)³ / [3(435,000)(0.00990)]

δ = 0.00242 in

Therefore, the calculated deflection of one snap-fit arm is:

**δ = 0.00242 in**

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

M = (0.25)(5.00) = 1.25 lbf·in

c = 0.50 / 2 = 0.25 in

σ = (1.25)(0.25) / 0.00990

σ = 31.6 psi

### Allowable Stress

Using a PLA yield strength of **7,615 psi** and the required safety factor of **3.5**:

σ_allow = σ_y / SF

σ_allow = 7,615 / 3.5

σ_allow = 2,176 psi

The calculated bending stress was:

σ_b = 31.6 psi

Since:

31.6 psi < 2,176 psi

the calculated bending stress is below the allowable stress for PLA.

**Result: PASS**

### Axial Stress

The snap-fit must support an axial load of **5 lbf**. Since the design has two flexible arms, I assumed the load is divided equally between them.

F_arm = 5 / 2

F_arm = 2.5 lbf

The cross-sectional area of one arm is:

A = bh

A = (0.95)(0.50)

A = 0.475 in²

The axial stress is:

σ_axial = F / A

σ_axial = 2.5 / 0.475

σ_axial = 5.26 psi

Since:

5.26 psi < 2,176 psi

the calculated axial stress is below the allowable stress for PLA.

**Result: PASS**

### Average Shear Stress

The snap protrusions hold the keychain inside the base. Since there are two snap features, I assumed the 5 lbf axial load is divided equally between them.

F_hook = 5 / 2

F_hook = 2.5 lbf

Using the snap protrusion dimensions:

A_shear = (0.95)(0.99)

A_shear = 0.9405 in²

The average shear stress is:

τ_avg = F / A

τ_avg = 2.5 / 0.9405

τ_avg = 2.66 psi

The calculated average shear stress in each snap protrusion is:

**τ_avg = 2.66 psi**

### Supports

I used paint-on support enforcers on the base so that support material was only added where it was necessary. I wanted to minimize the amount of support material to reduce waste, print time, and cleanup.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/02810fac-f780-4ec9-9c78-d3122153f6cb" />

The keychain was oriented flat on the build plate and did not require supports. The base required a small amount of support for its overhanging features.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/c5ab00b1-bb2b-44a6-aac9-e561822b7a50" />


- Material: PLA
- Infill: 20%
- Layer height: 0.20 mm
- Printer: Prusa CORE One
- Nozzle: 0.4 mm
- Supports: Paint-on support enforcers only
- Estimated total print time: 37 minutes
