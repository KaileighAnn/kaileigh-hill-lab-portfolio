
# L10 - SLA Printing Lab: Twist-Up Lipstick Container

## Objective

The objective of this lab is to design, manufacture, and evaluate a functional assembly using stereolithography (SLA) 3D printing. The project focuses on designing a sliding fit based on the RC2 specifications from the *Machinery's Handbook*, accounting for dimensional accuracy and resin shrinkage, and evaluating the fit of printed components.

For my project, I chose to design a miniature twist-up lipstick container with a removable cap and a fake lipstick. The goal is to create a functional mechanism that allows the lipstick to move up and down by rotating the base while demonstrating the importance of clearances and tolerances in SLA printing.

## Design Concept

### Twist-Up Lipstick Container

I decided to create a miniature lipstick container because I wanted to design something that was both functional and visually appealing while incorporating a mechanical sliding mechanism.

The design uses a rotating base and spiral groove to raise and lower the lipstick holder. When the base is twisted, the guide pin on the lipstick holder follows the spiral slot, allowing the lipstick to move vertically.

The assembly also includes a removable cap to protect the lipstick when it is not being used.

### Main Components

The lipstick container consists of six individually modeled components:

| Component | Description |
|---|---|
| Outer Tube | Main body that houses the internal mechanism and helps guide the lipstick holder |
| Rotating Base | Bottom component that rotates to operate the mechanism |
| Spiral Sleeve | Contains the helical slot that controls the movement of the lipstick holder |
| Lipstick Holder | Holds the fake lipstick and includes a guide pin that follows the spiral slot |
| Fake Lipstick | Decorative lipstick-shaped component that moves with the holder |
| Removable Cap | Covers and protects the lipstick assembly |

All six components were modeled separately in SolidWorks before being brought together into an assembly.

### How the Mechanism Works

The mechanism is designed to convert rotational motion into linear motion.

1. The user rotates the base of the lipstick container.
2. The rotating base turns the spiral sleeve inside the outer tube.
3. The guide pin on the lipstick holder follows the spiral slot.
4. The outer tube prevents the lipstick holder from rotating freely.
5. As the spiral sleeve rotates, the lipstick holder moves vertically.
6. Rotating the base in the opposite direction lowers the lipstick back into the container.

This mechanism allows the lipstick to extend and retract without requiring the user to pull it out manually.

## Design Requirements

The design was developed around the following requirements:

- Create a functional assembly using SLA 3D printing.
- Incorporate a sliding interface based on RC2 fit principles from the *Machinery's Handbook*.
- Design mating components with appropriate clearances.
- Account for potential dimensional changes during printing and post-curing.
- Model all components in SolidWorks.
- Assemble the components and check for interference.
- Measure the printed features and compare them with the original CAD dimensions.
- Evaluate whether the sliding mechanism operates as intended.

## Design Software and Manufacturing Process

| Category | Selection |
|---|---|
| CAD Software | SolidWorks |
| Manufacturing Method | Stereolithography (SLA) 3D Printing |
| Fit Reference | Machinery's Handbook, RC2 Sliding Fit |
| Design Units | Millimeters (mm) |
| Printer | TBD |
| Resin Material | TBD |
| Post-Curing Settings | TBD |

SolidWorks was used to create the individual components and evaluate how they fit together before manufacturing.

SLA printing was selected for this assignment because of its ability to produce small features, detailed geometries, and relatively smooth surfaces.

The printer, resin, and curing settings will be documented once the manufacturing equipment and materials are confirmed.

## Initial Design Dimensions

The following dimensions were used to develop the initial SolidWorks models.

| Component | Initial Dimensions |
|---|---|
| Outer Tube | 22 mm outer diameter, 60 mm height, 2 mm wall thickness |
| Rotating Base | 24 mm diameter, 12 mm height |
| Rotating Shaft | 6 mm diameter, 8 mm length |
| Spiral Sleeve | 17.5 mm outer diameter, 14 mm inner diameter, 40 mm height |
| Spiral Slot | 2.06 mm width |
| Lipstick Holder | 13.5 mm outer diameter, 15 mm height |
| Guide Pin | 2.04 mm width with rounded corners |
| Fake Lipstick | 10.2 mm diameter, 25 mm height |
| Removable Cap | 25 mm outer diameter, 50 mm height, 1.5 mm wall thickness |

These dimensions represent the initial CAD design and may be adjusted after evaluating the assembly and SLA printing tolerances.

## Design Considerations

Several factors were considered during the design process, including the overall size of the lipstick container, the movement of the internal mechanism, and the clearances between mating components.

One of the most important design considerations was the connection between the guide pin on the lipstick holder and the spiral slot on the spiral sleeve.

This connection must provide enough clearance for movement while limiting unwanted looseness.

Because the components will be manufactured using SLA printing, dimensional accuracy and shrinkage during post-curing must also be considered.

The following section discusses the RC2 sliding fit research and how SLA shrinkage may affect the final design.

## RC2 Sliding Fit Research and SLA Shrinkage

### Machinery's Handbook Reference

For this project, I researched the Class RC2 sliding fit using the *Machinery's Handbook*, page 654, Table 8a, which covers American National Standard Running and Sliding Fits (ANSI/ASME B4.1).

RC2 sliding fits are intended to provide accurate positioning while allowing parts to move easily with a small amount of clearance. These fits allow more maximum clearance than RC1 fits but are not intended for unrestricted free-running motion.

![Machinery's Handbook RC2 Fit Table](INSERT_IMAGE_URL_HERE)

*Figure 1: Table 8a from Machinery's Handbook showing the running and sliding fit specifications, including Class RC2.*

### Selected Sliding Interface

For my SLA printing project, I designed a miniature twist-up lipstick container with a removable cap and a fake lipstick.

The mechanism uses a rotating base, spiral sleeve, and lipstick holder to raise and lower the lipstick.

I selected the connection between the **guide pin on the lipstick holder and the spiral slot on the spiral sleeve** as the sliding interface.

As the base rotates, the guide pin follows the spiral groove, causing the lipstick holder to move vertically.

The RC2 specification is formally defined for cylindrical hole-and-shaft fits. Since my design uses a pin-and-slot connection, I am applying the clearance principles of RC2 as a reference rather than claiming that the geometry itself is a standardized RC2 fit.

### Initial Design Dimensions

| Feature | CAD Dimension |
|---|---|
| Spiral Slot Width | 2.060 mm |
| Guide Pin Width | 2.040 mm |
| Nominal Clearance | 0.020 mm |
| Guide Pin Shape | Rectangular with four rounded corners |
| Manufacturing Process | SLA 3D Printing |

### Clearance Calculation

The initial clearance was calculated by subtracting the guide pin width from the spiral slot width.

**Clearance = Slot Width - Guide Pin Width**

Clearance = 2.060 mm - 2.040 mm

**Nominal Clearance = 0.020 mm**

This clearance was selected as an initial design target to minimize excess movement while allowing the guide pin to slide through the spiral slot.

The selected clearance has not yet been verified against the applicable RC2 tolerance range in the *Machinery's Handbook*. It will also need to be evaluated against the dimensional accuracy of the SLA printing process.

### SolidWorks Design Adjustments

During the modeling process, I initially created a rectangular guide pin on the side of the lipstick holder.

After examining the connection between the guide pin and spiral slot, I added fillets to all four corners of the guide pin.

The rounded corners were intended to reduce the possibility of the pin catching on the edges of the spiral groove during movement.

I updated the SolidWorks assembly and confirmed that the modified guide pin fits inside the spiral slot without visible interference.

This initial fit check confirms geometric compatibility in the CAD model, but additional testing will be needed to determine whether the mechanism moves smoothly.

### SLA Resin Shrinkage and Post-Curing Research

Stereolithography (SLA) printing uses UV light to cure liquid photopolymer resin into solid layers.

After printing, the parts are typically washed to remove uncured resin and then exposed to additional UV light during post-curing.

According to Formlabs, post-curing increases polymer cross-linking, which improves the mechanical properties of the printed parts but can also cause additional shrinkage.

The amount of shrinkage depends on the resin material, printing conditions, and post-curing settings.

Shrinkage is especially important for my lipstick container because the guide pin must move through the spiral slot with very little clearance.

### Factors Affecting Dimensional Accuracy

Several factors may affect the final dimensions of the printed components:

- Resin type and material properties
- UV exposure during the printing process
- Washing and drying conditions
- Post-curing time and temperature
- Part orientation during printing
- Support placement and removal
- Printer resolution and dimensional accuracy

These factors can cause the actual dimensions of the printed components to differ from the original SolidWorks dimensions.

The exact shrinkage percentage will need to be researched using the manufacturer specifications for the printer and resin selected for this project.

### Effect of Shrinkage on the Sliding Fit

The initial design provides only 0.020 mm of nominal clearance between the guide pin and spiral slot.

Because this clearance is very small, even minor dimensional changes could affect the operation of the mechanism.

Shrinkage and printing errors may affect the guide pin and spiral slot differently. Therefore, I cannot assume that both features will shrink by the same percentage or that their clearance will remain constant.

If the final clearance is too small, the guide pin may bind inside the spiral slot.

If the clearance is too large, the lipstick holder may experience unwanted movement or looseness.

The final dimensions may need to be adjusted based on the printed results.

### Measurement and Testing Plan

After printing, washing, and post-curing the components, I will measure the guide pin and spiral slot using digital calipers or another appropriate measuring instrument.

I will compare the measured dimensions with the original CAD dimensions to evaluate dimensional accuracy.

| Feature | CAD Dimension | Measured Dimension |
|---|---|---|
| Spiral Slot Width | 2.060 mm | TBD |
| Guide Pin Width | 2.040 mm | TBD |
| Clearance | 0.020 mm | TBD |

The actual clearance will be calculated using:

**Actual Clearance = Measured Slot Width - Measured Pin Width**

I will then assemble the components and test whether the lipstick holder moves smoothly through the spiral groove.

The results will be used to determine whether the selected clearance is appropriate for the SLA printing process or whether further dimensional adjustments are necessary.

### Research Sources

1. *Machinery's Handbook*, page 654, Table 8a, American National Standard Running and Sliding Fits (ANSI/ASME B4.1).

2. Formlabs, "Introduction to Post-Curing Prints."
   https://formlabs.com/support/Introduction-to-Post-Curing-Prints/

3. Formlabs, "Guide to 3D Printing Tolerances, Accuracy, and Precision."
   https://formlabs.com/blog/understanding-accuracy-precision-tolerance-in-3d-printing/
