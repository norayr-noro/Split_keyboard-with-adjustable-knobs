# ⌨️ Split Keyboard Project
Building a split keyboard might sound a bit difficult for a beginner, mostly because of how much you'd learn,and thats why i think its a good project to start of with! Im building this slit keyboard mostly because the project uses pcb designing, schematic building and even cad modelling  all in one!Might sound like a lot but thats why i thought this project is ideal for a begginer.
---
## Components
Here I'll put down all the components I will likely use in the full project (most of this is subject to change):
* **56 × Cherry MX switches** 
* **56 × 1N5819 diodes**
* **2 × Raspberry Pi Pico** 
* **2 × EC11E rotary encoders**
* **2 × LiPo batteries** (1000-2000mah)
* **2 × TP4056 charging modules** 
* **Custom-designed PCB**
* **3D printed case + plate** 
* **~8 × M2 screws** 

---
## Libraries
All libraries I used are in the Stasis Hackclub guide(https://stasis.hackclub.com/starter-projects/split-keyboard) + I also used the symbols and footprints for the Raspberry Pi from ScottoKeeb's (I recommend checking him out for anything custom keyboard related!!his YouTube channel is https://www.youtube.com/watch?v=8WXpGTIbxlQ&list=PLBD2IS_t_iWZDMdG_ZF57x9Ebm3kxKqxF&index=3)

## 🧠 Design 

This project started with the Hack Club Stasis guide as a foundation, but i changed a few bits here and there and turned into this project!

One of the biggest changes was switching from the **XIAO nRF52840 (SMD)** to the **Raspberry Pi Pico**. The reason for that is mostly for convinience as i had a few picos lying around, and also more GPIO pins to make a proper keyboard.(more pins = more rows/columbs = more keys)
To manage inputs efficiently, the keyboard uses a **diode + switch matrix**, which:
For the apps used in designing:
* **KiCad** was used to design the schematic and PCB layout
* **Fusion 360** was used to create the keyboard case and plate.

The case surrounding the pcb is literally a square — Mostly because im not good at all in 3d modeling...(but if you at CAD software its a really easy thing!)

---

## ⚙️ Firmware

The keyboard is planned to run on **ZMK firmware**, which offers:
ZMK was chosen mostly because it's quite flexible, especially for custom keyboard builds.
from https://zmk.dev/docs/features/split-keyboards
---

## 📈 Current Progress

So far, the project has reached a final stage of design and im left waiting for the pcb and the print to finish.

---

## 🎯 Goals 

The main motivation behind this project was practicality and learning.

Sinec everything i needed was available this was easy to understand and know what i was doing.


### 🔄 Rotary Encoders

I also added these rotary encoders(one each hand) to control sound and brightness of the screen. These just make the design more fun and uniqe and it would not change a lot of these were not on the pcb
---

## 🚀 Next Steps

Final steps are to fully solder and assemble the PCB, upload the firmware, and wait for the print to finish
---

## 💭 Final Thoughts
This project had its ups and downs, but that didnt stop me from learing how actuall parts are made, from learning kicad and fusion360 to check if my design are actually viable was really hardd.
Even though its not perfect(its not even good tbh) it fell quite fun to learn and build and improve on the project!
Overall quite fun and chaotic, but with an actuall reward at the end.
## Photos of where I'm at now 
<img width="1263" height="709" alt="Screenshot 2026-04-25 164629" src="https://github.com/user-attachments/assets/147caf14-cafe-4e1b-bd39-6e3058d02d10" />


<img width="1366" height="706" alt="Screenshot 2026-04-26 142844" src="https://github.com/user-attachments/assets/b94624c7-36c7-49bc-9fa7-d51baad8dec8" />


Ill also attach the .step file for the PCB and the .f3d file for the 3d model i  have worked on to this repository for future reference...
