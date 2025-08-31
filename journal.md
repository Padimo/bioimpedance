---
Title: "Bioimpedance"
Author: "Padimo"
Description: "An ESP32S3 dev board with a MAX30001 bioimpedance sensor"
Created On: "8/15/2025"
---

# Day 1 8/15

Added the ESP32S3 WROOM 1 and power management.
![img1](journal/img1.jpg?raw=true)

*time spent: 2h*

# Day 2 8/18

Locked in. Added power management and MAX30001. Adding the MAX30001 power and copying the example schematic took forever.
The MAX30001 datasheet is looooooooong. But it was necessary. 

Tried to route PCB with autorouting but it failed. Shockingly managed to fit everything into a two layer board.

![img2](journal/img2.jpg?raw=true)
![img3](journal/img3.jpg?raw=true)

*time spent: 8h*

# Day 3 8/19

Got a review. Since MAX30001 is analog, I need to remove traces from under the chip (except ones that actually come from under the chip.
I had to unroute the entire board and reroute it by hand. I spent some time rearranging the ESP pins so that they had minimal overlap. 

![img4](journal/img4.jpg?raw=true)
![img5](journal/img5.jpg?raw=true)

*time spent: 4h*

# Day 4 8/20

Got another review. I was being dumb so today I learned keepout rules to remove copper fills from under the MAX IC. It's actually fixed now.
At least I didn't have to reroute the ESP pins! Bias trace was tricky.

![img6](journal/img6.jpg?raw=true)
![img7](journal/img7.jpg?raw=true)

*time spent: 2h*

*Total time spent: 16h*
