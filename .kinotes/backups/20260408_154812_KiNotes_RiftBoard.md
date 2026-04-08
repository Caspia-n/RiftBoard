# **RiftBoard - Design Notes**

## ********************************PCB layout time [2026-04-07 9:40]********************************
I made a Differential pair for usb data routing [2026-04-07 9:45] 
Added Decoupling caps for step-down and power lines [2026-04-07 10:00] 
Logoff [2026-04-07 10:19] 
Logon [2026-04-07 10:45] 
All components placed, wil commence routing algorithm to see how good it works. [2026-04-07 11:09] 
Algorithm took too long, started manual routing [2026-04-07 11:30] 
Log off [2026-04-07 12:13] 
Log on [2026-04-07 17:15] 
Had problems with some of the GPIOs as the chip has them in top to bottom while the pin header has it the other way around, I am going to keep trying to make it work, if not then I will flip the row around. [2026-04-07 17:31] 
I reassigned all the GPIOs, both the right header row and for the button and leds, this should make it easier to route. [2026-04-07 18:03] 

Started tracing with the reassigned GPIOs, the first part that had to go around the decoupling caps was quite difficult. [2026-04-08 10:30]
Finished routing, left all the GND pins, and connected all 3v3's together and vbus pins together too. [2026-04-08 10:48] 


I unrounded all the tracks, as I noticed it actually made the differential pair wrong, and I was unable to fix it, so I unrounded everything and retuned the traces. I also discovered that I forgot to comine D- + D- and D+ + D+.[2026-04-08 10:57] 

Logoff [2026-04-08 10:58] 
Logon [2026-04-08 12:07] 
Ground fill done, it took a lot of rerouting and vias to connect everything, but it worked out in the end. There was a wierd misalignment between the MCU and the tracks, so I had to lower the spacing, and some plces now have a 0.192 or 0.194 mm spacing instead of 0.2mm, I assed that this should work out fine as it will be the lower power gpio pins. [2026-04-08 12:28] 
Ran DRC and got quite the package, of course the minimum spcing that I just mentioned, and then isolated GND islands, but they weren't really isolated.
Labled everything, so silkscreen shows every component ID [2026-04-08 12:43] 
Connected and reinforced most ground fill parts [2026-04-08 13:00] 
DRC is as clean as it will get, I am happy, now time for the art and stuff [2026-04-08 13:03] 
Logoff[2026-04-08 13:38] 
Logon[2026-04-08 14:37] 
Logoof [2026-04-08 15:25] 



