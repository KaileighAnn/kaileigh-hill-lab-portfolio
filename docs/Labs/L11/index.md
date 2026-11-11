# Lab 11: Snap-Fit Design for SLA Printing (Form 4)

## Objective

The objective of this lab was to design and manufacture a functional snap-fit assembly using SLA 3D printing. The project focused on understanding how material properties, tolerances, geometry, and print orientation influence the performance of snap-fit connections.

For this project, I designed a small rectangular storage box with a removable snap-fit lid using SolidWorks. The goal was to create a functional enclosure that could be assembled without screws, adhesives, or additional fasteners.

The components were prepared for printing in PreForm using Alpha Clear V1 resin.

---

## 1. Snap-Fit Research

### Snap-Fit Design Principles

Snap-fit joints are mechanical connections that use elastic deformation to connect two components. During assembly, a flexible feature temporarily deflects to pass over a mating surface. Once the retaining feature reaches its engaged position, the elastic component returns toward its original shape and holds the parts together.

For this project, I designed a snap-fit enclosure using four retaining features on the underside of the lid.

The design incorporates angled engagement geometry intended to guide the lid into place and provide retention.

Important design considerations included:

- **Deflection:** The mating features must accommodate enough movement for assembly without exceeding the allowable material strain.
- **Undercut:** Retaining geometry must create mechanical engagement that prevents unintended separation.
- **Stress Concentrations:** Sharp corners can create localized stress concentrations and increase the risk of cracking.
- **Thickness:** Thinner flexible sections generally require less force to deflect, while thicker sections provide greater stiffness.
- **Clearance:** Proper spacing between the lid and box is necessary to accommodate manufacturing tolerances.
- **Material Properties:** Resin stiffness and allowable strain influence the flexibility and durability of the snap-fit connection.


### Mechanical Principles

The performance of a cantilever-type snap fit can be approximated using beam bending relationships.

For a rectangular cantilever with a constant cross-section, the maximum bending strain is approximately:

**Maximum Bending Strain:**

## ε_max = (3tδ) / (2L²)

Where:

- **ε_max** = Maximum bending strain
- **t** = Cantilever thickness
- **δ** = Required tip deflection
- **L** = Cantilever length

This equation shows that increasing the length of the flexible section reduces the strain for a given deflection.

The approximate transverse force required to deflect a constant-section cantilever is:

**Transverse Deflection Force:**

## F = (Ebt³δ) / (4L³)

Where:

- **F** = Transverse deflection force
- **E** = Elastic modulus
- **b** = Cantilever width
- **t** = Cantilever thickness
- **δ** = Required tip deflection
- **L** = Cantilever length

These simplified equations demonstrate how the geometry and stiffness of a flexible feature influence its mechanical behavior. Actual assembly forces also depend on friction, contact angles, and engagement geometry.

### Application to My Design

For my snap-fit box, I incorporated four retaining features into the underside of the lid.

The angled geometry was intended to assist with assembly by guiding the lid into the box opening.

The design required sufficient clearance between the lid and box to allow the retaining features to engage without damaging the resin.

**Figure 1: Snap-Fit Design Geometry**

<img width="521" height="316" alt="image" src="https://github.com/user-attachments/assets/6ba249fb-2563-4e5c-90dd-1f1569d29b02" />

*Figure 1: SolidWorks model showing the four retaining features located on the underside of the lid.*

### SLA Resin Considerations

SLA printing uses a photopolymer resin that is cured using light. This process produces detailed components with relatively smooth surface finishes.

Unlike FDM-printed PLA, the mechanical properties of SLA components depend strongly on the selected resin formulation and post-curing conditions.

For this project, Alpha Clear V1 resin was selected in PreForm.

The snap-fit design needed to account for:

- Resin stiffness and allowable strain
- Potential cracking during assembly
- Dimensional accuracy after curing
- Clearance between mating features
- Support placement near critical surfaces

### Research Reference

*Snap-Fit Joints for Plastics – A Design Guide*, provided through Canvas.

---

## 2. Design

### Design Concept

For this project, I designed a small rectangular box with a removable snap-fit lid using SolidWorks.

The assembly consists of two components:

1. **Bottom:** A hollow rectangular box that provides storage space and serves as the mating component.
2. **Top:** A rectangular lid containing four retaining features designed to secure it to the box.

The purpose was to create a useful enclosure that demonstrates a mechanical connection without additional fasteners.

### Box Body Design

I began by creating a rectangular sketch in SolidWorks.

Using the Extruded Boss/Base feature, I created the main rectangular body. I then used the Shell feature to remove the interior material while maintaining the surrounding walls and bottom surface.

This created a hollow storage compartment with an open top.

**Figure 2: Box Body CAD Model**

<img width="656" height="429" alt="image" src="https://github.com/user-attachments/assets/2271f41b-14d5-4818-a224-4ee3ce6c51fc" />

*Figure 2: SolidWorks model of the hollow box body created using Extruded Boss/Base and Shell.*

### Snap-Fit Lid Design

Next, I created the lid as a separate SolidWorks part.

I started with a rectangular base using Extruded Boss/Base. Additional extruded geometry and cut features were then used to create four retaining features on the underside of the lid.

The features were positioned around the interior perimeter of the lid to engage with the box.

The angled surfaces were intended to help guide the lid into place during assembly.

**Figure 3: Snap-Fit Lid CAD Model**

<img width="580" height="373" alt="image" src="https://github.com/user-attachments/assets/c640efe3-3015-48d7-b41c-68b8a1a4589e" />

*Figure 3: SolidWorks model showing the underside of the lid with four retaining features.*

### Snap-Fit Mechanism

The lid was designed to attach to the box through mechanical engagement between the retaining features and the box geometry.

As the lid is pressed into position, the mating geometry must accommodate the movement required for engagement.

Once seated, the retaining features are intended to resist separation and keep the lid attached.

The enclosure was designed to allow the lid to be removed when access to the interior is needed.

### Design Considerations

The following factors influenced the design:

- **Clearance:** Space was provided between mating surfaces to allow assembly.
- **Engagement:** Four retaining features were incorporated to secure the lid.
- **Wall Thickness:** The box walls needed sufficient thickness to maintain structural integrity.
- **Flexibility:** The engagement geometry needed to accommodate movement without damaging the resin.
- **Printability:** The two components were designed for separate SLA printing.
- **Functionality:** The design was intended to provide a reusable connection.

### CAD Assembly

After completing both components, I created a SolidWorks assembly to check their alignment.

The assembly was used to visualize the completed enclosure and inspect the positioning of the lid relative to the box.

**Figure 4: SolidWorks Assembly**

<img width="593" height="395" alt="image" src="https://github.com/user-attachments/assets/1b1412fc-1d2a-4caf-8dfb-d76f6d97cbe2" />

*Figure 4: Isometric SolidWorks assembly showing the snap-fit lid positioned above the hollow box.*

### Design Dimensions

| Parameter | Dimension |
|---|---|
| Box Length |10 mm |
| Box Width |8 mm |
| Box Height |5 mm |
| Box Wall Thickness |1 mm |
| Lid Thickness |1 mm |
| Number of Retaining Features | 4 |
| Snap-Fit Clearance | 0.2 mm |
| Retaining Feature Dimensions | 8.0 × 2.0 × 1.0 mm |

### Design Summary

The final CAD assembly consisted of a hollow rectangular box and a removable lid containing four retaining features.

Both components were exported for preprocessing and SLA printing.

---

## 3. Preprocessing

### Printer and Material Selection

After completing the SolidWorks assembly, I exported the two components as STL files and imported them into PreForm.

The components were prepared using Alpha Clear V1 resin with a layer thickness of 0.100 mm.

### PreForm Settings

| Parameter | Setting |
|---|---|
| Software | PreForm |
| Printer Setup | Form Studio 1 |
| Printer Selection | MatureImpala |
| Material | Alpha Clear V1 |
| Layer Height | 0.100 mm |
| Number of Components | 2 |
| Support Structures | Generated |
| Estimated Print Time | Approximately 1 hour |
| Estimated Resin Volume | 13.38 mL |

### Build Orientation

Both components were positioned at an angle on the build plate.

The box body was tilted with support structures underneath, while the lid was positioned at an angle with supports extending to its lower surfaces.

This orientation was intended to support the geometry during printing and reduce the likelihood of unsupported regions.

The components were arranged separately to allow adequate spacing between the models and support structures.

### Support Strategy

PreForm support structures were generated for both components.

The supports provided contact points beneath the parts to hold them during printing.

Support placement was particularly important because the lid contained retaining features that needed to maintain their geometry after printing.

### Isotropic vs. Anisotropic Properties

SLA components are generally more mechanically uniform across printing directions than FDM parts because they do not rely on extruded filament roads.

However, SLA components are not necessarily perfectly isotropic. Print orientation, resin chemistry, curing conditions, and processing can still influence mechanical behavior.

For this project, the printing orientation was selected primarily to accommodate the geometry and support requirements.

### Build Plate Layout

The two components were arranged on the build plate with separate support structures.

The estimated total resin volume reported by PreForm was 13.38 mL.

The estimated print time was approximately one hour.

**Figure 5: PreForm Build Plate Layout**

<img width="493" height="419" alt="image" src="https://github.com/user-attachments/assets/3d60894a-b133-4579-ab5b-a209cf7eb8ac" />

*Figure 5: PreForm setup showing the angled orientation, generated supports, Alpha Clear V1 resin, 0.100 mm layer height, and estimated print details.*

## 4. Post-Processing

### Washing

After printing, the components were prepared for washing to remove uncured resin from their surfaces.

The washing process is important because residual resin can affect the surface finish and dimensional fit of the snap-fit features.

**Wash Time:** 15 minutes

**Figure 6: Washing Process**

![Figure 6: Washing](INSERT-IMAGE-LINK)

*Figure 6: Printed components during the resin washing process.*

### Support Removal

The support structures were removed from the printed components using [INSERT METHOD].

Care was required around the lid's retaining features to prevent damage to the engagement geometry.

![Figure 7: Support removal](INSERT-IMAGE-LINK)

*Figure 7: Removal of support structures from the SLA printed components.*

### Curing

Following washing, the components were post-cured according to the selected resin's processing requirements.

Post-curing affects the final mechanical properties of SLA resin, including stiffness, strength, and allowable deformation.

These changes are particularly important for snap-fit designs because the retaining features must withstand movement during assembly.

**Curing Time:** 5 minutes

<img width="302.4" height="403.2" alt="IMG_2518" src="https://github.com/user-attachments/assets/1ab62741-d84b-4c21-9ec2-2b423923e66a" />

*Figure 8: SLA printed components undergoing post-curing.*

### SLA vs. FDM Printing

SLA printing provides several advantages over FDM printing, particularly for components containing small details.

| Property | SLA Resin | FDM PLA |
|---|---|---|
| Printing Process | Photopolymerization | Filament Extrusion |
| Surface Finish | Generally Smooth | Visible Layer Lines |
| Feature Detail | High | Nozzle Dependent |
| Layer Height | 0.100 mm Used | Varies |
| Mechanical Behavior | Resin and Cure Dependent | Strongly Orientation Dependent |
| Post-Processing | Washing and Curing | Usually Support Removal |
| Snap-Fit Flexibility | Depends on Resin Properties | Depends on Geometry and Orientation |

The post-processing stage was important for preparing the parts for assembly and evaluating their final fit.

---

## 5. Validation

### Snap-Fit Testing

After post-processing, the box and lid were evaluated to determine whether the retaining features could engage properly.

The main objective was to verify that the lid could attach securely to the box without damaging either component.

The following factors were evaluated:

- Alignment between the lid and box
- Ease of assembly
- Engagement of the retaining features
- Security of the connection
- Ability to remove the lid
- Visible cracking or deformation


### Testing Results

| Test | Result |
|---|---|
| Lid Alignment | Lid aligned properly with the box. |
| Snap Engagement | Snap-fit features engaged successfully. |
| Fit Tightness | Snug and secure fit. |
| Lid Retention | Lid remained securely attached. |
| Lid Removal | Lid could be removed without difficulty. |
| Visible Cracking | No visible cracks or damage observed. |
| Repeated Assembly | Successfully assembled and removed multiple times. |
| Overall Functionality | All components functioned as intended. |

### Final Printed Components

<img width="115.2" height="153.6" alt="2d86b0a9-bf1a-4585-ac9f-eb75a2d9010b" src="https://github.com/user-attachments/assets/17559742-d3bb-4446-9365-8914c2eba089" />


*Figure 9: Completed SLA printed box and lid after post-processing.*

### Completed Assembly

<img width="153.6" height="204.8" alt="download" src="https://github.com/user-attachments/assets/520cf10f-8020-45dc-b06f-432ab3f629bb" />

*Figure 10: Completed storage box showing the lid attached to the box body.*

### Snap-Fit Demonstration

<p align="center">
  <video autoplay muted loop playsinline width="500">
    <source src="/kaileigh-hill-lab-portfolio/Labs/L11/IMG_2535.mp4" type="video/mp4">
  </video>
</p>

*Figure 11: Video demonstrating the attachment and removal of the snap-fit lid.*

### Validation Summary

The snap-fit box was successfully printed and assembled. The lid aligned properly with the base and snapped securely into place, providing a snug fit while still allowing easy removal. The snap-fit features functioned as intended, with no visible cracking or damage during testing. The lid could be repeatedly attached and removed without issues. No major adjustments were necessary, and the overall design functioned as expected.

---

## 6. Lessons Learned

This project provided hands-on experience designing a mechanical connection for SLA 3D printing.

One of the main design considerations was creating a connection that could securely hold the lid while still allowing assembly and removal.

The project demonstrated the importance of understanding how geometric features, material stiffness, and dimensional clearance influence the performance of a snap-fit mechanism.

### Design Challenges

Designing the retaining features required consideration of how the lid would engage with the box.

Unlike a simple press-fit connection, a snap-fit mechanism requires geometry that allows temporary deformation and mechanical retention.

The design also needed to account for the limitations of SLA resin, particularly the possibility of cracking when thin features experience excessive strain.

### Manufacturing Considerations

Preparing the components in PreForm demonstrated the importance of print orientation and support placement.

The parts were tilted and supported to accommodate their geometry during printing.

The estimated print required approximately one hour and 13.38 mL of resin, including the material estimated by PreForm for the build.

### SLA vs. FDM

Compared with FDM printing, SLA provides smoother surfaces and greater detail for small mechanical features.

However, the material properties of SLA resin require careful consideration when designing components that must bend or flex.

Post-curing also introduces an additional manufacturing step that can affect the final mechanical behavior of the parts.


### Project Time and Resources

| Task | Time |
|---|---|
| Snap-Fit Research | 20 minutes |
| SolidWorks CAD Design | 1 hour |
| PreForm Preprocessing | 15 minutes |
| Estimated Printing | 1 hour |
| Washing | 15 minutes |
| Curing | 30 minutes |
| Support Removal | 15 minutes |
| Validation | 15 minutes |
| Documentation | 40 minutes |
| **Total Project Time** | **4 hours 30 minutes** |

**Material:** Alpha Clear V1 Resin

**Estimated Resin Usage:** 13.38 mL

### Conclusion

Lab 11 provided experience designing a two-component enclosure with a snap-fit lid using SolidWorks and preparing it for SLA manufacturing.

The project demonstrated how mechanical engagement, material selection, clearance, and manufacturing conditions must be considered when designing functional snap-fit components.

Through the design and preprocessing stages, I gained a better understanding of how snap-fit mechanisms can be incorporated into useful 3D-printed assemblies.

The final print functioned as intended, with the lid snapping securely into place while remaining easy to remove. Testing demonstrated the importance of proper clearances, material flexibility, and dimensional accuracy when designing functional snap-fit components for SLA printing.

---

## References

1. *Snap-Fit Joints for Plastics – A Design Guide*. Course document provided through Canvas.
2. Formlabs. *Form 4 and PreForm Documentation*. https://formlabs.com/
3. SOLIDWORKS. *3D CAD Design Software*. https://www.solidworks.com/
