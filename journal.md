---
Title: "Robot Brain"
Author: "Padimo/Omegon0"
Description: "Upgraded ESP32-based robot circuit board."
Created On: "8/8/2025"
---

# Day 1 8/8

This is the second attempt of making a robot. The first attempt failed because I tried to hotplate a lot of QFN packages and legitimately the only parts that worked were USB power, ESP and a singular neopixel. 
This attempt aims to simplify the robot so that it actually works. 

First of all motors need a decent amount of current so I'm using the LM1084-3v3 to supply that. (tbh doesn't really matter since the H bridges will be supplied from 12V battery but just in case)
H bridges I want an SMD equivalent of an L293N

Found one its called the L293DD and it has lots of ground pads. i think that's for heat sucking so that's important
started schematic 
For USB/battery power switching I'm just gonna use a physical slide switch SPDT because I cannot be bothered to create an automatic switching circuit (the last one failed miserably, see the EMG project)
wired a bit of stuff up

![sch0](https://github.com/Omegon0/robotbrain/blob/main/log/sch0.jpg?raw=true)

*time spent: 2h*

# Day 2 8/9

Wired up the motor drivers. 
I decided to add a magnetometer LIS2MDL because magnetic fields are a good way of measuring direction (compass)
I hate datasheets. I had to add electrolytic caps for the motor drivers and those are THT. Don't know if JLC PCBA will do that

![sch1](https://github.com/Omegon0/robotbrain/blob/main/log/sch1.jpg?raw=true)

*time spent: 3h*

# Day 3 8/10

Wired up the ESP. Added footprints

![sch2](https://github.com/Omegon0/robotbrain/blob/main/log/sch2.jpg?raw=true)

*time spent: 2h*

# Day 4 8/13

I realize now that the USB port is also THT, whoops. Well LCSC has it so I'm using it, I may have to hand-solder those items later on. Can't avoid PCBA because LIS2MDL. 
Arranged PCB outline and board (no image i forgot whoops)
how have i done so many PCB projects and not known about align/distribute. feels like a crime

*time spent: 2h*

# Day 5 8/14

I hand routed the whole board then realized I had no zones. Added those and then redid the board. only THEN did I google automatic routing kicad and install the freerouting plugin

![pcb](https://github.com/Omegon0/robotbrain/blob/main/pcb.jpg?raw=true)

*time spent: 3h*

# Day 6 8/15

Created github and stuff and wrote this journal based off of my own logs (i used my zip extension! check out https://github.com/Omegon0/zip)
Created renders and added some components (many steps failed to load. still working on that)

*time spent: 2h*

# Day 7 8/19

submitting today! 
edit: forgot to actually commit to and push the repo. i just said i dumped everything
