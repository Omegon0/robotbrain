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

![sch0](https://github.com/Omegon0/robotbrain/log/blob/main/sch0.jpg?raw=true)

*time spent: 2h*
