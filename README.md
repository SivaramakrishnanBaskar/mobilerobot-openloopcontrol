# MobileRobot-Openloopcontrol

## Aim:
To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1: Initiate the MobileRobot.

<br/>

Step2: Connect your PC with the MobileRobot.

<br/>

Step3: Open Python program.

<br/>

Step4: Program the movements of the robot using python code.

<br/>

Step5: Execute the python program.

<br/>

## Program

```
Developed By: Sivaramakrishnan B
Register Number: 212222110044

from robomaster import robot
import time 
from robomaster import camera

if __name__ == '__main__':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis

    ep_chassis = ep_robot.chassis
ep_led = ep_robot.led
ep_camera = ep_robot.camera

print("Video streaming started.....")
ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)



ep_chassis.move(x=2.8, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=255,g=100,b=0,effect="on")


ep_chassis.move(x=0 , y=0, z=50, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=204,g=255,b=204,effect="on")


ep_chassis.move(x=0.4, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")


ep_chassis.move(x=0, y=0, z=45, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=153,g=204,b=0,effect="on")


ep_chassis.move(x=0.8, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=204,g=204,b=255,effect="on")


ep_chassis.move(x=0, y=0, z=85, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=128,g=0,b=0,effect="on")



ep_chassis.move(x=1.2, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")


ep_chassis.move(x=0, y=0, z=-45, xy_speed=1).wait_for_completed()

ep_chassis.move(x=1.7, y=0, z=0, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=102,g=0,b=202,effect="on")


ep_chassis.move(x=0, y=0, z=43, xy_speed=1).wait_for_completed()


ep_chassis.move(x=1.4, y=0, z=0, xy_speed=1).wait_for_completed()

ep_chassis.move(x=0, y=0, z=95, xy_speed=1).wait_for_completed()
ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")


ep_chassis.move(x=2.2, y=0, z=0, xy_speed=1).wait_for_completed()

ep_chassis.move(x=0, y=0, z=80, xy_speed=1).wait_for_completed()

ep_led.set_led(comp = "all",r=255,g=102,b=0,effect="on")

ep_chassis.move(x=0.6, y=0, z=0, xy_speed=1).wait_for_completed()

time.sleep(4)


p_camera.stop_video_stream()
print("Stopped video streaming.....")
ep_robot.close()

    
    ep_robot.close()

```

## MobileRobot Movement Image:

![image](https://github.com/SivaramakrishnanBaskar/mobilerobot-openloopcontrol/assets/119476322/20067649-9751-48b3-8c8c-95c734b3ac5d)
<br/>
![image](https://github.com/SivaramakrishnanBaskar/mobilerobot-openloopcontrol/assets/119476322/7a9a21f4-b363-45b9-a908-630f3ab54f1f)
<br/>
![image](https://github.com/SivaramakrishnanBaskar/mobilerobot-openloopcontrol/assets/119476322/2267e9bd-ffe5-48ea-b1d1-2c43cec194cf)
<br/>
![image](https://github.com/SivaramakrishnanBaskar/mobilerobot-openloopcontrol/assets/119476322/a8a9563a-e811-4fc7-b9c8-463bbfe60604)


## MobileRobot Movement Video:

https://youtu.be/dvaE6C47CeY

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
