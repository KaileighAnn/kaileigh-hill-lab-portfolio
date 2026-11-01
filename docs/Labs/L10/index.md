
# L10 - SLA Printing Lab: Twist-Up Lipstick Container

## Objective

The objective of this lab is to design and manufacture a functional assembly using stereolithography (SLA) 3D printing while demonstrating an RC2 sliding fit based on the *Machinery's Handbook*. The project also focuses on dimensional accuracy, resin shrinkage, and evaluating the fit of printed components.

For my project, I chose to create a miniature twist-up lipstick container with a removable cap and fake lipstick.

## Design Concept

I wanted to create something that was both functional and visually appealing, so I decided to design a twist-up lipstick container.

The design uses a rotating base and spiral sleeve to raise and lower the lipstick holder. As the base rotates, a guide pin follows the spiral slot, converting rotational motion into vertical movement.

The assembly consists of six components: an outer tube, rotating base, spiral sleeve, lipstick holder, fake lipstick, and removable cap. Each component was modeled separately in SolidWorks before being assembled.

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

### Initial Clearance Calculation

The initial SolidWorks dimensions for the sliding interface are:

| Feature | Dimension |
|---|---|
| Spiral Slot Width | 2.060 mm |
| Guide Pin Width | 2.040 mm |
| Nominal Clearance | 0.020 mm |

**Clearance = Slot Width - Guide Pin Width**

Clearance = 2.060 - 2.040

**Clearance = 0.020 mm**

This is an initial design clearance and has not yet been verified as meeting the RC2 tolerance limits.

### SLA Resin Shrinkage

SLA printing uses UV light to cure liquid resin into solid parts. After printing, the components are washed and post-cured using additional UV light.

According to Formlabs, post-curing can cause additional resin shrinkage as the material continues to cure.

This is important because my sliding interface has a very small clearance, and dimensional changes could cause the guide pin to bind inside the spiral slot.

The amount of shrinkage depends on the resin, printer, and curing conditions. I will research the specific material properties once the resin used for this lab is confirmed.

### Measurement and Testing Plan

After printing and post-curing, I will measure the guide pin and spiral slot using digital calipers and compare the results with the original CAD dimensions.

**Actual Clearance = Measured Slot Width - Measured Pin Width**

I will then assemble the components and test whether the lipstick holder moves smoothly through the spiral groove.

## Research Sources

1. *Machinery's Handbook*, page 654, Table 8a, ANSI/ASME B4.1.
2. [Formlabs - Introduction to Post-Curing Prints](https://formlabs.com/support/Introduction-to-Post-Curing-Prints/)
3. [Formlabs - Understanding Accuracy, Precision, and Tolerance in 3D Printing](https://formlabs.com/blog/understanding-accuracy-precision-tolerance-in-3d-printing/)
