
# L08 - Aldi Shopping Cart Coin Keychain

For this lab, Gracie approached me with a task. I designed a functional 3D-printed keychain that can be used in place of a quarter when unlocking an Aldi shopping cart. My goal was to create a small, reusable item that I could keep on her keys so she would not need to carry a physical quarter.

---

## Reading and Writing

Asking smart questions is important in the engineering design process because it helps identify the actual problem before creating a solution. Understanding who will use the product, what it needs to accomplish, and what limitations exist allows engineers to make better design decisions. Asking questions throughout the process can also help identify potential problems early, reduce unnecessary redesigns, and improve the functionality of the final product.

**Reading:** [Great Questions Lead to Great Design](https://www.toptal.com/designers/product-design/design-thinking-great-questions)

---

## Problem Statement

### Purpose of the Design

Aldi shopping carts require a quarter to release the cart from the locking mechanism. This can be inconvenient when I do not have change available. I wanted to design a reusable alternative that Gracie could keep on her keychain and have available whenever she goes shopping.

### How I Noticed the Problem

My friend Gracie noticed this problem because she does not always have cash or loose change when shopping at Aldi. She mentioned how frustrating it can be to find a quarter just to use a shopping cart, so I decided to design a simple 3D-printed keychain that would solve this problem for her.

### Intended User

The intended users are Aldi shoppers who frequently forget to bring a quarter or prefer not to carry loose change. The design is intended to be lightweight, portable, reusable, and easy to access.

### Design Approach

My approach was to create a circular token based on the dimensions of a U.S. quarter and add an extended tab with a hole for a keyring. I used Creo Parametric to create the CAD model and PrusaSlicer to prepare the part for 3D printing.

### Research

I researched the dimensions of a U.S. quarter to determine the approximate size needed for the design. A quarter has a diameter of 24.26 mm and a thickness of 1.75 mm. These dimensions provided a starting point for the model.

I also considered the size of the keyring attachment and how the tab could affect the shopping cart mechanism. The finished part will need to be tested to verify that it functions properly.

**Reference:** [U.S. Mint Coin Specifications](https://www.usmint.gov/learn/coin-and-medal-programs/coin-specifications)

---

## Design

### Step 1 - Creating the Circle

I started my design in Creo Parametric by creating a circular sketch. This circle formed the main body of the keychain and represented the quarter-sized portion of the design.

<img width="960" height="600" alt="Screenshot 2026-10-19 194125" src="https://github.com/user-attachments/assets/4bfb3717-8948-4025-9e09-b800a96cdb8a" />

### Step 2 - Extruding the Circle

After creating the circle, I used the Extrude feature to turn the sketch into a three-dimensional solid. I used the thickness of a quarter as my starting reference.

<img width="960" height="600" alt="Screenshot 2026-10-19 194223" src="https://github.com/user-attachments/assets/7c4024d3-7e60-4688-8351-961e279e09ee" />

### Step 3 - Adding the Tab

Next, I created an extended tab connected to the circular body. I rounded the end of the tab to create a smooth shape and provide enough room for a keyring hole.

<img width="960" height="600" alt="Screenshot 2026-10-19 200102" src="https://github.com/user-attachments/assets/0388da82-88ac-4aa0-a08f-4fdd20189db3" />

### Step 4 - Adding the Keyring Hole

I added a circular hole near the end of the tab and used an extrusion cut to remove the material. This allows the finished part to attach directly to my keys.

<img width="960" height="600" alt="Screenshot 2026-10-19 200215" src="https://github.com/user-attachments/assets/d5fa2d65-4bda-4629-b3f8-89d9c4b7c4ab" />

### Step 5 - Adding the Dollar Sign

After completing the main geometry, I added a dollar sign to the surface of the coin. I used the sketch and extrusion tools in Creo to create the raised detail.

<img width="960" height="600" alt="Screenshot 2026-10-19 200305" src="https://github.com/user-attachments/assets/da0597f1-eff6-4e10-9921-a7bf36ac9f5e" />

### Engineering Allowances and Design Decisions

The most important design consideration was maintaining the approximate dimensions of a quarter while adding a functional keychain attachment.

I used the diameter and thickness of a quarter as starting dimensions. The keyring hole was positioned near the end of the tab to leave material around the opening for strength.

I also considered the tolerances associated with FDM 3D printing. Small dimensional differences can occur during printing, so the finished part will need to be measured and tested.

Another consideration is whether the extended tab will interfere with the shopping cart locking mechanism. If it does, the design will need to be adjusted.

---

## 3D Print

### Printer Information

I imported my completed model into PrusaSlicer and prepared it for printing using Printer #7.

### PrusaSlicer Setup

<img width="960" height="600" alt="Screenshot 2026-10-19 200550" src="https://github.com/user-attachments/assets/604afb2d-b5bd-46ed-b9ff-bc8c142bb36e" />


### Printing Settings

| Setting | Value |
|---|---|
| Printer | #7 |
| Slicer | PrusaSlicer |
| Layer Height | 0.20 mm |
| Supports | Support enforcers only |
| Build Orientation | Flat on build plate |
| Print Time | 4 minutes |


### Build Orientation and Layout

I positioned the keychain flat on the build plate because this provides a large contact area and improves stability during printing. This orientation also reduces the need for supports and allows the circular body and tab to be printed together.

### Supports

The design has very few overhangs when positioned flat on the build plate. I selected the support-enforcers-only option in PrusaSlicer. Since the model is relatively flat, I do not expect additional supports to be necessary unless the slicer identifies unsupported geometry.

### Surface Finish

After printing, I will inspect the surface finish of the keychain, including the top surface, bottom surface, and keyring hole. I will also check for rough edges, visible defects, or areas that require cleanup.

### Slicer Information

I used PrusaSlicer to position the model and review the printing configuration before slicing. I will record the final estimated printing time, filament usage, layer count, and other slice information after completing the slicing process.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/662518b7-b2e7-42be-a770-f3552a62616d" />

### Printing Process Video

The following video documents the 3D printing process.

<video autoplay muted loop playsinline width="500">
  <source src="/kaileigh-hill-lab-portfolio/Labs/L05/IMG_1908.mp4" type="video/mp4">
</video>
### Final Printed Part

After printing, I will inspect the finished keychain and determine whether the dimensions, keyring hole, and overall shape function as intended.

<img width="3024" height="4032" alt="IMG_1911" src="https://github.com/user-attachments/assets/d219ee3f-f1ef-4f3d-a2ec-cf706691fbe2" />


### Functional Testing

The final part will be tested with a keyring to verify that the attachment is functional. I will also compare the printed dimensions to those of a quarter and test whether the token works in a compatible Aldi shopping cart without forcing it into the mechanism.

**Testing Results:** It Worked!

---

## Lessons Learned

This project allowed me to apply the engineering design process to a simple everyday problem. I started by identifying an inconvenience and developing a functional solution that could be manufactured using a 3D printer.

One important part of the design was figuring out how to incorporate the keychain attachment while keeping the circular portion close to the dimensions of a quarter. I had to consider the placement of the tab, the size of the hole, and the overall geometry of the part.

I also practiced using different Creo features, including sketching, extruding, cutting holes, and adding raised details. These features allowed me to create the entire keychain as a single part.

Another important consideration was preparing the model for printing. I positioned the part flat in PrusaSlicer to provide a stable printing surface and reduce the need for support material.

After printing, I will evaluate the dimensional accuracy, surface finish, strength, and functionality of the design. Any mistakes or changes will be documented as part of the design process.


### Time Spent

| Activity | Time |
|---|---|
| Research and Planning | 10 minutes |
| CAD Design | 30 minutes |
| Slicing and Setup | 5 minutes |
| 3D Printing | 4 minutes |
| Testing and Documentation | 15 minutes |
| **Total** | **1 hour 4 minutes** |

### Resources Used

- Creo Parametric
- PrusaSlicer
- 3D Printer #7
- 3D Printing Filament
- U.S. Mint Coin Specifications
- Design Thinking Reading

---

## Conclusion

For this project, I designed an Aldi shopping cart coin keychain as a reusable alternative to carrying a quarter. I created the model in Creo Parametric using a circular body, an extended tab, a keyring hole, and a raised dollar sign. I then imported the model into PrusaSlicer to prepare it for 3D printing.

This project demonstrated how a simple everyday inconvenience can be addressed using mechanical design and additive manufacturing. The final printed part will be evaluated to determine whether it functions as intended and whether any improvements are necessary.
