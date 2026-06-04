# ⌨️ Split Keyboard Project
Building a split keyboard might sound a bit difficult for a beginner, mostly because of how much you'd learn, and that's why i think its a good project to start of with! Im building this slit keyboard mostly because the project uses pcb designing, schematic building and even cad modelling  all in one! Might sound like a lot, but that's why I thought this project is ideal for a beginner.

<img width="670" height="285" alt="Screenshot 2026-06-04 205529" src="https://github.com/user-attachments/assets/dac62670-7257-45a9-ab61-4fdbf0fc2a43" />


---
## Components
Here I'll put down all the components I will likely use in the full project:
|ITEM | URL | QUANTITY |PRICE (USD) |
|-------| ------| ---------------| ---------- |
|cherry-mx style switches| https://www.ebay.co.uk/itm/187479375359| 56 | 14.58|
|1N5819 diodes|https://www.rapidonline.com/st-1n5819-schottky-diode-40v-1a-do41-47-2566|56| 5.4| 
|Raspberry Pi Pico W|https://shorturl.at/rgenT|2|15.57|
|EC11E rotary encoders|https://www.adafruit.com/product/377|2|9|
|LiPo batteries (1500mah)	|https://shorturl.at/IHMxN|2|18.79|
|TP4056 modules|https://www.ebay.co.uk/itm/295410567795?var=593544577789|2|3.22|
|SS12D10 slide switches|	https://shorturl.at/kdSMI|2|2.68|


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

The final steps are to fully solder and assemble the PCB, upload the firmware, and wait for the print to finish
---
## UPDATES
 Changed the full design of the PCB to make it as slim as possible (could've done better tbh) to lower the cost of manufacturing the PCB + the fact it would look like a cleaner and nicer build in general. After that, I shifted the Pico W upwards for easier access to the USB port and simpler routing and debugging
Continuing with those changes, I moved on to the CAD models, changed the case and plate to fit the new PCB, and mostly did some polishing for where the USB-C would go. Finally, I added a BOM file(s) of where you could get those parts.


## 💭 Final Thoughts
This project had its ups and downs, but that didnt stop me from learing how actuall parts are made, from learning kicad and fusion360 to check if my design are actually viable was really hardd.
Even though its not perfect(its not even good tbh) it fell quite fun to learn and build and improve on the project!
Overall quite fun and chaotic, but with an actuall reward at the end.
## Photos of where I'm at now 

<img width="1085" height="631" alt="Screenshot 2026-04-26 144541" src="https://github.com/user-attachments/assets/a0ead9a9-d804-4c69-912b-7f038c43af21" />
<img width="1010" height="412" alt="Final_PCB" src="https://github.com/user-attachments/assets/4d89601a-f4e8-4085-8a32-1623c93437ad" />
<img width="1122" height="473" alt="Final_PCB(3d)" src="https://github.com/user-attachments/assets/eff43778-76d4-4d14-9ec9-a07e3a5df0bd" />
<img width="935" height="471" alt="CAD_case" src="https://github.com/user-attachments/assets/f820dc94-6b7d-4d91-877b-2104c5420132" />
<img width="827" height="377" alt="CAD_plate" src="https://github.com/user-attachments/assets/71a01d38-9771-4966-bffd-ae04b6f5317b" />
<img width="782" height="462" alt="CAD_final" src="https://github.com/user-attachments/assets/e449bb22-ccc8-4305-b3a7-bd4967e20e17" />


Ill also attach the .step file for the PCB and the .f3d file for the 3d model i  have worked on to this repository for future reference...
