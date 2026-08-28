# L2 – Individual Research: DfAM

## Research independently

**_Find one design rule or guideline specific to Design for Additive Manufacturing. In your own words, write two to three sentences: what the rule is and why it matters. Note your source._**

>**Design Rule – 45° Overhang Rule**
>
>When designing a part for additive manufacturing, overhangs should generally be kept at 45° or greater from the build plate when possible. This helps the part support itself while printing and reduces the need for extra support material, which saves material and makes post-processing easier.
>
>**Source:** Autodesk, *Additive FFF and SLA Technologies – Design Considerations for Additive Manufacturing*.

**_Find one FDM specific consideration. This could be overhangs, bridging, layer adhesion, warping, supports, or infill strategy. In your own words, write two to three sentences: what it is and how a designer works around it. Note your source_**

>**FDM Consideration – Warping**
>
>Warping can happen during FDM printing when the plastic cools unevenly and causes the edges of the part to lift off the build plate. Designers can help prevent this by avoiding large flat areas when possible, using rounded corners, and making sure the part has good contact with the build plate.
>
>**Source:** Prusa Research, *Warping*.

## Small Group Share Out
**_In groups of 3 to 4, explain your DfAM finding and your FDM finding to your group. Use your own words rather than reading your notes directly. Listen to your teammates' findings as well._**
>One of my teammates also researched warping and taught me that keeping the build plate clean can help with adhesion. Better adhesion helps keep the part from lifting off the build plate during printing, which can reduce warping.


## Make Something Small – 3D Printing

For the second part of this lab, I went through the process of finding a small model online, preparing it in PrusaSlicer, and then 3D printing it using one of the FDM printers in the Rapid Prototyping Lab. I chose a small cherry keychain for my print.

### Download

I started by looking through [Printables](https://www.printables.com/) for something small that I liked and that would also meet the requirements for the assignment. The print had to be no larger than 2 in × 2 in, less than 0.25 in tall, have a flat surface to build on, use PLA, and take less than 1.5 hours to print.

<img width="469" height="458" alt="image" src="https://github.com/user-attachments/assets/f488c61d-5f86-4688-8cec-f7f6ce45afe2" />

I looked at a few different designs before choosing the cherry. I wanted something cute and simple that I would actually want to keep, but I also had to consider whether the design would work well as a small FDM print.

#### Other Designs I Considered

Before choosing my final design, I looked at a few different options on Printables. I wanted something cute and small, but I also needed to consider the size requirements, print time, and how easily each design could be printed.

##### Low Poly Heart Keychain

<img width="120" height="120" alt="image" src="https://github.com/user-attachments/assets/2b5a69c6-7d59-4845-b813-2742eddf4176" />

One design I considered was the Low Poly Heart Keychain. I liked this design because it was small, simple, and had a flat surface that seemed like it would print well. However, I decided not to choose it because it had more dimension than I wanted, and I was not completely sure if the angled sides would require supports. Since I wanted to keep the print as simple as possible, I decided not to take the chance.

**Model:** [Low Poly Heart Keychain](https://www.printables.com/model/550636-low-poly-heart-keychain)

##### Cherry Keychain

<img width="90" height="120" alt="image" src="https://github.com/user-attachments/assets/a8ccd1b7-02b0-4ad0-8053-e38353d5fbc1" />

I also considered the Cherry Keychain. I liked the design because it was cute and both pieces had flat bottoms that could sit directly on the build plate. However, I decided not to use this one because having two separate pieces would have made the printing process a little more complicated and would have taken longer to print.

**Model:** [Cherry Keychain](https://www.printables.com/model/1538971-cherry-keychain)

#### Final Choice

<img width="128" height="72" alt="image" src="https://github.com/user-attachments/assets/4074f62f-8381-41bb-af43-b3ea293cb7b3" />

I ended up choosing a **cherry keychain**. I liked the design, and its mostly flat shape seemed like a good option for this assignment. After deciding on the cherry, I downloaded the STL file and opened it in PrusaSlicer.

**Model Source:** [Cherry Keychain on Printables](PASTE-LINK-HERE)

---

### Preprocessor

I imported the cherry STL into **PrusaSlicer** and selected the **Prusa CORE One with a 0.4 mm nozzle** as the printer. I also made sure that **Generic PLA** was selected because PLA was required for the assignment.

<img width="955" height="530" alt="image" src="https://github.com/user-attachments/assets/87565fe1-55df-4a25-93c2-a8b42a1283c8" />

#### Build Orientation

I kept the cherry flat against the build plate because it had a large, flat bottom surface. This gave the model good contact with the build plate and allowed it to print without needing additional supports. Keeping it flat also kept the overall height of the print low.

#### Scaling

The original model was too large for the assignment, so I had to scale it down in PrusaSlicer. I used uniform scaling so that the proportions of the cherry would stay the same.

<img width="959" height="529" alt="image" src="https://github.com/user-attachments/assets/690d02f0-16af-4351-839c-d507ce7cdf94" />

My final dimensions were:

- **X:** 39.15 mm
- **Y:** 50.8 mm
- **Z:** 1.9 mm
- **Scale:** 3.85%

The maximum dimensions for the assignment were 50.8 mm × 50.8 mm × 6.35 mm, so my scaled model met the requirements. The largest dimension was exactly 50.8 mm, or 2 inches.

#### Supports and Print Settings

I did not add any support enforcers because the cherry was able to lie flat on the build plate and did not have any major unsupported sections.

The settings I used were:

- **Printer:** Prusa CORE One HF
- **Nozzle:** 0.4 mm
- **Filament:** Generic PLA
- **Print Setting:** 0.20 mm BALANCED
- **Layer Height:** 0.20 mm
- **Infill:** 15%
- **Supports:** No support enforcers added
- **Brim:** No

When I sliced my cherry by itself, PrusaSlicer estimated a print time of approximately **4 minutes** and a filament use of **1.78 g**.

<img width="956" height="565" alt="lab2slice" src="https://github.com/user-attachments/assets/a314ce1e-a373-43de-817e-e00ff390d8b4" />


#### Printing With a Partner

Since there were a limited number of printers available, I shared a build plate with **Candy Vasquez**. We added both of our models to the same plate and made sure there was enough space between them.

<img width="958" height="567" alt="Screenshot 2026-08-27 143248" src="https://github.com/user-attachments/assets/2f39c1e9-5a89-4dc9-91d9-9a772807a1a5" />

After both models were added and sliced, PrusaSlicer estimated a total print time of approximately **13 minutes** and a combined filament use of **4.62 g**.

#### Adjustments and Mistakes

The biggest adjustment I made during this process was scaling the cherry down to fit within the assignment requirements. At the time, I was mainly paying attention to the overall X, Y, and Z dimensions. After seeing the finished print, I realized that scaling a model down also makes all of its smaller details much smaller.

This became important with the key-ring loop at the top of my cherry. Even though the overall model fit within the required dimensions, the loop became very thin after scaling.

---

### Print

I printed my cherry with **Candy Vasquez** using **Printer #07** in the Rapid Prototyping Lab.

Before starting the print, we made sure that our models were positioned correctly, the correct G-code was selected, and PLA was being used.

Once the print started, I watched the first layers to make sure the filament was sticking to the build plate correctly. I learned earlier during our group discussion that keeping the build plate clean can help improve adhesion, so seeing the first layers form correctly helped confirm that the print had started successfully.

I continued checking the print as it progressed to make sure both models remained attached to the build plate.

<img width="275" height="406" alt="image" src="https://github.com/user-attachments/assets/fd42e0cd-71af-409d-9df4-8a0186cab419" />

I also recorded approximately 15 seconds of the printing process.

[Watch the Printing Process](https://github.com/KaileighAnn/kaileigh-hill-lab-portfolio/blob/main/docs/Lab2.mp4) 

#### Finished Product

After the print finished, I removed my cherry from the build plate and looked over the finished part.

<img width="220" height="293" alt="Finished cherry print" src="https://github.com/user-attachments/assets/e6c7cc8d-d2e7-4cd1-8f17-d00f92084267" /> <img width="220" height="293" alt="Finished cherry print" src="https://github.com/user-attachments/assets/cd4281ad-63f5-4c39-976b-dbc17a004353" /> <img width="220" height="293" alt="Finished cherry print" src="https://github.com/user-attachments/assets/7fcec247-47be-4a9b-9efc-6ad5006ffc73" />


Overall, I was happy with how the main part of the cherry turned out. The larger sections printed fairly cleanly and the details of the cherry were still visible.

The main problem I noticed was the small loop at the top where a key ring would attach.

<img width="300" height="400" alt="Key-ring loop detail" src="https://github.com/user-attachments/assets/aaa0533f-31cb-4ef0-a36a-5691076c20d5" />

The loop did not print as cleanly as the rest of the model. Some of the filament around it was uneven and there were a few loose strands. I think scaling the model down contributed to this because the loop became much thinner than it was in the original model. The small size and curved geometry of the loop may have made it harder for the printer to reproduce accurately.

---

### Lessons Learned

This activity helped me better understand the entire process of 3D printing, from choosing a model to seeing how my decisions in PrusaSlicer affected the final part.

#### 1. Model Selection Matters

I learned that I cannot choose a model based only on how it looks. I also need to consider its size, shape, small features, overhangs, and how easily it can be placed flat on the build plate.

#### 2. Scaling Can Affect Small Details

I had to scale my cherry down significantly to meet the 2-inch size requirement. Although the overall model still looked good, the key-ring loop became very small and did not print as cleanly as the larger parts of the cherry.

#### 3. Build Orientation Makes a Difference

Keeping the largest flat surface of the cherry against the build plate gave it a good base and allowed me to print it without adding supports. This also helped keep the print simple and reduced unnecessary material.

#### 4. The Slicer Preview Is Important

PrusaSlicer gave me the chance to check the dimensions, estimated print time, filament use, and individual layers before printing. If I did this print again, I would pay more attention to the layer preview around very small features like the key-ring loop instead of focusing mainly on the overall dimensions.

#### What I Would Change

If I printed this cherry again, I would try to improve the key-ring loop. I would either make the loop thicker or choose a similar design with a larger loop so that it would still be strong enough after scaling.

I would also consider trying a smaller layer height to see if it improved the detail around the curved loop. Most importantly, I would look more closely at how scaling affects the smallest features before deciding that a model is ready to print.

#### Time Spent

From searching for a model on Printables to finishing the physical print, the entire process took approximately **57 minutes**.

- Searching for and choosing a model: **20 minutes**
- Downloading and preparing the STL: **5 minutes**
- Scaling and slicing in PrusaSlicer: **5 minutes**
- Setting up the printer: **10 minutes**
- Actual printing: **17 minutes**
  
I would also like to recognize **Candy Vasquez** for working with me to put both of our models on the same build plate and complete the printing process.

---

### Resources

- [Printables](https://www.printables.com/) – Used to find and download the cherry STL file.
- [Cherry Keychain Model](https://www.printables.com/model/1656765-cherry-keychain-for-ams/files) – Original model used for my print.
- [PrusaSlicer](https://www.prusa3d.com/page/prusaslicer_424/) – Used to scale, arrange, and slice the model into G-code.
- UNC Charlotte Rapid Prototyping Lab – FDM printer and PLA used to manufacture the part.
