# Lab 4 - Overhang Angle Benchmark

## Parameter

For this lab, I chose to test the **unsupported overhang angle** of the Prusa CORE One. The class FDM design rules list **45°** as the recommended maximum angle that can be printed without supports. I designed one artifact containing several different angles so I could compare their print quality under the same printing conditions.

My flower benchmark tests **0°, 20°, 30°, 40°, 45°, 50°, 60°, and 70°** overhangs.

### Prediction

Before printing, I predict that the artifact will print successfully through approximately **45° to 50°**. I expect the surface quality to begin noticeably decreasing at the larger angles, especially around **60° and 70°**.

## Design

I wanted my benchmark to perform the required overhang test while also being more visually interesting than a traditional test block. I decided to make the final artifact look like a flower, with each petal representing a different overhang angle.

### Creating the Base Shape

I started by sketching two equal squares and rotated one of the squares relative to the other. Overlapping the two squares created the basic eight-sided geometry for my design.


<img width="960" height="600" alt="a" src="https://github.com/user-attachments/assets/28d466e0-8e71-47f0-a22d-99a30b82e7d3" />


I then added dimensions and constraints to define the geometry of the overlapping squares.


<img width="960" height="600" alt="b" src="https://github.com/user-attachments/assets/bef354b4-c0b4-4312-b232-51926c8b9d97" />


Next, I used the **Delete Segment** tool to remove the unnecessary interior portions of the overlapping squares. I also used the **Line** tool where needed to connect the remaining edges and create one continuous closed shape.


<img width="960" height="600" alt="c" src="https://github.com/user-attachments/assets/66b02287-4c6a-4e9a-9d53-ccf90eb162bc" />


After cleaning up the sketch, I checked the resulting geometry and dimensions to make sure I had a closed profile that could be extruded.


<img width="960" height="600" alt="d" src="https://github.com/user-attachments/assets/3c09c418-3edc-479d-906b-f6e43661660c" />


I then extruded the completed base sketch to create the main three-dimensional body of the artifact.


<img width="960" height="600" alt="e" src="https://github.com/user-attachments/assets/9b575aca-44a0-4cf7-b166-529d200e9971" />


### Creating the Petal Sections

Next, I created a rectangular sketch on one of the outside faces of the model. This rectangle created the geometry that would later become one of the individual overhang test sections.


<img width="960" height="600" alt="f" src="https://github.com/user-attachments/assets/b8481348-bab1-4413-8934-dba4350d3f2b" />


I extruded the rectangular feature outward from the side of the original body.


<img width="960" height="600" alt="g" src="https://github.com/user-attachments/assets/42f99ee9-f55e-471f-a96f-1b597df9d6a6" />


I repeated this process around the other sides of the model until I had eight sections extending from the center. Each section would eventually become one petal of the flower.


<img width="960" height="600" alt="h" src="https://github.com/user-attachments/assets/6ba938c4-8c72-40fb-8d40-80da3fc90d1c" />


### Creating the Overhang Angles

To accurately create the different overhang angles, I created reference datum planes that I could use to make sure each angled cut started at the same position of the petal.


<img width="960" height="600" alt="i" src="https://github.com/user-attachments/assets/27d92482-cf7f-444c-88b3-3c9bcb50ac7c" />


On the reference plane, I sketched a triangular profile. I dimensioned the triangle to the specific overhang angle I wanted that section to test.


<img width="960" height="600" alt="j" src="https://github.com/user-attachments/assets/ca718929-1f78-4176-b914-ae6dbd43dbf8" />


I then used an extrude with **Remove Material** to cut the triangular section away from the model. This created the angled underside that acts as the actual overhang test.


<img width="960" height="600" alt="k" src="https://github.com/user-attachments/assets/e5d81e16-7eba-44fa-be47-2d54fa0df921" />


I repeated the same process around the model while changing the angle for each section.

### Labels and Flower Shape

After creating the different angles, I added the corresponding degree value to the top of each section. This makes it easy to identify which overhang angle I am inspecting after the artifact is printed.


<img width="960" height="600" alt="l" src="https://github.com/user-attachments/assets/9f56eab1-d733-4ece-92b4-304646efa7b9" />


I then used the **Round** tool on the outer edges of the sections. Rounding these edges changed the rectangular sections into shapes that looked more like flower petals while still preserving the overhang geometry underneath.


<img width="960" height="600" alt="m" src="https://github.com/user-attachments/assets/dd3b5a4c-ec35-4fed-b1a3-69c0ad4b1214" />


While checking the finished labels, I noticed that the **20° label was not positioned correctly**. I went back into the model and corrected its placement so the printed artifact would clearly identify the correct angle.


<img width="960" height="600" alt="n" src="https://github.com/user-attachments/assets/9cd3171a-51b4-4c88-92d4-9a97355e1573" />


Finally, I added a circular feature in the center to complete the flower appearance. The finished artifact contains eight labeled petals testing **0°, 20°, 30°, 40°, 45°, 50°, 60°, and 70°**.


<img width="960" height="600" alt="o" src="https://github.com/user-attachments/assets/a5d42dbe-071c-40d5-b83b-e5d3acabd3e2" />


## Preprocessor

After completing the CAD model, I exported the model and opened it in **PrusaSlicer** to prepare it for the Prusa CORE One.

### Supports

I turned **support material off** because the purpose of this experiment is to determine how well the printer can produce unsupported overhangs. Using supports would interfere with the parameter I am testing and would prevent me from accurately determining the printer's overhang limit.


<img width="960" height="600" alt="p" src="https://github.com/user-attachments/assets/e596388e-16a0-4dca-b4ea-eb95c3e63100" />


### Infill, Material, and Printer

I used **Generic PLA** and selected the **Prusa CORE One HF0.4 nozzle** printer profile. I set the infill to **20%** because strength is not the parameter being tested. Twenty percent infill provides enough internal structure for the artifact while keeping the material usage and print time relatively low.

I also used the **0.20 mm BALANCED** print setting.

The model was scaled uniformly to **162.68%**, giving it a final size of approximately **50 mm × 50.07 mm × 24.4 mm**.


<img width="960" height="600" alt="q" src="https://github.com/user-attachments/assets/585cf313-a7ec-4566-81d1-5f012536d0e1" />


### Slicing

After confirming the settings, I sliced the model and reviewed the layer preview. The estimated printing time was approximately **37 minutes**, which is below the one-hour maximum allowed for this assignment.

The sliced model required approximately:

- **13.74 g of filament**
- **4.61 m of filament**
- **37 minutes of estimated print time**

The final preview also allowed me to check that the individual overhang sections and labels were being generated correctly before printing.


<img width="960" height="600" alt="r" src="https://github.com/user-attachments/assets/98a325df-8c6c-4e49-a97c-04f03fd13a76" />


## Print Artifact

I printed the final flower overhang benchmark on **Printer 7** using the Prusa CORE One.

I printed the artifact by itself because I completed the design close to the deadline rather than coordinating a shared print with another student.

The completed artifact is designed to show how print quality changes as the unsupported overhang angle increases. Since all eight angles are located on the same artifact, they are printed using the same material, printer, layer settings, orientation, and environmental conditions. This makes it easier to directly compare the effect of overhang angle.

...

### Print Video

...
