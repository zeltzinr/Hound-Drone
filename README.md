# Hound-Drone
Hey guys! here are some initial goals. Something to get started. If you have any other suggestion go ahead and add them. 
## Goals 
1. Check sensors on Navio
-> make sure they are working.
-> check how we're going to call each port being used for servos and other future extnesions. 
2. Make a solid flow chart for initial take off and leveled orbiting. 
 -> this is what we have so far: 
        Start
        Ceck sensors
        Check servos
        ---------> ready to launch 
                  - angle servos - take off
                  - power motor
                  if speed = maneuvering speed start spiral 
        - pitch spiral climb airspeed till altitude reached (still at full trottle) 
        - if altitude reached, start orbit
        end 
        
        ---------> routing
        - check for orbit point
        - check gps and angular speed
        - if not withing radius adjust servos 
        - check acceleration
        - cehck battery 
        - repeat
        
        ---------> landing 
        - check sensors 
        - angle servos and set throttle 
        - if altitude2 <= desired altitude then initiate stall 
        
        ---------> stall
        - cut motor 
        - if altitude3 <= desired altitude then pitch up to stall angle
        - power off
 
-> Here we can make the flow chart with github:
draw.io

-> here is a basic key for the flow chart

![basic-symbols](https://user-images.githubusercontent.com/33044780/35118521-9f43c916-fc57-11e7-9fab-b766d3943330.jpg)

