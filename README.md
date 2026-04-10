**Schematic design**  
I started designing the schematic in KiCad, and following the tutorial i started with the capacitors on the power line  
<img width="522" height="129" alt="Screenshot 2026-03-16 143728" src="https://github.com/user-attachments/assets/57855e55-be47-4f7c-9d69-6d0033eba444" />

I actually copied the 3v3 capacitor line for 5v too, but then later in the tutorial found out that it was not necessary. I added the usb interface and flash memory, and did some more research to understand the use cases of SPI.  
<img width="233" height="300" alt="Screenshot 2026-03-16 143758" src="https://github.com/user-attachments/assets/ef876516-1c8b-4c8a-ae0d-acde7add0eb8" />

Then I did all the labels and actually removed three to be replaced by a red led(with 50ohm resistor), a blue led(10ohm) and a button connected to 3v3.  
The headers will be shuffled a bit so the pins are all at my preffered optimal places.  
<img width="173" height="147" alt="Screenshot 2026-03-16 143810" src="https://github.com/user-attachments/assets/9c3be6d6-1ee4-4fa5-b4cb-034e0c180082" />

**Sketch Finished**  

**Header Pins**  
I first fixxed the I/O headers to fit what I wanted, I use a lot of servos normally, and when on low power, you can put them on the board, so I though 5v was important. I also made sure tha 3v3 and GND pins were abundant for possibly LEDS, or I2C interfaces.  
<img width="379" height="367" alt="Screenshot 2026-03-24 123425" src="https://github.com/user-attachments/assets/e31810e3-aea9-4d8a-b7f2-d3b651736588" />

**Button**  
I also added a programmable button, because I thought it would be nice to have one:  
<img width="127" height="73" alt="Screenshot 2026-03-24 123841" src="https://github.com/user-attachments/assets/6c1c747c-7563-416a-a3e0-d82c9bdb7d9f" />

**Cleaning**  
I then removed the caps i had on the 5V line, as I saw it wasn't needed. The crystal show 3 pins, but it is the right version, so I will find out if it works later, and added boxes and labels everywhere:  
<img width="533" height="363" alt="Screenshot 2026-03-24 123923" src="https://github.com/user-attachments/assets/e4368306-a78a-4cbd-9770-b73320162847" />

**ERC**  
I ran the ERC to check my schematic, and it passed with just the power pin errors that should be igmored:  
<img width="831" height="489" alt="Screenshot 2026-03-24 124952" src="https://github.com/user-attachments/assets/1da408bc-3289-462b-a38d-ddf74574a53d" />

**Footprint assigments**  
I copied most of the footprints from the turorial, only had to make some small adjustments  
But the LED was a bit more difficult, so i was looking around on JLC but couldn't find what I was looking for exaclty, until I later discovered that the footprint was just the size specification.  
<img width="461" height="435" alt="Screenshot 2026-03-30 100742" src="https://github.com/user-attachments/assets/26135fe2-bc5d-4dba-8bd2-f1d183405ab7" />

**PCB design**  
I started Designing the PCB and also changed some components around, I decided to follow the tutorial on the step-down converter, since I won't be using it for high current applications.  
<img width="772" height="773" alt="Screenshot 2026-03-30 103404" src="https://github.com/user-attachments/assets/b52e2857-7423-4168-ad28-0a63d52becdf" />

After that I started routing which was a pain, it doesn't feel the way it is supposed to so I will have to check out the KiCad settings. I did a few concept configs, I don't have screenshots of those, but here is the start of the routing:  
<img width="1327" height="1137" alt="Screenshot 2026-03-30 111854" src="https://github.com/user-attachments/assets/a8187185-3785-4707-9ef2-efafe29aea59" />

Next I will continue routing and probably do it over 5 times to make usre to not place vias on the pads, which I did on another design that I was about to order, so thanks for that tip hehe.  

**PCB routing**  
PS, this log looks different because I started using a kicad plugin to keep track of time and progress, and this is just copied over with small adjustments.  
I made a Differential pair for usb data routing, at first the flash mem was too close, making the resistors misaligned and everything was screwed, so I redid that and then I did some of that tuning and the differential pair is now good. [2026-04-07 9:45] Added Decoupling caps for step-down and power lines [2026-04-07 10:00] Logoff [2026-04-07 10:19] Logon [2026-04-07 10:45] All components placed, wil commence routing algorithm to see how good it works, just for curiosity. [2026-04-07 11:09] Algorithm took too long, started manual routing [2026-04-07 11:30] Log off [2026-04-07 12:13] Log on [2026-04-07 17:15] Had problems with some of the GPIOs as the chip has them in top to bottom while the pin header has it the other way around, I am going to keep trying to make it work, if not then I will flip the row around. [2026-04-07 17:31]
<img width="692" height="732" alt="image" src="https://github.com/user-attachments/assets/886e0c06-d0a7-4195-89b1-c9a4fcf7ae29" />

I reassigned all the GPIOs, both the right header row and for the button and leds, this should make it easier to route. [2026-04-07 18:03]  
<img width="501" height="624" alt="image" src="https://github.com/user-attachments/assets/cc4b3ed6-285d-4d0b-a5b4-78ca0d4daee6" />

**PCB routing done**  
Started tracing with the reassigned GPIOs, the first part that had to go around the decoupling caps was quite difficult. [2026-04-08 10:30] Finished routing, left all the GND pins, and connected all 3v3's together and vbus pins together too. [2026-04-08 10:48]  
<img width="426" height="929" alt="image" src="https://github.com/user-attachments/assets/13120461-b2b0-42ee-8f18-514639901172" />

I unrounded all the tracks, as I noticed it actually made the differential pair wrong, and I was unable to fix it, so I unrounded everything and retuned the traces. I also discovered that I forgot to combine D- + D- and D+ + D+.[2026-04-08 10:57]  
<img width="468" height="1018" alt="image" src="https://github.com/user-attachments/assets/a3fc407a-70c4-4aa2-8d98-957f131cb78c" />

Logoff [2026-04-08 10:58] Logon [2026-04-08 12:07] Ground fill done, it took a lot of rerouting and vias to connect everything, but it worked out in the end. There was a wierd misalignment between the MCU and the tracks, so I had to lower the spacing, and some plces now have a 0.192 or 0.194 mm spacing instead of 0.2mm, I assessed that this should work out fine as it will be the lower power gpio pins. [2026-04-08 12:28] Ran DRC and got quite the package, of course the minimum spcing that I just mentioned, and then isolated GND islands, but they weren't really isolated. Labled everything, so silkscreen shows every component ID [2026-04-08 12:43]  
<img width="662" height="512" alt="image" src="https://github.com/user-attachments/assets/2daabfdf-7177-4236-a46e-673bb97229b4" />

Connected and reinforced most ground fill parts [2026-04-08 13:00] DRC is as clean as it will get, I am happy, now time for the art and stuff [2026-04-08 13:03] Logoff[2026-04-08 13:38] Logon[2026-04-08 14:52] I spent quite some time getting a nice design, now I got it and will put it on the board, as well as getting BOM and everything next session.  
<img width="662" height="512" alt="image" src="https://github.com/user-attachments/assets/5df2442a-f90f-426b-82d2-416f0eb3e00e" />

**Order ready**  
Fishing up design placement and little ornaments [2026-04-10 08:50]  
I am happy with the design and how the baord looks, I will now get the fabrication outputs done using a plugin that automatically makes it JLCPCB compatible. [2026-04-10 09:01]  
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/4fc4baf5-d6aa-4bef-8dd9-81b7a4085343" />

I had to replace the 14pin connector, because it wasnt availible on JLC, Now I have to slightly change some routing. [2026-04-10 09:25] I did some digging and found out that the crystal oscilator's orientation does not matter as long as the ground pads are on ground, so pin 1 and 3 are interchangeable.  
<img width="317" height="228" alt="image" src="https://github.com/user-attachments/assets/cab317bb-bcfe-4389-b7d4-34efe18922e2" />

I will not do PCBA, because when I looked it was 80AUD because of the parts from extended library. [2026-04-10 10:13]  
I want to get this board and my personal board that is not on hackclub together as it is cheaper to get both:  
<img width="349" height="444" alt="image" src="https://github.com/user-attachments/assets/cee08fa0-c91f-4b89-bd13-09f15a46996d" />
[Just RiftBoard x5]

<img width="358" height="446" alt="image" src="https://github.com/user-attachments/assets/3d5fa777-1e80-4c93-a77b-4384527bddd9" />
[With LilG(personal board) x10 added]

So the total will look like this:
<img width="1289" height="636" alt="image" src="https://github.com/user-attachments/assets/9a44b1a0-fa68-4be9-8826-b5d5c0870be8" />
