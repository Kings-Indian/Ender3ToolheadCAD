# Ender3Toolhead Development Journal

**Total Time Spent: 26 hours**

---
title: "Ender3Toolhead"
author: "Tanishq"
description: "This is a toolhead designed around an ender 3"
created_at: "2025-05-28"
---
## I Decided the Scope of My Project

- It will be on a 300 mm Stainless Steel MGN12H Linear Guide. Linear rails are stiffer, more precise, and simpler to mount than linear rods, reducing backlash and ringing artifacts in 3D printing. Unlike rods, a single rail can achieve linear motion without rotation, making setups lighter.
- It will rely on direct drive extrusion. This is due to its more consistent extrusion and lack of slipping.
  - **2a.** It will contain dual gear extrusion. This is due to its lack of slippage.
  - **2b.** It will most likely be based around the ProtoXTruder but modified to have the advantage of a Sherpa Mini's dual gear. Other extruders like the Orbiter were considered, but due to price and difficulty in manufacturing (I plan to print it, and the planetary may be difficult to make and expensive with bought parts) aren't likely to be used.
- Cooling will likely have a 2510 fan on the hotend and two 5015s on the nozzle.
- The Hot End will most likely be a Dragon Hotend UHF due to its impressive flow rate of 70.5 mm³/s.

### **May 28, 2025** - 1 hour spent
### **June 29-30, 2025** - So I forgot to commit so everything got delelted but heres a rundown opf the p[ast few days:

1. Im using a lancer long with a  CHT Volcano Nozzle. <img width="610" height="696" alt="image" src="https://github.com/user-attachments/assets/e57756fc-0448-4793-b0b8-577a360abb73" /> <img width="1075" height="784" alt="image" src="https://github.com/user-attachments/assets/e2f5b49b-0e2d-49c0-a956-1b319651f213" />
<img width="1336" height="835" alt="image" src="https://github.com/user-attachments/assets/ebbeb340-757d-4472-baf6-72e448dad283" />
<img width="1126" height="992" alt="image" src="https://github.com/user-attachments/assets/21db17d4-3e95-42b1-829f-5475136b276b" />
for the cooling ill use a 3010 fan on the hotend and a cpap fan on the tip

<img width="489" height="534" alt="image" src="https://github.com/user-attachments/assets/d382d9d3-a37c-49b7-9207-eb12ab044933" />
**Time spent**: 10 hours 

### **June 31, 2025**:

I decided the following changes:

1. I will add a skr mini e3v3board to make it quiter and improve performance. I also need it for the Independent Fan Control
2. Ill switch out the CR touch with a btt microprobe, a mroe accurate touch probe
3. I will add a ebb36 board
4. I will route the cpap fan bettter by making it on the back and using vzbot ducts

ill start by designing the beginnings and ends of the ducts. I will then likely connect them, put the ebb36 board below the belt tensioner, and then but a microprobe on the front middle. 
<img width="875" height="705" alt="image" src="https://github.com/user-attachments/assets/77fea19e-3fb0-431f-8291-c543cf931968" />

<img width="688" height="607" alt="image" src="https://github.com/user-attachments/assets/ce2f3741-420c-4e0a-beb5-9a8823702816" />

optimally I have the same volume as the input all the way/2 since I split it. 9.5^2*pi/2=#ductz* the y length. <img width="402" height="362" alt="image" src="https://github.com/user-attachments/assets/4fd5f913-8032-48b3-aa5b-562dce246fcb" />

**Time spent**: 3.5 hours
<img width="686" height="604" alt="image" src="https://github.com/user-attachments/assets/f45b26ce-ff07-4d07-9c5f-fd03dfe04cef" />
Having a lot of t rouble with lofts 😭this is the best I got it
**Time spent**: 5 hours

### **July 25, 2025**
After a bajllion iterations this is what I made 😭
<img width="1002" height="549" alt="image" src="https://github.com/user-attachments/assets/f7211e40-4738-4038-b326-9f7a8fb3b2e7" />
**Time spent**: 6 hours

### **July 26, 2025**
Ill att the BTT Microprobe now 
<img width="1792" height="845" alt="image" src="https://github.com/user-attachments/assets/b3bf0840-8d18-442f-b212-3545e2611e52" />
<img width="2041" height="1062" alt="image" src="https://github.com/user-attachments/assets/d57db7a5-277a-4c2a-8294-0325918921b6" />

Maximum length - range/2=
28.70000-2mm-26.7 

### **July 28, 2025**

I cleaned up everything :) 

Final assembly:

<img width="914" height="1092" alt="image" src="https://github.com/user-attachments/assets/6da7b77f-af21-4b13-a57d-4405525b0bbb" />
<img width="910" height="840" alt="image" src="https://github.com/user-attachments/assets/d00a86af-5ecb-4086-ad92-66310683a2c7" />
Cpap fan mount:
<img width="910" height="840" alt="image" src="https://github.com/user-attachments/assets/244d11f5-6b42-495b-b590-fa4d7b654d85" />
<img width="918" height="831" alt="image" src="https://github.com/user-attachments/assets/21010d5c-06ff-4260-bc57-a8f18eaed4ad" />

mounted:

<img width="549" height="789" alt="image" src="https://github.com/user-attachments/assets/3ceb7409-bdbd-4550-a30b-d53acaf30d4a" />

### **July 29, 2025**
Ill also add a btt skr mini e3 v3.0. I actually cadded this in not expecting this too fit in the default Ender 3 case obviously since its a different board. Not only do the cable holes allign perfectly, the mounting holes even fit the board
<img width="667" height="1029" alt="image" src="https://github.com/user-attachments/assets/19e2318e-bcae-47a0-b229-161b97197638" />
<img width="1191" height="700" alt="image" src="https://github.com/user-attachments/assets/b4dfa217-081c-4b1a-b2eb-b2b9d713f352" />
I honestly cant find a single improvement I can do with a new case. 
(I also decided not to add that board because I heard the heat of a toolhead damages it heavily)

**Time spent**: 0.5 hours

