# Lab 6 – Artifact Mate: Joystick Snap-Fit

## Objective

The objective of this lab was to parametrically design and 3D print a small component that snap fits onto an existing artifact. I used an analog joystick module as my artifact and designed a custom cap that snaps onto the top of the joystick.

The design was created using measured dimensions from the joystick, parameters and constraints in Creo, and engineered clearance to allow the final part to snap onto the joystick securely.

## Artifact

For my artifact, I used an analog joystick module. I chose the circular top of the joystick as the feature that my design would mate with.

<p align="center">
  <img src="https://github.com/user-attachments/assets/2844be15-693c-4405-87df-8fc68685f2d1" alt="Joystick side view" width="45%">
  <img src="https://github.com/user-attachments/assets/1c82cf23-b46d-45d7-bb22-30a87014c0f1" alt="Joystick top view" width="45%">
</p>

## Measurements and Hand Sketch

I measured the joystick with calipers before beginning the CAD model. The top of the joystick had a diameter of **20.0 mm** and a thickness of **5.0 mm**. The neck underneath the joystick top had a diameter of **10.7 mm**.

The difference between the top and neck created an overhang of:

**(20.0 - 10.7) / 2 = 4.65 mm**

This overhang gave the snap-fit tabs an area to catch underneath the joystick.

<img width="913" height="900" alt="image" src="https://github.com/user-attachments/assets/3d255226-9ea3-4ce4-97be-3428dd2827bb" />

## Parameters and Design Decisions

I used parameters based on the measurements of the joystick so the cap could be easily adjusted if the first print did not fit correctly.

| Parameter | Value | Reason |
|---|---:|---|
| Joystick top diameter | 20.0 mm | Measured from the artifact |
| Joystick top thickness | 5.0 mm | Measured from the artifact |
| Neck diameter | 10.7 mm | Measured from the artifact |
| Clearance | 0.30 mm per side | Allows room for the printed cap to fit over the joystick |
| Cap inside diameter | 20.6 mm | Joystick diameter plus clearance |
| Cap outside diameter | 24.6 mm | Provides a 2 mm wall around the cap |
| Wall thickness | 2.0 mm | Provides strength while still allowing the snap sections to flex |
| Top thickness | 2.0 mm | Provides a solid top without making the part too thick |
| Snap lip | 1.0 mm | Allows the cap to catch underneath the joystick |
| Number of snap sections | 3 | Keeps the snap fit evenly distributed around the joystick |
| Snap section angle | 60° | Creates three equal snap sections with gaps for flexibility |
| Snap spacing | 120° | Evenly spaces the three snap sections around the cap |

### Engineered Allowance

I added **0.30 mm of clearance on each side** of the 20.0 mm joystick. This made the inside diameter of the cap:

**20.0 mm + (2 × 0.30 mm) = 20.6 mm**

The clearance was added because making the opening exactly 20.0 mm could make the printed part too tight to fit over the joystick.

### Snap-Fit Design

I used three snap sections spaced **120° apart** around the bottom of the cap. Each section covers approximately **60°**. The spaces between the sections allow the walls to flex outward while the cap is pushed over the joystick. The **1.0 mm lip** then catches underneath the joystick top to hold the cap in place.

## CAD Design Process

I created the snap-fit cap in Creo using the measurements and parameters from my hand sketch. I built the model in multiple steps so the dimensions and snap-fit features could be controlled and modified if needed.

### Step 1 – Create the Main Body

I started by creating a circular body with an outside diameter of **24.6 mm** and an overall height of **8 mm**.

<img width="960" height="600" alt="l61" src="https://github.com/user-attachments/assets/0261d128-a35d-4221-b93e-6fe903b8e209" />

### Step 2 – Shell the Cap

I used the Shell tool to hollow out the bottom of the part. I used a **2.0 mm wall thickness** to create the cavity for the joystick while keeping the outside walls strong enough for the snap fit.

<img width="1920" height="1200" alt="Screenshot 2026-09-28 210216" src="https://github.com/user-attachments/assets/d06b3227-7340-4ba3-8c52-4c3cebcde147" />

### Step 3 – Round the Top

I rounded the top of the cap to make the shape more comfortable to use and similar to a normal joystick cap.

<img width="1920" height="1200" alt="Screenshot 2026-09-28 210329" src="https://github.com/user-attachments/assets/afdc905a-1ab3-40d7-befd-2607cdf9ef95" />

### Step 4 – Create the Snap Sections

I divided the bottom of the cap into **three snap sections**. Each section was approximately **60°** and the sections were positioned **120° apart** so they were evenly distributed around the cap.

The gaps between the sections allow the walls to flex outward when the cap is pushed over the joystick.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/963baff3-8e49-49a4-8546-eac804f91cc4" />

### Step 5 – Create the Snap Lip

I added a **1.0 mm snap lip** to the bottom of the sections. The lip is designed to pass over the joystick top and catch underneath its edge.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/817206b0-1f77-4dea-ba54-ff16fd018026" />

### Step 6 – Create the Openings

I removed material between the three snap sections. These openings allow each section to flex independently when the cap is installed.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/450bb851-da3a-4757-aa33-19d2c4da4034" />

### Step 7 – Round the Snap-Fit Edges

I rounded the edges of the three snap-fit sections to remove sharp corners and create a smoother transition. This helps the cap slide over the joystick more easily while also reducing stress at the edges of the snap sections.

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f62299f7-a2fe-471c-8aee-543c73e64daa" />

### Final CAD Design

The finished design has three flexible snap sections around the bottom and a rounded top. The final dimensions of the model are approximately **24.6 mm × 24.6 mm × 8.0 mm**.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/a1729197-a3a5-4662-8aef-bc060cbb19f9" />

After completing the model, I exported the part as an **STL file** to prepare it for 3D printing.

## 3D Printing Process

After completing the CAD model, I exported the design as an STL file and imported it into PrusaSlicer to prepare it for printing.

### Slicer Setup

I used **PrusaSlicer 2.9.6** to prepare the part. The STL imported successfully with no errors detected.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/16efcf84-a58c-4659-aa5a-9e27f99be2e3" />

The final model size was **24.6 mm × 24.6 mm × 8.0 mm**.

### Print Settings

| Setting | Value |
|---|---|
| Material | PLA |
| Nozzle diameter | 0.4 mm |
| Layer height | 0.20 mm |
| Number of layers | 40 |
| Infill | 20% |
| Part size | 24.6 × 24.6 × 8.0 mm |
| Model volume | 1710.74 mm³ |
| Filament used | 1.93 g |
| Filament length | 0.65 m |
| Estimated print time | 8 minutes |
| Supports | Support enforcers only |

### Build Orientation

I oriented the part with the rounded top on the build plate and the snap-fit sections facing upward. I chose this orientation to keep the snap-fit features accessible and reduce the amount of support material needed.

### Sliced Model

After slicing, PrusaSlicer generated **40 layers** at a layer height of **0.20 mm**. The estimated print time was approximately **8 minutes**, and the print required approximately **1.95 g of PLA**.

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/e22d144c-b63f-4799-8c17-e218932a9274" />

## Printing

The final STL file was printed using a **Prusa CORE One** with PLA. The slicer estimated approximately 8 minutes, but the actual printing time was **14 minutes 47 seconds**. The printer reported approximately **2 g of PLA** used.

<video autoplay muted loop playsinline width="500">
  <source src="/kaileigh-hill-lab-portfolio/Labs/L06/IMG_1460_converted.mp4" type="video/mp4">
</video>

### Finished Part

After printing, I removed the part from the build plate and inspected the three snap-fit sections. The part printed successfully and the snap features were intact.

<p align="center">
  <img src="https://github.com/user-attachments/assets/f624d623-442f-4282-a44a-8a4985508377" width="32%" />
  <img src="https://github.com/user-attachments/assets/9ce925b9-efca-4ea2-9d5e-b375dade5d01" width="32%" />
  <img src="https://github.com/user-attachments/assets/3a7f7fb8-bef2-4843-8246-9219182d9961" width="32%" />
</p>
