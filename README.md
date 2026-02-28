# 2026-Rebuilt
Code for FRC 2026 Rebuilt season robot named Tubs

Code for this project can be found https://drive.google.com/drive/folders/1fjmmcrGFe04reTASdwDBGGoulZAy3yIZ?usp=share_link

2-28-2026  Update from Roer from Orange Laptop
  **Updated shooter subsystem to be velocity controlled instead of power
    - Created feedforward and PID controller for shooter
    - Created a button that calculates distance away from basket and sets speed accordingly
    - Used Desmos and some experimenting to create a linear regrssion for targetRPM and distance from targetRPM
  ** Added CurrentLimits to SwerveDrive, which seems to help with brownouts.
  ** Created a Snappy DriveSwerveWithJoystick command that doesn't limit acceleration, but haven't tested.  

2-24-2026 Update from Rathbun
   - Created climber code (but stole from intake buttons to do it I think, -roer)
   - Created pathplanner code (untested)
   - Needs to be merged into 2-28-2026 and tested

2-21-2026 Update from Roer from Orange Laptop
  **SCRIMMAGE CODE
   - separated buttons for lifter and shooter trigger
   - fixed direction issue for driving on red alliance
   - minor tuning changes

2-19-2026 Update fro Roer from Orange Laptop
  **Created Intake subsystem
    - intake operates with button operation on control joystik
    - intake operates based solely on power input
    - power is set initially in Constants, but can be tunable in AdvantageScope
    - tested on 2-19 in practice

  **Created Shooter subsystem
    - shooter operates with two motors controlling the flywheel, and one motor with pulleys
      controlling the 'lifting pulleys' 
    - controlled by one button on control joystick that operates both simultaneously
    - controlled only by controlling power
    - power settings are set initially in constnats but tunable in advantage scope.
    - tested on 2-19 in practice

2-17-2026 (fork of 2-13-2026) From JJ
  - installed pathplanner and a simple path
  - untestable yet because drive subsystem wasn't testable, radio was sketchy, and battery not held in place yet
  - Roer attempted to test on patches with some success but unable to deterimine (yet) why it seemed to operate with unexpected paths. 
  - Expect a refinement from JJ, and Roer plans to install into 2-19's code after 2-19 proves workable. 

2-13-2026 Update from Roer from Orange Laptop
  Updated Swerve Drive with correct can id's, angle offsets, and tuned kp, ki, kd, ks and kv values
  Updated to do list
  Cleaned up telemetry statements to migrate away from SmartDashboard and onto AdvantageKit Logger

2-9-2026
  Initial Commit by Roer 
    Code built off of latest version of Patches 2026 rebuild
    Swerve Module rewritten to use SparkFlex Motor encoders
    Swerve Module rewritten to allow for tunable KP, KI, KD, and Feedward KS, KV values
    Can Id's preliminarily set but likely wrong... 
    To do list created for initial drive setup
    
