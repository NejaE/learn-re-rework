---
title: "Robot Commander"
permalink: robot_commander
nav_exclude: true
--- 

# How to drive with a Smartphone or workstation using Robot Commander in AP mode

Robot Commander can be used on an Android phone. It's an old app that is becoming fast obsolete by EZ-Map, however it should still come in handy for basic testing. As such however, it is no longer being maintained.

<div class="image-wrapper">

<img src="assets/Robot_Commander.png" />


<p class="image-caption">Robot Commander</p>

</div>

## To use an Android phone:

1. Turn the robot on.
2. If you haven't, install the Robot Commander app on your Android phone. Download it on your phone at <https://play.google.com/store/apps/details?id=com.jrlandau.robotcmdr>.
3. Allow at least 1 minute after turning the robot on to allow the robot to boot up. The robot will come up as its own WiFi network. So on the phone, if you go to Settings/WiFi, you should see a WiFi network that looks something like`ubiquityrobotXXXX`, where `XXXX` corresponds to 4 hexadecimal digits. Connect to this network.  The password is `robotseverywhere`. If you cant find robot's WiFi network, try restarting your robot
4. Start the Robot Commander app.  
5. Enter the address `ubiquityrobot.local` in the space to the left of the Connect button.
Continue with #6 below.

<!---
## To use a workstation
Temporarily withdrawn.  

1. Turn the robot on.
2. Unless you've done it already, install the [Google Chrome browser](https://www.google.com/chrome/browser/desktop/index.html) on your workstation.  Bring up the browser.
3. Allow at least 3 minutes after turning the robot on. On your workstation, connect to the UbiquityRobot network. The password is `robotseverywhere`.
4. Enter the address <https://10.42.0.1/speechcommands.html> in the address bar of the Chrome browser, and press the enter key.
5. If the browser gives you any warnings regarding a lack of security, disregard them.
6. Press or click the `Connect` button. You will hear "Connected" and the button will now read "Disconnect".  
-->

## Using Robot Commander To Move The Robot
* Press any arrow to move the robot. To keep the robot moving, keep pressing or clicking.
* Tap the Microphone to use speech.
* Say, "forward", "back", or other commands. There is a list of commands in the menu in the top right corner of the screen. The forward and back and the rotation commands allow you to say how far, for example "forward 3 feet" or "back 5 meters", or "rotate right 90 degrees".
* Where there is a lot of competing speech, you can turn on the "wake word" feature, in Settings. When it is on, all commands must be prefaced by the wake word, "robot".

### Robot Commander Simple Movement Commands
* forward, advance, keep going, go ahead, go straight, reverse, back, backward, go back, retreat<br>
* forward/reverse etc., may be followed by meters/centimeters/feet\*
* turn right
* turn left
* turn around
* stop, halt
* faster, speed up
* slower, slow down
* again, repeat
* find aeroplane, bicycle, bird, boat, bottle, bus, car, cat, chair, cow, diningtable, dog, horse, motorbike, person, pottedplant, sheep, sofa, train, tvmonitor
* battery
* help

## Using Robot Commander In Navigation Mode

A mostly experimental mode of Robot Commander is to allow setting of ```waypoints``` which are a specific location and direction of the robot when full robot navigation is in use and our  move_basic node is up and running.  

Full navigation is an advanced robot mode of operation but to get a general feel for one such mode you may wish to use [Our Fiducial-Based Localization](https://github.com/UbiquityRobotics/fiducials). Note that this nav stack is deprecated.

Assuming navigation is running and the robot is set to know it's location in the map then Robot Commander can be used to set and return to waypoints that you define within Robot Commander.

### Set a waypoint
* You can move the robot in the same way as you did in the Robot Commander section above.  To set waypoints you must have set up fiducial markers as in the section on fiducials above.
* Tap the Microphone to use speech.
* Say `waypoint alpha`. You can use any name you like for a waypoint, but the phonetic alphabet is convenient as it is, by design, easily understood.
* Robot Commander will ask whether it has understood the waypoint name. Assuming that it has,
* Check the waypoint with the voice command `list waypoints`.

Perhaps you may wish to drive to more locations and define other waypoints such as `waypoint beta` and so on.

### Goto A waypoint

* Now you can move the robot to some other location in the area.
* The voice command `go to alpha` will now cause the robot to go to the waypoint you established, and to face in the same direction it was when you set the waypoint.
* You can remove a waypoint with the voice command `remove waypoint alpha`.  

### Voice Commands For Navigation mode

The following list are voice commands that can be used if the robot is in a full navigation mode within a pre-defined map.

* rotate right (may add "n degrees")
* rotate left (may add "n degrees")
* (set) waypoint ____ (waypoint name)
* go to ____ (waypoint name)
* remove waypoint ____ (waypoint name)
* list waypoints
