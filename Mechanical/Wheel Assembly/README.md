# Wheel Assembly
The wheel assembly attaches the wheels to the motors and mounts the motors to the rest of the rocker-bogie suspension system that makes up the robot chassis.

![Wheels picture](img/wheels/wheels_title.PNG)
Final result.

# Preface

## Features

* The flexible wheels allow for high traction as they deform around objects, improving climbing performance
* Drive motors chosen to handle the high torque that the system sees, achieving both speed and climbing performance

## Skills

* Drill Press/Hand drill

## Tools

* Drill Press or hand drill
* Allen Key set
* Imperial Wrench Set
* Optional: 3D printer

## Dependencies on Other Modules

None

## Mechanical Interface/Attachments to Rover

* Corner wheels: 1/4 clamping hub to 1/4 inch stainless steel shaft on corner steering
* Actobotics + GoBilda channels and channel connectors to rocker-bogie

## Overview

1. Drilling the wheels
2. Assembling the base wheel mounts
3. Assembling the corner wheel mounts
4. Mounting the wheels

# Instructions

## Drilling the wheels

| item                              | ref | qty |                                                                 img |
| --------------------------------- | --- | --- | ------------------------------------------------------------------: |
| wheels                            | S30 | 6   | <img src="../../images/components/Structural/S30.jpg" height="100"> |
| hand drill or drill press         | D3  |     |       <img src="../../images/components/Tools/D3.png" height="100"> |
| center punch or starter drill bit | D7  |     |      <img src="../../images/components/Tools/D7.jpeg" height="100"> |
| drill bit #23                     | D6  |     |      <img src="../../images/components/Tools/D6.jpeg" height="100"> |

Drill holes in the wheels as shown in Figure 1 using the center drill and drill \#23.

> The wheel is normally meant to be mounted using one bolt through the middle of the rim. This will not work well in our case as the rover sees very high torque at the wheel and the one-bolt system would be difficult to attach to any part of our system without the wheel slipping. To attach more firmly, we will drill two holes on either side of the original hole where we will mount the motor hub clamp as shown in Figure 1

| ![](img/fabrication/Wheel%20Drill.PNG) | ![](img/fabrication/Wheel%20Aligned.PNG) |
| -------------------------------------- | ---------------------------------------- |

Figure 1: Drilling the wheels

The important dimension is that the two holes are as close to 0.770 inches apart as possible while remaining centered about the center of the wheel. We found that the geometry shown in Figure 1 allowed us to get the holes most easily. Normally for these through holes you would use drill \#25, but in order to give a little extra tolerance we recommend a few steps up from that, something around drill \#23. Test the holes with the 4mm Clamping Hub **S14** to make sure the holes align as shown in Figure 1. If the holes do not align, you can file them out slightly or even attempt to re-drill them depending on how close you are. Repeat this drilling process for all 6 of the wheels.

## Assembling the base wheel mounts

Next, we will build the wheel assemblies which are divided into the middle wheels and corner wheel assemblies. We will build 6 identical base wheels and then add slightly more complexity onto 4 of those which will eventually become the corner wheels.

| item           | ref  | qty | img                                                                   |     | item               | ref | qty | img                                                                   |
| -------------- | ---- | --- | --------------------------------------------------------------------- | --- | ------------------ | --- | --- | --------------------------------------------------------------------- |
| channel        | S45  | 6   | <image src="../../images/components/Structural/S45.webp" width="100"> |     | drive motor        | E49 | 6   | <image src="../../images/components/Electronics/E49.webp" width="100"> |
| 6mm D-hub      | S49  | 6   | <image src="../../images/components/Structural/S49.webp" width="100"> |     | M4 screws          | B15 | 48  | <image src="../../images/components/Screws/B15.webp" width="100">     |
| clamping mount | S47  | 6   | <image src="../../images/components/Structural/S47.webp" width="100"> |     | allen key set      | D2  |     | <image src="../../images/components/Tools/D2.jpeg" width="100">       |
| threaded plate | S46  |     | <image src="../../images/components/Structural/S46.webp" width="100"> |     | pattern adaptor    | S48 |     | <image src="../../images/components/Structural/S48.webp" width="100"> |


1. **Prepare the motor channel**: We will start by attaching pattern adaptors to connect the Servocity brackets to the bigger GoBilda brackets. Connect the pattern adaptor **S48** to the threaded plate **S46** using the screws that came with the pattern adaptor, as shown in Figure 2, but don't tighten the screws yet to make the next step easier. Now use M4 screws **B15** to attach the threaded plates **S46** to the GoBilda motor channel **S45**. The threaded plate should be on the outside of the channel. Once all screws are in, tighten them and make sure there is no air gap between the parts. Now repeat the process on the other side of the U-channel.

    | <image src="img/fabrication/pattern_adaptors.jpg"> | <image src="img/fabrication/attaching_adaptor_motor_channel_closeup.jpg"> | <image src="img/fabrication/attaching_adaptor_motor_channel.jpg"> | <image src="img/fabrication/motor_channel_adaptor.jpg"> |
    | -------------------------------------------------- | ------------------------------------------------------------------------- | ----------------------------------------------------------------- | ------------------------------------------------------- |

    Figure 2: Connecting the pattern adaptors. The tolerances might be tight, in which case it's best to connect the M4 screw to the threaded plate where the hole is elongated first, then loosely insert the larger screw into the channel adaptor before you attach the remaining two screws.

2. **Motor mount**: Attach the motor into the GoBilda channel **S45** you just prepared using clamping mount **S47** and screws **B15** as shown in Figure 3. Don't tighten the clamping mount to the motor all the way so we can adjust the positioning later to make the wheel center align with the corner steering axis. Slide on the motor shaft D-hub all the way back and tighten the clamp screw.

    <image src="img/fabrication/assembled_base_motor.jpg" height="250">

    Figure 3: Attaching the motor to the lower bracket

With that the base wheel assembly is completed! We will attach the wheels after building the corner wheel assemblies. Repeat above steps for the remaining 5 wheels.

## Assembling the corner mounts

Now, we need to create the four corner wheels. These build on what we made for the base wheel assemblies in the last step. For the corner motors, we will need to extend the attachment point upwards as it is important that the axes of the corner steering motors are directly above the middle of the wheels to enable smooth steering.

| item                           | ref  | qty | img                                                                   |     | item                          | ref | qty | img                                                                   |
| ------------------------------ | ---- | --- | --------------------------------------------------------------------  | --- | ----------------------------- | --- | --- | --------------------------------------------------------------------  |
| 3" channel                     | S2   | 4   | <image src="../../images/components/Structural/S2.jpg" width="100">   |     | 48 Tooth Plain Bore Gear      | S26 | 4   | <image src="../../images/components/Structural/S26.jpg" width="100">  |
| 4.5" channel                   | S4   | 4   | <image src="../../images/components/Structural/S4.jpg" width="100">   |     | 6-32 x 1/2" Button Head Screw | B3  | 8   | <image src="../../images/components/Screws/B3.png" width="100">       |
| Channel connector plate        | S6   | 12  | <image src="../../images/components/Structural/S6.jpg" width="100">   |     | 6-32 x 1/4" screws            | B1  | 40  | <image src="../../images/components/Screws/B1.png" width="100">       |
| 0.25" Face tapped clamping hub | S12  | 4   | <image src="../../images/components/Structural/S12.jpg" width="100">  |     | allen key set                 | D2  |     | <image src="../../images/components/Tools/D2.jpeg" width="100">       |
| Loctite Threadlocker           | S34  |     | <image src="../../images/components/Structural/S34.jpg" width="100">  |     | 6-32 x 3/4" Threaded Standoff | T3  | 4   | <image src="../../images/components/Standoffs/T3.png" width="100">    |
| wheels                         | S30A | 6   | <image src="../../images/components/Structural/S30.jpg" width="100">  |     | 6-32 x 5/8" screws            | B4  | 12  | <image src="../../images/components/Screws/B4.png" width="100">       |


1. **Channel Attachments 1**: Attach 3 inch channel **S2** to your base wheel assembly using 8 screws **S6** as shown in Figure 4.

    <image src="img/fabrication/assembled_base_motor.jpg" height="250">

    Figure 4: Attaching the 3in channel to the motor assembly

2. **Preparing the 4.5 inch Channels - D-Clamping Hub Attachment**: Attach the 0.25in clamping hub **S12** and the plane bore gear **S26** to the channel using screws **B3** from the top and **B1** from the bottom as shown in Figure 5.

    | <img src="img/wheels/Corner%20Wheel%20Step%205.PNG" height="250"> | <img src="img/wheels/Corner%20Wheel%20Step%206.PNG" height="250"> |
    | ----------------------------------------------------------------- | ----------------------------------------------------------------- |

    Figure 5: Attaching the large encoder gear

3. **Preparing the 4.5 inch Channels - Hard stop mount**: In order to keep the wheels from spinning too far in either direction, we will install a physical hard stop in the system. Attach a standoff **T3** with screw **B1** and optionally Loctite Threadlocker **S34** to the channel as shown in Figure 6. This standoff will be our hard stop. Make sure that you use the correct mounting hole or the standoff will not line up with the hard stops on the encoder mount.

    <image src="img/wheels/hard%20stop%20mount.PNG" height="250">

    Figure 6: Attaching the hard stop that prevents the corner motor from rotating too far

4. **Attaching the 4.5 inch channel**: Attach the 4.5in channel **S4** to the top of the 3in channel from the last step using two channel connectors **S6** and screws **B1** as shown in Figure 7.

    | <img src="img/wheels/Corner%20Wheel%20Step%204.PNG" height="250"> | <img src="img/wheels/corner_assembly_cad.jpg" height="250"> |
    | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
    
    Figure 7: Attach the 4.5in channel you made in step 3 to the base wheel mount

5. **Repeat for the other corner wheels**: You should have 4 corner assemblies and 2 base wheel assemblies.


## Mounting the wheels
   
For all 6 assemblies, use screws **B4** to mount the wheels to the shaft clamp on the motors.

<image src="img/wheels/Wheel%20Step%203.PNG" height="250">

Figure 8: Attaching the wheels

Congratulations, you finished another major assembly!
