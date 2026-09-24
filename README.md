# Omron TM7S Student Workshop Guide

This guide supports undergraduate students using the Omron TM7S collaborative robot in the RMIT IA-Cobotics Lab.

> **Safety first:** Follow the instructions of the supervising staff member at all times. Do not press buttons or move the robot until the guide tells you to do so.

## Workshop flow

1. Start the robot safely.
2. Log in and switch to manual mode.
3. Move the robot using interactive and screen controls.
4. Create, connect, and run a simple robot routine.

![Omron TM7S tablet interface](resources/TM7S-Omron-360-0000.webp)

## 1. Start the robot safely

The tablet is attached to the robot and is used to operate it.

1. Make sure the emergency stop is pressed before doing anything else.

   ![Press the emergency stop](resources/2-HitEstop.png)

2. Press the power button once. The power light will turn on and the tablet will show startup screens.

   | Press the power button | Startup screen |
   | --- | --- |
   | ![Press the power button](resources/3-TurnOnTablet.png) | ![Tablet starting up](resources/4-TabletTurningOn.png) |

## 2. Log in and select manual mode

### Log in

After startup, the tablet displays the login screen. Ask the supervising staff member for the username and password.

> **You need a keyboard for this step.** Connect it to the USB port near the top-left of the tablet.

![Tablet login screen](resources/5-LoginScreenAsk.png)

After logging in, the tablet should look similar to this:

![Tablet after login](resources/6-NextScreen.png)

### Switch from Auto to T1

The robot starts in **Auto** mode. Do not interact with or move the robot while Auto is selected.

1. Move at least **1.5 metres away** from the robot before changing its mode.

   ![Safe distance from the robot](resources/8-Overview.png)

2. Twist the emergency-stop button until it pops up. The markings on the button show the direction to turn.

   | Twist the emergency stop | Emergency stop released |
   | --- | --- |
   | ![Twist the emergency stop](resources/9-TwistOverview.png) | ![Release the emergency stop](resources/10-Twist2.png) |

3. Touch and hold **M/A** for at least five seconds. Hold it until you hear a beep and **Auto** begins flashing.

   ![Touch and hold M/A](resources/11-M_A_LaterStep.png)

4. Enter the following button sequence:

   **`+`, `-`, `+`, `+`, `-`**

5. Touch **M/A** again, then press **Play**. Confirm that **T1** is highlighted in the status bar.

   | Press `+` | Press `-` | Press Play | T1 selected |
   | --- | --- | --- | --- |
   | ![Press plus](resources/12PressingPlus.png) | ![Press minus](resources/13-PressingNegative.png) | ![Press Play](resources/14-PressingPlay.png) | ![Manual mode active](resources/15-InManual.png) |

The robot is now ready for manual operation.

## 3. Move the robot

### Open the simulator view

Press the simulator-view button to display the robot and its controls.

![Robot and simulator view](resources/17-ViewOfRobotAndSim.png)

### Option A: interactive manual movement

1. Press the black button on the robot manipulator **halfway**, stopping before the second click.
2. Confirm that the ring around the robot's TCP turns bright green.
3. While holding the button, gently push the robot to move it.

> **Move very slowly.** Keep control of the robot at all times and stop immediately if anything looks unsafe.

![Hold the manipulator button halfway and move slowly](resources/19-Hold_ManipulatorForFreeRangeOperation.png)

### Option B: joint and Cartesian controls

The simulator provides two groups of movement controls:

- **Cartesian:** `X`, `Y`, `Z`, `Rx`, `Ry`, and `Rz`
- **Joint:** `J0` through `J6`

1. Select **Cartesian** or **Joint**.
2. Select the blue button for the axis or joint you want to move.
3. Press the tablet-side button halfway, as in Option A.
4. Hold `+` or `-` and observe the robot's movement.

![Cartesian and joint motion controls](resources/18-ViewOfMotionScreen.png)

![Press the tablet-side button halfway](resources/16-PressHalfInTablet.png)

Discuss these questions with your group:

- Which robot values or parameters change when you move an axis or joint?
- How are Cartesian movements different from joint movements?
- How do `X`, `Y`, and `Z` differ from `Rx`, `Ry`, and `Rz`?

## 4. Exercise: build and run a routine

In this exercise you will create a project, record robot poses, connect the poses, and replay the routine.

### Create a project

1. Open the project menu from the tablet.

   | Open the project menu | Select the project view |
   | --- | --- |
   | ![Open the project menu](resources/IMG_1215.JPEG) | ![Select the project view](resources/IMG_1216.JPEG) |

2. Confirm that the project workspace is open.

   ![Project workspace](resources/IMG_1217.JPEG)

3. Select **File > New**.

   ![Create a new project](resources/IMG_1218.JPEG)

4. Enter a name for the project and confirm it.

   ![Name the project](resources/IMG_1219.JPEG)

### Record poses

1. Use manual interactive mode from Section 3 to move the robot to a safe starting pose.
2. Add a point or pose to the routine.
3. Move the robot to the next pose and record it again.
4. Repeat until you have at least two poses.

   ![Example project view](resources/IMG_1220.JPEG)

The later workshop photos show the pose and waypoint workflow:

![Example pose](resources/IMG_1226.JPEG)

![Second example pose](resources/IMG_1230.JPEG)

![Record a waypoint](resources/Screenshot%202026-09-24%20132950.png)

### Connect and run the routine

1. Connect the recorded points in order to make one continuous routine.

   ![Connect the recorded points](resources/IMG_1223.JPEG)

2. Drag the final connection back into the loop as shown in the example.

   ![Close the routine loop](resources/IMG_1224.JPEG)

3. Press the tablet-side button halfway to enable operation.
4. Press **Play** and watch the robot replay the routine.

> Keep the emergency stop accessible and be ready to stop the robot while the routine runs.

## Completion checklist

- [ ] Robot started with the emergency stop pressed.
- [ ] Robot changed from Auto to T1 with staff supervision.
- [ ] Robot moved slowly in simulator view.
- [ ] Cartesian and joint controls were compared.
- [ ] A project was created with at least two recorded poses.
- [ ] The poses were connected and replayed safely.
