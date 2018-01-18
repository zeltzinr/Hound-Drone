# Hound-Drone

## Goals 
1. Check sensors: make sure they are working. 
2. Make a solid flow chart for initial take off and leveled orbiting. 
 -> this is what we have so far: 
        Start
        Check sensors
        Check servo motors
        ----------> ready to launch
                    - angle servos - take off
                    - power motor
                    - if speed = maneuvering speed start spiral
        - pitch spiral climb airspeed till altitude reached (still at full throttle)
        - if altitude reached start orbit
        end
        -----------> routing
          - check for orbit point
          - check gps and angular speed
          - if not within radius adjust servos
          - check acceleration
          - check battery
          - repeat
        ------------------------> landing
          - check sensors
          - angle servos & set throttle
          - if altitude2 <= desired altitude then initiate stall
        --------------------------------------------> stall
        - cut motor
        - if altitude3 <= desired altitude then pitch up to stall angle
        - power off  
-> here is a basic key

