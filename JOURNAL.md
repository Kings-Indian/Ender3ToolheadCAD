---
title: "Ender3 Toolhead"
author: "Tanishq Goyal"
description: "A custom toolhead designed for the Ender 3 platform."
created_at: "2025-05-28"
---

**Time Spent in Total: 31 hr**

# May 28th: Project Scope Definition

I decided the scope of my project:

- It will be on a 300 mm Stainless Steel MGN12H Linear Guide. Linear rails are stiffer, more precise, and simpler to mount than linear rods, reducing backlash and ringing artifacts in 3D printing. Unlike rods, a single rail can achieve linear motion without rotation, making setups lighter.
- It will rely on direct drive extrusion. This is due to its more consistent extrusion and lack of slipping.
  - **2a.** It will contain dual gear extrusion. This is due to its lack of slippage.
  - **2b.** It will most likely be based around the ProtoXTruder but modified to have the advantage of a Sherpa Mini's dual gear. Other extruders like the Orbiter were considered, but due to price and difficulty in manufacturing (I plan to print it, and the planetary may be difficult to make and expensive with bought parts) aren't likely to be used.
- Cooling will likely have a 2510 fan on the hotend and two 5015s on the nozzle.
- The Hot End will most likely be a Dragon Hotend UHF due to its impressive flow rate of 70.5 mm³/s.

**Total time spent: 1h**

---

# June 29-30th: Component Selection and Initial Design

I'm using a lancer long with a CHT Volcano Nozzle. For the cooling I'll use a 3010 fan on the hotend and a cpap fan on the tip.

![image](https://github.com/user-attachments/assets/e57756fc-0448-4793-b0b8-577a360abb73)
![image](https://github.com/user-attachments/assets/e2f5b49b-0e2d-49c0-a956-1b319651f213)
![image](https://github.com/user-attachments/assets/ebbeb340-757d-4472-baf6-72e448dad283)
![image](https://github.com/user-attachments/assets/21db17d4-3e95-42b1-829f-5475136b276b)
![image](https://github.com/user-attachments/assets/d382d9d3-a37c-49b7-9207-eb12ab044933)

**Total time spent: 10h**

---

# July 21st: Electronics and Control System Design

I decided the following changes:

1. I will add a skr mini e3v3board to make it quiter and improve performance. I also need it for the Independent Fan Control
2. Ill switch out the CR touch with a btt microprobe, a mroe accurate touch probe
3. I will add a ebb36 board
4. I will route the cpap fan bettter by making it on the back and using vzbot ducts

I'll start by designing the beginnings and ends of the ducts. I will then likely connect them, put the ebb36 board below the belt tensioner, and then but a microprobe on the front middle.

![image](https://github.com/user-attachments/assets/77fea19e-3fb0-431f-8291-c543cf931968)
![image](https://github.com/user-attachments/assets/ce2f3741-420c-4e0a-beb5-9a8823702816)

Optimally I have the same volume as the input all the way/2 since I split it. 9.5^2*pi/2=#ductz* the y length.

![image](https://github.com/user-attachments/assets/4fd5f913-8032-48b3-aa5b-562dce246fcb)

**Total time spent: 3.5h**

![image](https://github.com/user-attachments/assets/f45b26ce-ff07-4d07-9c5f-fd03dfe04cef)

Having a lot of trouble with lofts 😭this is the best I got it

**Total time spent: 5h**

---

# July 25th: Duct Design Finalization

After a bajillion iterations this is what I made 😭

![image](https://github.com/user-attachments/assets/f7211e40-4738-4038-b326-9f7a8fb3b2e7)

**Total time spent: 6h**

---

# July 26th: BTT Microprobe Integration

I'll add the BTT Microprobe now.

![image](https://github.com/user-attachments/assets/b3bf0840-8d18-442f-b212-3545e2611e52)
![image](https://github.com/user-attachments/assets/d57db7a5-277a-4c2a-8294-0325918921b6)

Maximum length - range/2= 28.70000-2mm-26.7

**Total time spent: 2h**
---

# July 28th: Final Assembly and Cleanup

I cleaned up everything :)

Final assembly:

![image](https://github.com/user-attachments/assets/6da7b77f-af21-4b13-a57d-4405525b0bbb)
![image](https://github.com/user-attachments/assets/d00a86af-5ecb-4086-ad92-66310683a2c7)

CPAP fan mount:

![image](https://github.com/user-attachments/assets/244d11f5-6b42-495b-b590-fa4d7b654d85)
![image](https://github.com/user-attachments/assets/21010d5c-06ff-4260-bc57-a8f18eaed4ad)

Mounted:

![image](https://github.com/user-attachments/assets/3ceb7409-bdbd-4550-a30b-d53acaf30d4a)

**Total time spent: 3h**

---

# July 29th: Electronics Board Integration

I'll also add a btt skr mini e3 v3.0. I actually CADded this in not expecting this to fit in the default Ender 3 case obviously since its a different board. Not only do the cable holes align perfectly, the mounting holes even fit the board.

![image](https://github.com/user-attachments/assets/19e2318e-bcae-47a0-b229-161b97197638)
![image](https://github.com/user-attachments/assets/b4dfa217-081c-4b1a-b2eb-b2b9d713f352)

I honestly can't find a single improvement I can do with a new case. (I also decided not to add that board because I heard the heat of a toolhead damages it heavily)

**Total time spent: .5 hr**

