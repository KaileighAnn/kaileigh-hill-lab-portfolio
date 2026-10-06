# Lab – 3D Printed Mechanism

## Research

Before designing my mechanism, I researched recent linkage and mechanism designs to better understand how motion can be transferred through mechanical components.

### Compliant Four-Bar Robotic Finger – 2021

A compliant four-bar linkage for a robotic finger was patented in 2021. The mechanism replaces some of the traditional rigid links and pin joints of a four-bar linkage with flexible compliant sections. When an input is applied, the links and compliant joints work together to produce a finger-like bending motion.

This type of mechanism could be used in the **medical industry** for prosthetic hands and in the **robotics/manufacturing industry** for robotic grippers that need to handle objects.

<img width="201" height="120" alt="image" src="https://github.com/user-attachments/assets/901c6242-3e18-48d5-9a18-b6a4fa557c20" />

### Robotic Finger Linkage – 2023

A robotic finger linkage published in 2023 uses a four-bar mechanism along with an actuator and elastic member. The connected links rotate relative to one another to create flexion and extension similar to the movement of a finger. The mechanism can also allow passive movement when an external force is applied.

This mechanism could be used in the **medical industry** for prosthetic or rehabilitation devices and in the **automation industry** for robotic hands and gripping systems.

<img width="178" height="120" alt="image" src="https://github.com/user-attachments/assets/324b3db7-182e-47f6-a891-66c6e9729898" />

### Additional Research – Compliant Mechanisms

A 2024 study investigated a compliant mechanism for an automotive side-door latch. The mechanism uses elastic deformation and controlled motion to operate the latch and provide an electrically powered release function. This demonstrates how mechanisms can be designed to perform repetitive motion while reducing the number of traditional moving joints.

Compliant mechanisms like this could be used in the **automotive industry** for door and locking systems and in the **consumer-product industry** for compact latches, closures, and release mechanisms.

### Sources

1. U.S. Patent 11,185,427, *Compliant Four-Bar Linkage Mechanism for a Robotic Finger*, 2021.
2. U.S. Patent Application US20230415355A1, *Linkage Mechanism, Robotic Finger and Robot*, 2023.
3. Wang, M., Hang, L., Zhong, C., and Qin, P., *Research on a Novel Compliant Mechanism Applied in the Vehicle Side Door Latch and Stability Analysis via Lyapunov Exponents*, Journal of Mechanical Engineering Science, 2024.

---

## Design

### Purpose

For this project, I designed a functional 3D-printed hair claw clip mechanism. The clip converts squeezing motion at the handles into rotational motion that opens the gripping jaws. When the handles are released, a torsion spring returns the jaws to the closed position.

I chose a hair claw because it is a simple mechanism that performs a useful everyday task. I also wanted to create something that was functional and unique while remaining simple enough to CAD and 3D print.

### Initial Design

I used an existing hair claw clip as a reference to understand how the pivot, spring, handles, and teeth work together. Instead of copying the original design, I created my own geometry and incorporated a daisy theme to make the final product unique.

I reused the torsion spring from an existing claw clip. Initial measurements of the spring were:

| Feature | Measurement |
| --- | ---: |
| Inside Diameter | 1.7 mm |
| Coil Length | 10.0 mm |
| Number of Coils | 9 |

The clip was designed around this spring so that the existing hardware could be reused in the final assembly.

**Figure 1. Original claw clip used as a reference.**

<p align="center">
  <img src="https://github.com/user-attachments/assets/9bd6e99e-8525-426f-b5cf-10eda9728a2b" width="300">
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/553b4024-be3b-49d8-a345-51b6e6d732c1" width="300">
</p>

### Components

| Component | Function | Type |
| --- | --- | --- |
| Claw Half 1 | Forms one side of the clip and gripping teeth | 3D Printed |
| Claw Half 2 | Forms the opposite side and gripping teeth | 3D Printed |
| Torsion Spring | Supplies force to return the clip to its closed position | Reused/Purchased |
| Pivot Pin | Connects the two halves and provides the axis of rotation | Reused/Purchased |

### CAD Development

The claw clip was modeled in Creo Parametric. I started with the basic shape of the clip and then added each functional feature separately. This allowed the body, teeth, hinge, and pivot features to be adjusted independently throughout the design process.

**Figure 1. Initial Claw Profile**

The initial profile of the claw was created using arcs and straight sections to form the curved body. An opening was included in the center to reduce material while maintaining the overall shape of the clip.

<img width="960" height="600" alt="l73" src="https://github.com/user-attachments/assets/79254cec-6c67-468d-a017-090a860ac160" />

**Figure 2. Initial Body Extrusion**

The completed profile was extruded to create the main body of the first claw half. This established the basic thickness and overall shape that the remaining features were built onto.

<img width="960" height="600" alt="l74" src="https://github.com/user-attachments/assets/2bdca251-1708-4396-b528-8c806983fd66" />

**Figure 3. Side Profile Development**

A second sketch was created to define the curved side profile of the claw. This shape was used to create the curvature needed for the clip to wrap around and hold hair.

<img width="960" height="600" alt="l76" src="https://github.com/user-attachments/assets/32fc3920-9e70-46b5-ba48-7d0965170311" />

**Figure 4. Curved Claw Geometry**

The side-profile geometry was added to the original body to create the three-dimensional curved shape of the claw.

<img width="960" height="600" alt="l77" src="https://github.com/user-attachments/assets/98d84247-1ff4-43de-9c9d-9993a1d8238e" />

**Figure 5. First Tooth**

The first gripping tooth was created at the lower edge of the claw. The tooth was extended from the curved body so that it could reach toward the opposite half when the clip was closed.

<img width="960" height="600" alt="l78" src="https://github.com/user-attachments/assets/98ee6f52-1d7f-461a-a932-0658e7e7a3e0" />

**Figure 6. Tooth Pattern**

The first tooth was patterned across the claw to create six evenly spaced gripping teeth. Using a pattern kept the teeth consistent and made the design easier to modify.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/309b2725-b864-48a9-a2ef-783e23e431fe" />

**Figure 7. Rounded Tooth Ends**

The ends of the teeth were rounded using the Round feature. A 3 mm radius was used to remove the sharp edges and create smoother contact surfaces.

<img width="960" height="600" alt="l79" src="https://github.com/user-attachments/assets/5f881940-10bd-44f0-ac6a-cfcb5d46f30c" />

**Figure 8. Hinge Tab Sketch**

The hinge geometry was created near the top of the claw. The tab was designed with a rounded end and a hole through its center for the pivot pin.

<img width="960" height="600" alt="l710" src="https://github.com/user-attachments/assets/1ce01236-b23d-4d9c-bf06-d44d81fca7f4" />

**Figure 9. First Hinge Tab**

The hinge-tab sketch was extruded from the claw body. This feature provides one of the supporting surfaces for the pivot connection between the two claw halves.

<img width="960" height="600" alt="l711" src="https://github.com/user-attachments/assets/d440e5c7-183b-4e10-87cd-923db457068e" />

**Figure 10. Pivot Hole**

A hole was created through the hinge tab for the pivot pin. The pin passes through the hinge features of both claw halves and creates the axis about which the mechanism rotates.

<img width="960" height="600" alt="l712" src="https://github.com/user-attachments/assets/7a442ff3-ec00-4bf9-b6fe-5129373dc57d" />

**Figure 11. Second Claw Half**

The second claw half was modeled separately so its hinge features could interlock with those of the first half. The two halves use the same general claw geometry but have different hinge-tab locations.

<img width="960" height="600" alt="l713" src="https://github.com/user-attachments/assets/d16a5711-a640-482b-8261-82ab86ca286e" />

**Figure 14. Sliced Components**

The two claw halves and pivot pin were exported as STL files and imported into PrusaSlicer. Supports were generated underneath the required overhanging regions. I also used **elephant foot compensation** to reduce the expansion of the first layer and improve the fit and dimensional accuracy of the printed parts. The complete print was estimated to take approximately **2 hours and 8 minutes** and use approximately **46.89 g of filament**.

<img width="960" height="600" alt="l714" src="https://github.com/user-attachments/assets/a877d634-523b-40e6-b1a1-c7d2998eda33" />

### Tolerances

The primary moving interface is the pivot pin rotating inside the hinge holes. FDM printed holes commonly print slightly undersized, so clearance must be included to prevent the joint from binding.

A starting clearance of approximately **0.2–0.3 mm per side** was considered based on the recommended FDM clearance discussed in class. The final pivot-hole dimension was selected based on the diameter of the reused pin and verified through printing and assembly.

The fit was designed to allow the claw halves to rotate freely without creating excessive looseness.

### Design Decisions

**1. Reused spring vs. printed spring**

I considered creating a flexible printed spring or reusing the torsion spring from an existing claw clip. I chose the existing metal torsion spring because it already provided the required closing force and would be more reliable than a small FDM-printed spring.

**2. Thin teeth vs. thicker teeth**

I considered using many thin teeth similar to the original clip or fewer, thicker teeth. I chose thicker teeth because they are easier to print and less likely to break while still providing enough gripping points for the clip.

**3. Standard body vs. decorative body**

A plain rectangular claw would have been the simplest option, but it would not make the design very unique. I chose to incorporate a daisy theme while keeping the basic mechanical geometry simple. This allowed the final design to be more personalized without significantly increasing print difficulty.

---

## 3D Print

### Purpose

The purpose of the print was to manufacture the two functional claw halves and verify that the printed mechanism could rotate, open, close, and grip using the reused torsion spring.

### Components

The two claw halves were printed separately. The torsion spring and pivot pin were then installed after printing to create the completed mechanism.

### Printing

The parts were oriented to reduce unnecessary support material while maintaining the strength of the teeth and hinge features.

<p align="center">
  <video autoplay muted loop playsinline width="500">
    <source src="/kaileigh-hill-lab-portfolio/Labs/L07/claw-clip-demo.mp4" type="video/mp4">
  </video>
</p>

**Completed printed components.**

*Insert print photo.*

After printing, the parts were removed from the build plate and any support material was removed. The pivot holes and mating surfaces were checked before assembly.

### Assembly

The two printed claw halves were aligned at the hinge. The torsion spring was positioned between the halves and the metal pivot pin was inserted through the hinge and spring.

**Figure 10. Final assembled claw clip.**

*Insert final photo.*

The handles were then squeezed to verify that the jaws opened freely and that the torsion spring returned the clip to its closed position.

---

## Lessons Learned

### Time

I spent approximately **5 hours total** on this project. About **30 minutes** were spent researching, **2 hours** creating and adjusting the CAD models, **30 minutes** preparing the parts in PrusaSlicer, and about **2 hours** printing and working on assembly. The CAD portion took the most time because I had to make sure the two claw halves and hinge features would fit together correctly.

### Biggest Mistake

My biggest mistake was not watching the printer closely when I first started the print. The filament was not coming out correctly, and I did not notice until about **30 minutes into the print**. I had to stop the print, fix the filament issue, and restart it from the beginning. This taught me to watch the first few layers of a print before leaving the printer.

### Tolerances

The most important tolerance in this design was around the hinge and pivot pin because the two claw halves needed to rotate freely without being too loose. I included clearance between the moving components to account for the accuracy of FDM printing. The project showed me that even small changes in clearance can make a large difference in how well a printed mechanism fits and moves.
