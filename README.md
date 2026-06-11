# ⌨️ Split Keyboard Project
Making your own keyboard sounds difficult, but it really isn't! And this repo is proof of that. As a beginner in the field of CAD and PCB design, this is an ideal project to make because it combines areas like PCB and CAD modeling, and in this repo, I'll be writing on how I built it following the guide on hackclub stasis!

<img width="667" height="293" alt="image" src="https://github.com/user-attachments/assets/5c00ea47-3108-4733-822d-e85a52db5863" />



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
Because I used the hackclbu split keyboard tutorial as a foundation, one of the biggest changes was switching from the XIAO nRF52840 (SMD) to the Raspberry Pi Pico. The reason for that is mostly for convenience, as I had a few picos lying around and also more GPIO pins to make a proper keyboard.(more pins = more rows/columbs = more keys), And with the diode+switch matrix would make an ideal build.

---

### 🔄 Rotary Encoders

I also added these rotary encoders(one in each hand) to control the sound and brightness of the screen. These just make the design more fun and unique, and it would not change a lot if these were not on the PCB, so feel free to change stuff around!

---

## UPDATES
 Changed the full design of the PCB to make it as slim as possible (could've done better tbh) to lower the cost of manufacturing the PCB + the fact it would look like a cleaner and nicer build in general. After that, I shifted the Pico W upwards (all the wayyyyyy to the edge) for easier access to the USB port and simpler routing and debugging
Continuing with those changes, I moved on to the CAD models, changed the case and plate to fit the new PCB, and mostly did some polishing for where the USB-C would go and where the slide switch should go. 



## Photos of where I'm at now 

<img width="1085" height="631" alt="Screenshot 2026-04-26 144541" src="https://github.com/user-attachments/assets/a0ead9a9-d804-4c69-912b-7f038c43af21" />
<img width="1001" height="378" alt="image" src="https://github.com/user-attachments/assets/e13ece1f-1b0f-429e-b3a0-ce0bbfd60b19" />
<img width="1066" height="473" alt="image" src="https://github.com/user-attachments/assets/2b1b3858-2901-4fab-ae89-3659396544f3" />

<img width="827" height="377" alt="CAD_plate" src="https://github.com/user-attachments/assets/71a01d38-9771-4966-bffd-ae04b6f5317b" />
<img width="782" height="462" alt="CAD_final" src="https://github.com/user-attachments/assets/e449bb22-ccc8-4305-b3a7-bd4967e20e17" />


I'll also attach the .step file for the PCB and the .f3d file for the 3d model i  have worked on to this repository for future reference...
