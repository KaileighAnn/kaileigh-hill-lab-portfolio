# Lab 4 - Overhang Angle Benchmark

## Parameter

For this lab, I chose to test the **unsupported overhang angle** of the Prusa CORE One. The class FDM design rules list **45°** as the recommended maximum angle that can be printed without supports. I designed one artifact containing several different angles so I could compare their print quality under the same printing conditions.

My flower benchmark tests **20°, 30°, 40°, 45°, 50°, 60°, 70° and 80°** overhangs.

### Prediction

Before printing, I predict that the Prusa CORE One will successfully print unsupported overhangs through approximately **75°**. Prusa states that the CORE One's Nextruder and 360° cooling allow it to print unsupported overhangs up to 75°. Because of this, I expect the **80° overhang to show the most noticeable decrease in surface quality or begin to fail**.

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


<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/d8725192-3858-47c1-9c15-ab8550c57d92" />


Finally, I added a circular feature in the center to complete the flower appearance. The finished artifact contains eight labeled petals testing **20°, 30°, 40°, 45°, 50°, 60°, 70° and 80°**.


<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/8f21d6ea-401e-4b11-bbcd-0ec150668a05" />


## Preprocessor

After completing the CAD model, I exported the model and opened it in **PrusaSlicer** to prepare it for the Prusa CORE One.

I uniformly scaled the artifact to 162.68% so the individual overhang sections and angle labels would be large enough to print clearly while still keeping the artifact small and the print time below one hour. Uniform scaling preserved the angles being tested.

### Build Orientation

I kept the flower flat in its designed orientation on the build plate. This orientation allowed each petal to print at its intended overhang angle. Rotating the artifact would change how the angled surfaces were built and would affect the accuracy of the overhang test.

### Supports

I turned **support material off** because the purpose of this experiment is to determine how well the printer can produce unsupported overhangs. Using supports would interfere with the parameter I am testing and would prevent me from accurately determining the printer's overhang limit.


<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/04228e87-9c5c-4912-b91c-65652fd49569" />



### Infill, Material, and Printer

I used **Generic PLA** and selected the **Prusa CORE One HF0.4 nozzle** printer profile. I set the infill to **20%** because strength is not the parameter being tested. Twenty percent infill provides enough internal structure for the artifact while keeping the material usage and print time relatively low.

I also used the **0.20 mm BALANCED** print setting.

The model was scaled uniformly to **162.68%**, giving it a final size of approximately **50 mm × 50.07 mm × 24.4 mm**.


<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/a70f27c1-8b40-4dda-8e93-9d7aa2f88602" />

### Mistakes

While checking the model, I noticed that I had incorrectly positioned the 20° label. I went back into the CAD model and corrected its location before exporting the final design. Checking the model before slicing helped me catch the mistake before printing.

<img width="578" height="600" alt="yay" src="https://github.com/user-attachments/assets/e18439bd-8b69-46ae-99f2-4d0c7190f2f9" />


### Slicing

After confirming the settings, I sliced the model and reviewed the layer preview. The estimated printing time was approximately **36 minutes**, which is below the one-hour maximum allowed for this assignment.

The sliced model required approximately:

- **12.66 g of filament**
- **4.25 m of filament**
- **36 minutes of estimated print time**

The final preview also allowed me to check that the individual overhang sections and labels were being generated correctly before printing.


<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/3a7629aa-2b2c-4b74-8fbb-6a7243040c05" />



## Print Artifact

I printed the final flower overhang benchmark on **Printer 7** using the Prusa CORE One.

I printed the artifact by itself because I completed the design close to the deadline rather than coordinating a shared print with another student.

The completed artifact is designed to show how print quality changes as the unsupported overhang angle increases. Since all eight angles are located on the same artifact, they are printed using the same material, printer, layer settings, orientation, and environmental conditions. This makes it easier to directly compare the effect of overhang angle.

## Final Print Review

My final print kept its flower shape, and all eight petals remained intact. The angle labels are visible on the top, making it easier to identify each test section.

The underside shows differences in print quality. Some sections look smooth, while others have noticeable ridges, sagging, and loose filament. This shows why inspecting the underside is important when evaluating unsupported overhangs. A completed petal does not necessarily mean it printed with acceptable surface quality.

### Final Design Photos

<p align="center">
  <img width="32%" alt="Final print top view" src="https://github.com/user-attachments/assets/8ccf4256-f3ba-4dd0-9073-036c0b8d48ed" />
  <img width="32%" alt="Final print underside view" src="https://github.com/user-attachments/assets/391955a8-ea79-4d5b-adae-235b70cecb02" />
  <img width="32%" alt="Final print side view" src="https://github.com/user-attachments/assets/433d37dd-a6c5-4051-9fbb-dfb4c6eadd93" />
</p>

- **Top view:** Shows the completed flower and angle labels.
- **Underside view:** Shows differences in surface quality between the overhangs.
- **Side view:** Shows the angled surfaces and visible drooping.

## Results

I considered an overhang acceptable if its underside maintained its intended shape without obvious sagging, gaps, or loose strands.

- **First angle with noticeable surface defects:** 60°
- **Largest angle with acceptable surface quality:** between 60° and 70°
- **Angle with the poorest surface quality:** 80°

## Comparison to My Prediction

Before printing, I predicted acceptable results through approximately 45°–50°, with more noticeable defects around 70°–80°.

The largest acceptable angle in my test was 60°, which was higher than my predicted limit of 45°–50°. The printer handled a larger unsupported overhang than I expected while maintaining acceptable surface quality.

## Lessons Learned

### 1. Predicted vs. Actual Performance

I predicted acceptable unsupported overhangs through approximately 75°, but 60° was the largest tested angle that met my surface-quality criteria. All eight petals finished printing, but completing the print did not mean every overhang had acceptable quality.

### 2. Comparison to the Class Design Rule

My largest acceptable tested angle of 60° exceeded the class FDM guideline of 45° by 15°. This shows that the 45° guideline was conservative for this artifact and these printing conditions. The printer's cooling may have helped the overhangs maintain their shape, but this test did not isolate cooling as a variable.

### 3. Inspecting the Underside

The top surfaces looked more consistent than the undersides. Inspecting only the top would have hidden sagging and loose filament beneath the petals. In a future test, I would photograph each underside with its angle label visible and use the same surface-quality criteria for every section.

### 4. Improving the Test Resolution

The gap between 60° and 70° prevented me from identifying the exact point where quality became unacceptable. I would add 62°, 64°, 66°, and 68° sections in a future design to narrow down the acceptable overhang limit. I would also focuse less on the little angle like 20-40 because they are kind of irrelevant. 

### 5. Checking Labels Before Printing

I initially positioned the 20° label incorrectly and corrected it before exporting the model. This reinforced the importance of checking that every label matches its test surface. In the future, I would inspect all labels in CAD and in the sliced preview before starting the print because they are all visible but not as aesthetically pleasing as I would have liked them to be. 

## Conclusion

The flower benchmark allowed me to compare eight unsupported overhang angles in one print. Under my printing conditions, 60° was the largest angle that met my surface-quality criteria. For similar prints, I would use this result when deciding whether to change the orientation or add supports.

## Time Spent

| Task | Time |
|---|---|
| Design and CAD | Approximately 1 hour |
| Slicing and printer setup | Approximately 15 minutes |
| Printing | 42 minutes 42 seconds |
| Inspection and documentation | Estimated 1 hour |
| **Total** | **Approximately 2 hours 58 minutes** |

### Print Video

<video autoplay loop muted playsinline style="width: 100%; max-width: 500px;">
  <source src="IMG_0997.mp4" type="video/mp4">
</video>

## Resources

### 1. Class Design Rules for 3D Printing

I used the **Design Rules for 3D Printing** provided in class as a reference for my experiment. The FDM design rules list **45° as the recommended maximum unsupported overhang angle**. I used this as the general FDM design rule to compare to the results from the Prusa CORE One.

### 2. Prusa Research - Modeling with 3D Printing in Mind

I used Prusa Research's official documentation to research the expected overhang capabilities of the Prusa CORE One. Prusa states that its FDM printers with the Nextruder and 360° cooling, including the CORE One, can print unsupported overhangs of **up to 75°**.

Based on this information, I predict that the Prusa CORE One will successfully print overhangs through 75° and that print quality will begin to fail or significantly decrease at angles greater than 75°.

[Prusa Research - Modeling with 3D Printing in Mind](https://help.prusa3d.com/article/modeling-with-3d-printing-in-mind_164135?product=core-one-plus)

### 3. Prusa Research - Failing Supports

I also used Prusa Research's information about supports and overhangs. Prusa explains that support material is commonly used for large or highly sloped overhangs and that PrusaSlicer allows the overhang threshold to be adjusted. This helped support my decision to turn supports off so that I could test the actual unsupported overhang capability of the printer.

[Prusa Research - Failing Supports](https://help.prusa3d.com/article/failing-supports_1807)
