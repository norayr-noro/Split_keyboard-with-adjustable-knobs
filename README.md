# ⌨️ Split Keyboard Project
Building a split keyboard might sound a bit difficult for a beginner, mostly because of how much you'd learn,and thats why i think its a good project to start of with! Im building this slit keyboard mostly because the project uses pcb designing, schematic building and even cad modelling  all in one!Might sound like a lot but thats why i thought this project is ideal for a begginer.
---
## Components

* **56 × Cherry MX switches** — reliable, widely used mechanical switches
* **56 × 1N5819 diodes** — used in the switch matrix to prevent ghosting
* **2 × Raspberry Pi Pico** — dual microcontroller setup for each half
* **2 × EC11E rotary encoders** (20mm D-shaft preferred)
* **2 × LiPo batteries** — planned for portable power
* **2 × TP4056 charging modules** — for battery charging and management
* **Custom-designed PCB**
* **3D printed case** (designed in Fusion 360)
* **~8 × M2 screws** (subject to change as the design evolves)

---
## Libraries
All libraries i used are in the Stasis Hackclub guide(https://stasis.hackclub.com/starter-projects/split-keyboard) + I also used the symbols and footprints for the Raspberry Pi from ScottoKeeb's (i recommend checking him out for anything custom keyboard related!!his youtube channel is https://www.youtube.com/watch?v=8WXpGTIbxlQ&list=PLBD2IS_t_iWZDMdG_ZF57x9Ebm3kxKqxF&index=3)

## 🧠 Design 

This project started with the Hack Club Stasis guide as a foundation, but quickly evolved with several personal modifications and decisions.

One of the biggest changes was switching from the **XIAO nRF52840 (SMD)** to the **Raspberry Pi Pico**. This decision was mainly driven by:

* Easier handling (especially compared to SMD components)
* Greater availability
* More accessible GPIO pins for expansion and flexibility

To manage inputs efficiently, the keyboard uses a **diode + switch matrix**, which:

* Reduces the number of required GPIO pins
* Improves performance
* Simplifies wiring and scalability

For design tools:

* **KiCad** was used to design the schematic and PCB layout
* **Fusion 360** was used to create the keyboard case and overall structure

The case design is relatively simple due to the square nature of the PCB, which limits more advanced shaping — Mostly because im not good at all in 3d modeling...

---

## ⚙️ Firmware

The keyboard is planned to run on **ZMK firmware**, which offers:
ZMK was chosen mostly because it's quite flexible, especially for custom keyboard builds.
from https://zmk.dev/docs/features/split-keyboards
---

## 📈 Current Progress

So far, the project has reached an advanced design stage:

* ✅ Schematic fully designed in KiCad
* ✅ PCB layout completed and routed
* ✅ 3D case modeled in Fusion 360

At this point, the project is largely designed and ready for refinement, prototyping, and physical assembly.

---

## 🎯 Goals 

The main motivation behind this project was practicality and learning.

Since most of the required components were already available, it made sense to start building immediately rather than waiting or over-planning. This allowed for faster iteration and more hands-on experience.

Key goals include:

* Developing real-world PCB design skills
* Learning CAD and mechanical design through Fusion 360
* Understanding how hardware and firmware integrate
* Building a fully functional and personalized keyboard

---

## ✨ Features

* Split ergonomic keyboard layout
* Fully custom PCB design
* Dual microcontroller architecture
* Expandable and modifiable design

### 🔄 Rotary Encoders

* One encoder dedicated to **volume control**
* One encoder dedicated to **brightness adjustment**

These add an extra layer of interactivity beyond standard key input.

---

## 🚀 Next Steps

* Final PCB polishing and validation
* Refinement of the 3D printed case
* Firmware setup and configuration (ZMK)
* Physical assembly and testing
* Iteration based on performance and usability

---

## 💭 Final Thoughts

This project has been a mix of challenges and progress — from learning new tools like KiCad and Fusion 360, to troubleshooting design decisions along the way.
While not everything is perfect (and some parts are intentionally simple), the focus for me has always been  on learning, building, and improving. Every step adds more understanding, making future iterations even better.
Overall, a fun, slightly chaotic, but very rewarding build.
## Photos of where I'm at now 
<img width="1263" height="709" alt="Screenshot 2026-04-25 164629" src="https://github.com/user-attachments/assets/147caf14-cafe-4e1b-bd39-6e3058d02d10" />


<img width="1366" height="706" alt="Screenshot 2026-04-26 142844" src="https://github.com/user-attachments/assets/b94624c7-36c7-49bc-9fa7-d51baad8dec8" />


Ill also attach the .step file for the PCB and the .f3d file for the 3d model i  have worked on to this repository for future reference...
