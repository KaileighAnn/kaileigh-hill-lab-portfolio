# L3 - Design Something Small

## Research

For this lab, I researched three infill patterns that we did not go over in class: **Adaptive Cubic, Rectilinear, and Hilbert Curve**. Each pattern has a different shape and can be useful depending on what the part is being used for.

### Adaptive Cubic

Adaptive Cubic uses cube-shaped sections that get smaller and more dense closer to the walls of the part. This pattern is useful for larger prints because it can give the part good support without using as much material throughout the entire inside.

<img width="768" height="635" alt="prusa-slicer_zlVdiEYu4q-768x635" src="https://github.com/user-attachments/assets/46d90b17-1ebd-457f-8bda-4a58a7b65165" />


### Rectilinear

Rectilinear infill is made up of straight, parallel lines that change direction between layers. It is a good option for basic prints because it is simple, prints fairly quickly, and does not use a lot of extra material.

<img width="2048" height="1536" alt="rectilinear_final-2048x1536" src="https://github.com/user-attachments/assets/1b6d27db-cd99-41b7-b4f9-b52cc5573a3e" />


### Hilbert Curve

Hilbert Curve infill creates a continuous maze-like pattern inside the part. One interesting use for this pattern is for parts that may be filled with epoxy or another material after printing because the pattern creates connected spaces throughout the inside.

<img width="2048" height="1536" alt="hilbert_curvefinal-2048x1536" src="https://github.com/user-attachments/assets/ceb282b0-47c1-4839-8524-27b4b6df6f95" />


### How Does Infill Percentage Affect Mechanical Properties?

Increasing the infill percentage generally makes a part **stronger and stiffer** because there is more material supporting the inside. However, it also makes the part heavier, uses more filament, and takes longer to print. A lower infill percentage does the opposite and is better when high strength is not needed.

### How Do Different Infill Patterns Affect Mechanical Properties?

Different infill patterns change how the material is arranged inside the part and how forces are distributed. Because of this, two parts with the same infill percentage can still have different strengths depending on the pattern being used.

## Research Sources

- **Prusa Research – Infill Patterns:**  
  https://help.prusa3d.com/article/infill-patterns_177130
  
  (Pictures came from here also)

- **Prusa Research – Infill:**  
  https://help.prusa3d.com/article/infill_42

## Design

For this assignment, I decided to make a dog tag for my dog. I wanted to print something that I would actually use, and of course the first thing that came to mind was something for my dog.

### Step 1 – Starting Shape

<img width="955" height="562" alt="1" src="https://github.com/user-attachments/assets/d02f22e9-97b9-45c9-8f7d-7cf318b5e746" />


First, I started with two circles that were tangent to each other, each with a diameter of **0.5 in**. This gave me a total height of **1 in**.

### Step 2 – Adding the Other Side

<img width="950" height="560" alt="2" src="https://github.com/user-attachments/assets/013e9074-5c57-448a-87bf-84a3b93b1de1" />

Then I added two more circles that were the same size as the first two and parallel to them.

### Step 3 – Setting the Width

<img width="951" height="528" alt="3" src="https://github.com/user-attachments/assets/63970d87-3cf9-47c6-8b3b-6374f16057e1" />


I changed the distance between the two sets of circles to **1 in**, so the center points of the circles were 1 in apart. This made the overall width of the part **1.5 in**, which meets the size requirements in the instructions.

### Step 4 – Connecting the Shape

<img width="950" height="560" alt="4" src="https://github.com/user-attachments/assets/91376d19-fb09-413f-8b1f-19f3c1a24e9c" />


Then I added parallel lines to connect the two sets of circles.

### Step 5 – Cleaning Up the Sketch

<img width="950" height="557" alt="5" src="https://github.com/user-attachments/assets/0a03a5ee-6536-4abe-b4f8-8a7e8df33e4a" />


I used the **Delete Segment** tool to remove the inside sections and create the final outside shape that I wanted.

### Step 6 – Extruding the Part

<img width="948" height="560" alt="6" src="https://github.com/user-attachments/assets/a230059e-9e49-411c-a227-227a9a30b883" />


After finishing the sketch, I pressed **OK**, which brought me to the extrude screen.

### Step 7 – Setting the Thickness

<img width="952" height="562" alt="7" src="https://github.com/user-attachments/assets/19586831-23a7-46dd-838c-dadbf42433d1" />


I changed the view to the side and extruded the part to a thickness that looked proportional and strong enough so the dog tag would not be too fragile.

### Step 8 – Adding the Collar Loop

<img width="956" height="557" alt="8" src="https://github.com/user-attachments/assets/1e288d48-1c7d-4efd-adfa-2de5b2923cb6" />


After looking at the design, I realized I needed a way to attach the tag to my dog's collar. I added two circles centered on the middle line to create the loop.

### Step 9 – Finishing the Loop

<img width="953" height="560" alt="9" src="https://github.com/user-attachments/assets/e3717f14-7ae2-4a99-b81a-d4b3dbb56a7e" />


I used the **Delete Segment** tool again to make the loop part of the same sketch. I chose **0.08 in** for the inner radius and **0.15 in** for the outer radius because I felt those dimensions looked proportional to the rest of the tag.

### Step 10 – Extruding the Loop

<img width="945" height="557" alt="10" src="https://github.com/user-attachments/assets/e4676d81-6b25-46bc-8628-274dd9cde0c8" />


Then I pressed **OK**. Since I had already created the original extrusion, the new section matched the thickness of the rest of the part.

### Step 11 – Preparing for the Text

<img width="956" height="562" alt="11" src="https://github.com/user-attachments/assets/7f973f76-114e-4f58-8875-033e6949ccea" />


Next, I selected the top surface of the part and started another sketch. I added centerlines so I could make sure the text was placed directly in the middle of the dog tag.

### Step 12 – Adding the Name

<img width="953" height="557" alt="12" src="https://github.com/user-attachments/assets/0fd4f751-b890-487f-8828-5fb22f8b4eef" />


I used the center point as the starting point for the text and typed **“DIXIE.”** I changed the horizontal setting to **Center** and the vertical setting to **Middle** so the name would stay centered on the tag.

### Step 13 – Sizing the Text

<img width="947" height="560" alt="13" src="https://github.com/user-attachments/assets/d2516115-f544-4af7-8b85-3e205b991bee" />


I changed the height of the text to **0.25 in** while making sure it stayed centered on the part.

### Step 14 – Engraving the Text

<img width="955" height="563" alt="14" src="https://github.com/user-attachments/assets/254d3cf2-1799-4754-a7d9-37deee13414a" />


I changed the extrude direction so the text would go into the part instead of sticking out. I set the depth to **0.05 in**, which created a small engraved section without cutting too far into the tag.

### Final Design

<img width="956" height="563" alt="15" src="https://github.com/user-attachments/assets/ec74fef2-2b90-4811-8d02-198cb9fd4b4f" />


This is what my final dog tag design looked like before exporting it into PrusaSlicer.

## Preprocessor and Printing

After finishing my design in Creo, I exported the part as an STL file and opened it in PrusaSlicer. I then adjusted the print settings to meet the requirements for this lab.

### Build Orientation

I placed the dog tag flat on the build plate with the largest surface facing down and the words facing up. I had to rotate the part 90degrees in the x direction to get it to this point. I chose this orientation because it gives the part a stable surface on the build plate and allows it to print without needing supports.

<img width="959" height="599" alt="image" src="https://github.com/user-attachments/assets/e107d4ae-92cd-47e1-99b4-4601f5962b16" />

### Scaling and Final Dimensions

I did not need to scale my part because I originally designed it using inches in Creo. When I imported the part into PrusaSlicer, the dimensions were shown in millimeters, but they were the correct conversions of the dimensions I used in Creo. The final size was **37.97 × 25.27 × 6.35 mm**, or about **1.50 × 1.00 × 0.25 in**, which meets the size requirements for the assignment.

### Infill Settings

I changed the infill from the default **15% to 25%** and changed the pattern to **Rectilinear**. I chose 25% because I wanted the dog tag to be a little stronger since it will actually be used on my dog's collar, but I also did not want to use more material than needed. I chose Rectilinear because it is a simple pattern that gives the inside of the part support while still keeping the print time low.

<img width="959" height="539" alt="image" src="https://github.com/user-attachments/assets/2daa9790-53c2-48a0-9553-71b7837fc806" />

### Wall Thickness

I changed the wall thickness from the default **2 perimeters to 3 perimeters**. I chose to make the walls a little thicker because the dog tag will actually be used on my dog's collar, so I wanted it to be stronger and less likely to break.

<img width="959" height="539" alt="image" src="https://github.com/user-attachments/assets/a08b4e15-1476-40e4-a19d-7d9de1137a39" />

### Sliced Preview and Print Time

After changing my settings, I sliced the final design to make sure everything was ready to print. I used **Generic PLA** on the **Prusa CORE One with a 0.4 mm nozzle**. PrusaSlicer estimated the print time to be about **10 minutes** and the part would use about **3.69 g of filament**. This is well under the required print time of 1.5 hours.

<img width="959" height="539" alt="image" src="https://github.com/user-attachments/assets/af80d6ab-79c0-4453-b109-09e5f3335353" />


Here is a closer look at the slice.
<img width="644" height="476" alt="image" src="https://github.com/user-attachments/assets/22130f9d-9dfc-4d3b-b822-30a41a67f620" />

## Print

### Printing Process

After finishing all of my settings in PrusaSlicer, I exported the G-code and took it to the printer. My part was printed on the same build plate as Candy Vasquez.

<img width="959" height="599" alt="part3" src="https://github.com/user-attachments/assets/b9b36d04-7e7b-4f27-9180-8d3751c9bee8" />

The print started successfully and I watched the first few layers to make sure the parts were sticking to the build plate correctly.

<video autoplay muted loop playsinline width="500">
  <source src="/kaileigh-hill-lab-portfolio/Labs/L03/3d-printing.mp4" type="video/mp4">
</video>

### During the Print

I checked on the print throughout the process to make sure there were no problems. The parts continued printing correctly and stayed attached to the build plate.

<img width="428" height="571" alt="IMG_0496" src="https://github.com/user-attachments/assets/844249a3-dbd1-4b1e-8044-c3b3320e2a76" />

### Final Print

The dog tag printed successfully and the final part came out close to how I designed it in Creo. The engraved **DIXIE** text and the loop for attaching it to a collar both printed correctly.

<img width="302" height="403" alt="IMG_0506 (1)" src="https://github.com/user-attachments/assets/a0ffabd8-8bf0-470d-8318-220235486de3" />

### 3D Operation Video

The video below shows the final dog tag and how it can be attached and used on a dog collar.

[3D operation video]

## Lessons Learned

### What I Learned

This lab helped me understand more about how the settings in PrusaSlicer actually affect the final part. I learned that infill percentage, infill pattern, and wall thickness can all change how strong a part is and how much material it uses. I also got more practice designing something in Creo and then taking that design all the way through the 3D printing process. I also learned that these little detail can affect the time by a lot. 

