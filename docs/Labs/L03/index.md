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
