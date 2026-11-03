# L10 - SLA Printing Lab: Twist-Up Lipstick Container

## Objective

The objective of this lab is to design and manufacture a functional assembly using stereolithography (SLA) 3D printing while demonstrating an RC2 sliding fit based on the *Machinery's Handbook*. The project also focuses on dimensional accuracy, resin shrinkage, and evaluating the fit of printed components.

For my project, I chose to create a miniature twist-up lipstick container with a removable cap and fake lipstick.

## Design Concept

I wanted to create something that was both functional and cute, so I decided to design a twist-up lipstick container.

The design uses a rotating base and spiral sleeve to raise and lower the lipstick holder. As the base rotates, a guide pin follows the spiral slot, converting rotational motion into vertical movement.

The assembly Originally consists of six components: an outer tube, rotating base, spiral sleeve, lipstick holder, fake lipstick, and removable cap. Each component was modeled separately in SolidWorks before being assembled.

After considering print time and material usage, I decided to simplify my design to just three parts. I removed the cap since it was not necessary for this project, combined the lipstick holder with the modeled lipstick, and combined the rotating base with the spiral sleeve since they need to rotate together. These changes helped reduce material usage and print time while keeping the twist-up mechanism functional.

## RC2 Sliding Fit Research and SLA Shrinkage

### Machinery's Handbook Reference

I researched the RC2 sliding fit using the *Machinery's Handbook*, page 654, Table 8a, which references ANSI/ASME B4.1.

RC2 fits are intended for accurate positioning while allowing components to slide or turn easily with a small amount of clearance.

<img width="1536" height="1152" alt="image" src="https://github.com/user-attachments/assets/00be712b-5ce7-4031-97aa-7e0c1a45f878" />

*Figure 1: Machinery's Handbook, page 654, Table 8a, showing the RC2 sliding fit specifications.*

### Selected Sliding Interface

For my design, I selected the connection between the guide pin on the lipstick holder and the spiral slot on the spiral sleeve.

The guide pin follows the spiral slot as the base rotates, allowing the lipstick holder to move vertically.

Since RC2 specifications are intended for cylindrical hole-and-shaft fits, I am using the clearance principles as a reference for my pin-and-slot mechanism.


### RC2 Sliding Fit Clearance Calculation

Using the *Machinery's Handbook*, page 654, Table 8a, I researched the RC2 sliding fit requirements for my guide pin and spiral slot.

For the selected nominal size range of 0–0.12 inches (0–3.048 mm), the RC2 clearance limits are:

| Specification | Clearance |
|---|---|
| Minimum RC2 Clearance | 0.00254 mm |
| Maximum RC2 Clearance | 0.01397 mm |

Since my design uses a guide pin and spiral slot rather than a traditional hole and shaft, I used these limits as a reference for my sliding mechanism.

### Initial CAD Clearance

The original SolidWorks dimensions were:

| Feature | Dimension |
|---|---|
| Spiral Slot Width | 2.060 mm |
| Guide Pin Width | 2.040 mm |
| Designed Clearance | 0.020 mm |

**Clearance = Slot Width - Guide Pin Width**

Clearance = 2.060 - 2.040

**Original Clearance = 0.020 mm**

After scaling the model to 80% for SLA printing:

| Feature | Scaled Dimension |
|---|---|
| Spiral Slot Width | 1.648 mm |
| Guide Pin Width | 1.632 mm |
| Designed Clearance | 0.016 mm |

**Scaled Clearance = 1.648 - 1.632 = 0.016 mm**

The scaled clearance was slightly larger than the maximum RC2 clearance of 0.01397 mm.

### RC2 Design Evaluation

To better match the RC2 specification, a theoretical target clearance of 0.010 mm could be used.

With a guide pin width of 1.632 mm:

**Target Slot Width = 1.632 + 0.010 = 1.642 mm**

This would provide a nominal clearance within the RC2 range.

However, my final printed design used the original scaled dimensions. The actual clearance was measured after printing and curing to evaluate how closely the manufactured parts matched the intended fit.


### SLA Resin Shrinkage

For my final print, I used Formlabs Grey Resin with a layer height of 0.050 mm. After printing, I removed the supports, cleaned and washed the parts, and then UV cured them.

According to Formlabs, additional shrinkage can occur during post-curing as the resin continues to harden. This is important for my design because the guide pin and spiral slot have very small clearances, meaning even slight dimensional changes could affect the fit.

To evaluate dimensional accuracy, I compared my final measurements to the theoretical CAD dimensions after scaling the model to 80%.

| Feature | Scaled CAD | Measured | Difference |
|---|---|---|---|
| Spiral Slot Width | 1.648 mm | 1.71 mm | +0.062 mm |
| Guide Pin Width | 1.632 mm | 1.68 mm | +0.048 mm |
| Clearance | 0.016 mm | 0.030 mm | +0.014 mm |

**Actual Clearance = 1.71 - 1.68 = 0.030 mm**

Both measured features were slightly larger than their theoretical CAD dimensions, resulting in a greater clearance than originally intended.

Although the measured clearance exceeded the RC2 reference range, the guide pin successfully slid through the spiral slot. However, the rotating base did not fit properly, preventing the complete twist-up mechanism from functioning as intended.

These results showed the importance of accounting for dimensional variation when designing small moving parts for SLA printing. Since measurements were only taken after curing, I could not determine how much of the variation was caused specifically by resin shrinkage.

## CAD Design and Modeling

The twist-up lipstick container was designed in SolidWorks as a three-part assembly consisting of the outer body, spiral sleeve, and lipstick holder. Each component was modeled separately and then combined into an assembly to create the twist-up mechanism. The design allows the lipstick holder to move vertically as the spiral sleeve rotates, while the outer body keeps the holder aligned.

### Part 1: Outer Body

The outer body was designed to hold the internal components and guide the vertical movement of the lipstick holder.

I started by creating a cylinder using the Extruded Boss/Base feature with a diameter of 22.00 mm and a height of 50.00 mm.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/e746f10a-6d67-4bf8-8133-fbe3495b27b1" />

*Figure 2: Initial cylinder created using the Extruded Boss/Base feature.*

Next, I used the Shell feature with a wall thickness of 2.00 mm to hollow out the cylinder and create space for the internal components.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/9ec004ab-fc56-4e34-8eed-f0a82745da17" />

*Figure 3: Shell feature used to hollow out the outer body.*

I originally added a 6.40 mm diameter hole to the bottom of the body as part of my initial design. However, I later decided this feature was unnecessary and removed it.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/5e08ade5-16d9-4240-987a-a7f48356cfff" />

*Figure 4: Initial hole created at the bottom of the body.*

Next, I created a vertical slot along the inside wall of the body. This slot allows the guide pin on the lipstick holder to move up and down while preventing the holder from rotating with the spiral sleeve.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/a95b9a41-b75b-41b7-b285-d844a50f0475" />

*Figure 5: Vertical guide slot created to control the movement of the lipstick holder.*

I then modified the bottom of the body by removing the original bottom section to better accommodate the internal mechanism.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/5baa5993-3133-4284-93c5-2d9d13632ca2" />

*Figure 6: Bottom of the outer body modified to accommodate the internal components.*

After testing my first prototype using PETG filament, I decided to add a small locking slot beside the vertical guide slot near the bottom. This modification allows the lipstick holder to lock into position when fully lowered, helping prevent unwanted movement.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/2d4b13c7-5c37-4eaa-814f-0794b80816a6" />

*Figure 7: Locking slot added near the bottom of the vertical guide slot after PETG prototype testing.*

### Part 2: Spiral Sleeve

The spiral sleeve was designed to convert rotational movement into vertical movement, allowing the lipstick to extend and retract when the base is turned.

I started by creating a hollow cylinder using the Extruded Boss/Base feature. The cylinder had an outer diameter of 17.50 mm, an inner diameter of 14.00 mm, and a height of 40.00 mm.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/2f7f2c5d-78dc-455a-9af5-7052c0e5a940" />

*Figure 8: Initial hollow cylinder created for the spiral sleeve.*

Next, I used the Helix/Spiral feature to create the path that the lipstick holder's guide pin would follow. The helix was designed to travel along the sleeve and control the vertical movement of the lipstick.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/eb90ec2a-7f2f-4f56-9f55-041e2e92c4f3" />

*Figure 9: Helix/Spiral feature created to define the path of the twist-up mechanism.*

I then created a reference plane at the top of the helix so that I could sketch the profile needed to create the spiral groove.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/0511bb5c-9298-46b3-baae-e337e828365b" />

*Figure 10: Reference plane created at the top of the helix for the sweep profile.*

Using the Swept Cut feature, I removed material along the helix to create the spiral groove. This groove provides the path for the guide pin to follow as the sleeve rotates.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/084a465f-a4fe-46e6-8379-3b1eed374ab9" />

*Figure 11: Swept Cut feature used to create the spiral groove along the sleeve.*

Next, I modified the bottom of the sleeve to prepare it for the rotating base.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/1c3f2801-26be-4d47-a5a6-f4a996488a93" />

*Figure 12: Bottom of the spiral sleeve modified to prepare for the rotating base.*

Finally, I added a circular base with a diameter of 25.00 mm and a height of 10.00 mm. This base provides a surface that can be turned by hand to rotate the spiral sleeve and operate the mechanism.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/c54bf26b-8cc0-4658-af47-42e2c8bc9e28" />

*Figure 13: Final spiral sleeve with the rotating base added to operate the twist-up mechanism.*

### Part 3: Lipstick Holder

The lipstick holder was designed to fit inside the spiral sleeve and move vertically as the base rotates. It also includes a modeled lipstick shape to demonstrate how the mechanism would work.

I started by creating a cylinder with a diameter of 13.50 mm and a height of 15.00 mm using the Extruded Boss/Base feature.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/44f8c608-8a06-4d5c-94fe-af8bc79baea3" />

*Figure 14: Initial cylinder created for the lipstick holder.*

Next, I used the Shell feature with a wall thickness of 1.50 mm to hollow out the cylinder.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/563f427a-d634-4808-a168-ecae156bf707" />

*Figure 15: Shell feature used to hollow out the lipstick holder.*

I then created a guide pin on the side of the holder using the Extruded Boss/Base feature. To position the pin correctly, I referenced the angle of the spiral groove in the sleeve and created a rectangular sketch at the same angle. This helped ensure the pin would align with the spiral path.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/ba727ab6-5511-4adf-b330-acdbd4eec417" />

*Figure 16: Angled guide pin created to align with the spiral groove in the sleeve.*

After creating the pin, I used the Fillet feature to round its edges. This was intended to help the pin slide more smoothly through the spiral groove and reduce interference from sharp corners.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/d0c6483a-53a2-4053-9132-c5410568e2e8" />

*Figure 17: Fillet feature applied to the guide pin to improve sliding movement.*

Next, I extruded a longer cylinder from the inside of the holder to represent the lipstick itself. This allowed the design to demonstrate the extension and retraction of a lipstick.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/5536c730-249a-4000-bad7-52b82a05248b" />

*Figure 18: Additional cylinder extruded from the holder to represent the lipstick.*

I then used the Extruded Cut feature to create an angled tip, similar to the shape of a traditional lipstick.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/bf8a35f6-a7d8-4d77-ada1-274590807fb8" />

*Figure 19: Extruded Cut feature used to create the angled lipstick tip.*

Finally, I applied fillets around the top edges of the lipstick to create a smoother and more realistic appearance.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/09951bfc-defc-4532-a243-54d4c8e07877" />

*Figure 20: Final lipstick holder with the angled tip and rounded edges.*

### Final CAD Assembly

After modeling all three components, I inserted them into a SolidWorks assembly to check how they fit together.

The lipstick holder sits inside the spiral sleeve, with its guide pin passing through the spiral groove and into the vertical guide slot of the outer body. When the circular base is rotated, the spiral groove pushes the pin along its path while the vertical slot prevents the holder from rotating. This causes the lipstick holder to move up or down depending on the direction of rotation.

The assembly was used to check component alignment and identify potential interference before moving on to physical prototyping.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/400c3017-1f9d-4404-b663-bf5e405a2ed2" />

*Figure 21: Final SolidWorks assembly showing the outer body, spiral sleeve, and lipstick holder combined into the twist-up mechanism.*

### Design Modifications

Several modifications were made throughout the design and prototyping process.

- **Bottom Opening:** The original hole and bottom section of the outer body were removed to better accommodate the internal mechanism.
- **Guide Pin:** The pin was positioned to align with the spiral groove and filleted to improve sliding movement.
- **Locking Feature:** A small locking slot was added to the outer body after testing the PETG prototype to help hold the lipstick in its fully lowered position.
- **Print Scaling:** The final SLA assembly was scaled to 0.80 of the original CAD dimensions to meet the printing volume requirements, including supports.

These modifications helped improve the design and prepare the assembly for SLA printing.

## Final Prints and Comparison

### Initial PETG Prototype

Before printing with SLA resin, I printed my design using PETG filament to test the fit and functionality of the twist-up mechanism. I wanted to make sure everything worked before using resin and potentially wasting material.

The PETG prototype worked as intended. The rotating base turned smoothly, allowing the lipstick holder to move up and down inside the outer body.

<img width="1536" height="1152" alt="image" src="https://github.com/user-attachments/assets/a39daa13-c222-4498-8ecb-472b30dd2813" />

*Figure 22: Initial PETG prototype of the twist-up lipstick container.*

![Figure 23](PASTE_PETG_ASSEMBLY_IMAGE_LINK_HERE)

*Figure 23: Assembled PETG prototype used to test the twist-up mechanism.*

### Final SLA Resin Print

After testing the PETG prototype and making the final design modifications, I printed the three components using gray SLA resin with a layer height of 0.050 mm. The model was scaled to 80% of its original size to meet the resin volume requirements, including supports.

After printing, I cleaned, washed, and UV cured the components before testing the final assembly.

<img width="1536" height="1152" alt="image" src="https://github.com/user-attachments/assets/9489679b-d38a-4e16-b565-19c7a688ef2c" />

*Figure 24: Final SLA printed components after post-processing.*

<img width="1152" height="1536" alt="image" src="https://github.com/user-attachments/assets/0e70e1b0-0cb5-4007-9bdc-68032e2da423" />

*Figure 25: Final assembled lipstick container printed using gray SLA resin.*

### PETG vs. SLA Print Comparison

I compared the PETG prototype with the final SLA print to evaluate the differences in size, appearance, and functionality.

<img width="1152" height="1536" alt="image" src="https://github.com/user-attachments/assets/6b44da9f-3d97-4503-8a02-abb9e87274f2" />

*Figure 26: Side-by-side comparison of the PETG prototype and final gray SLA resin print.*

The PETG prototype successfully demonstrated the complete twist-up mechanism, while the SLA print had a smoother surface finish but did not function as intended.

Although the guide pin was able to slide through the spiral groove in the SLA print, the rotating base did not fit over the outer body correctly, preventing the mechanism from operating.

This comparison showed how differences in printing methods, scaling, and dimensional accuracy can affect the functionality of moving assemblies.

### Final Fit Measurements

I measured the guide pin and spiral slot on the SLA print using calipers to evaluate the final clearance.

| Feature | Measured Dimension |
|---|---|
| Guide Pin Width | 1.68 mm |
| Spiral Slot Width | 1.71 mm |
| Actual Clearance | 0.030 mm |

**Clearance = 1.71 - 1.68 = 0.030 mm**

The measured clearance was larger than the RC2 reference range, but the guide pin was still able to slide through the spiral slot.

While the final SLA assembly did not fully function, the successful PETG prototype demonstrated that the mechanism could work. The differences between the two prints highlighted the importance of dimensional accuracy and testing when designing functional 3D printed parts.

## Research Sources

1. *Machinery's Handbook*, page 654, Table 8a, ANSI/ASME B4.1.
2. [Formlabs - Introduction to Post-Curing Prints](https://formlabs.com/support/Introduction-to-Post-Curing-Prints/)
3. [Formlabs - Understanding Accuracy, Precision, and Tolerance in 3D Printing](https://formlabs.com/blog/understanding-accuracy-precision-tolerance-in-3d-printing/)
4. https://haokan.baidu.com/v?vid=4821194170485125459&pd=pcshare&hkRelaunch=p1%3Dpc%26p2%3Dvideoland%26p3%3Dshare_input
