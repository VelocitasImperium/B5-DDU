# **B5-DDU**

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-8.png" width="600">

**Copyright by VELOCITAS IMPERIUM - All rights reserved**

**Files are intended only for personal use, not commercial or for resale**


* 1 - [Introduction](#1-introduction)
* 2 - [Safety notes](#2-safety-notes)
* 3 - [BOM and parts](#3-bom-and-parts)
* 4 - [Preparing 3D Printed parts](#4-preparing-3d-printed-parts)
* 5 - [PCB Assembly steps](#5-pcb-assembly-steps)
* 6 - [Flashing and Programming the PCB](#7-flashing-and-programming-the-PCB)
* 7 - [Assembly](#8-assembly)
* 8 - [Troubleshooting](#9-troubleshooting)
* 9 - [Extras](#10-extras)



## 1. Introduction

We hope you find the order and assembly process smooth, and a reminder that we are always available to help through the discord. Simply post your questions in the #diy-and-simgear channel and one of our staff (or helpful members) will try to assist. This guide covers all the necessary information to assemble your DDU, as well as links to the required shifters and clutches. Without further ado, let's begin.

## 2. Safety notes

#### With any DIY project we must ensure we are safe at all times to avoid any potential injury or damage. Our recommendations are the following:

1. Always wear safety glasses, particularly when performing steps such as sanding the 3D print
2. Ensure any soldering is done in a well ventilated area, using a fan to pull away dangerous fumes if possible
3. Wear gloves to avoid later contamination when soldering with leaded solder.
4. Find a comfortable position to avoid back pain later on, this wheel takes quite a while to assemble and it is better to do it comfortably.

## 3. Bom and parts

The BOM is available [**here**](https://docs.google.com/spreadsheets/d/1LTHWi-7xIeATiLtcv8ewfXO0zlp6xbxwbrMM7N581tc/edit#gid=1313035800) and you can make your own copy to tick off parts as you go.

It's a good idea to order everything before starting so that you don't miss anything or end up with incorrect parts. The BOM also contains some useful tips on what parts to order and recommendations, _as well as some recommended tools for the job!_ We have intentionally left some flexibility with the parts (eg: switches from either AliExpress or Mouser) so you can make the decision on how much you'd like to spend. In general, the extra money does reflect extra quality but if you think you can get a great deal somewhere else, go for it! That's the benefit of DIY 🙂 \*Velocitas Imperium are not endorsing any of these parts, just making helpful suggestions if you are struggling to source the parts yourself\*

We will now cover some specifics for ordering certain items, such as the **Graphics/Adhesives, CNC,** and the **PCB**.

## 3.1 Plexiglass + UV print

You can order a 2mm transparent Plexiglas plate, with our supplied UV print file, there is an extra PNG file included to show what should be transparent and where it should not be (BLUE = Transparent), both files should be sent to your preferred manufacturer.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-silk1.png" width="600">
<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-silk2.png" width="600">

## 3.2 PCB Order

For the PCB I suggest you use JLCPCB and follow these instructions (if you don't understand a step you can ask for help in our Discord).

Upload the gerber file to their website leave everything default but the stackup has to be the JLC7628 for the best result.(You can leave the default as it's the same stackup, but JLCPCB may change it in the future)

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-1.png" width="600">

Enable PCB assembly and leave the default options.
If you want to use the microUSB connector on the PCB, you must enable the standard PCBA service or they will not be able to solder it.
There is an extra USB port on the PCB that you can use for the Vocore screen to avoid the extra charge for standard PCBA assembly.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-4.png" width="600">

Hit confirm, upload the BOM and CPL(POS) file like this

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-3.png" width="600">

After hitting process BOM & CPL you will get into the list of all the components needed for the build, it is all pre-configured by us, so you will need to hit NEXT, as they can't solder the Micro USB connector used for the vocore they will ask if you want to switch to their standard PCBA service (premium service) for a big markup so they will be able to solder that connector, you can decline and go with the extra port in the PCB or get the Micro USB port from lcsc and solder if afterwards.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-2.png" width="600">
<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-6.png" width="600">

After you have confirmed the parts you will have to select the Product description:

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-5.png" width="600">

and you're done, you can finish the order.
**NOTE:It should cost around 110e without the microUSB connector, if you get a much lower price check you have done everything correctly.


## 4. Preparing 3D Printed parts

The following settings are intended for use with a 0.4mm nozzle and wall line count (perimeters) of 4 (printing times with and ender 3)

<table>
  <tr>
    <th>File Name</th>
    <th>Layer Height</th>
    <th>Infill</th>
    <th>Supports</th>
    <th>Est. print time</th>
    <th>Extra notes</th>

  </tr>
  <tr>
    <td>All parts</td>
    <td>0,12</td>
    <td>60%</td>
    <td>No</td>
    <td>3h</td>
    <td> </td>
  </tr>
</table>

## 4.1 Postprocessing

For a better finish, sanding and painting are suggested, the necessary steps are as follows(for grips only sanding is suggested):

1. Spray filler primer
2. Dry sanding from 200 up to 600 grit
3. Wet sanding from 800 to 1000 grit

**NOTE**** :** Be careful with power tools on plastic, due to risk of melting.

## 5. PCB Assembly steps
In this part of the guide you will need this items:

<table>
  <tr>
    <th>Items needed:</th>
    <th>Quantity</th>
  </tr>
  <tr>
    <td>PCB</td>
    <td>1</td>
  </tr>
  <tr>
    <td>USB Type B connector</td>
    <td>1</td>
  </tr>
  <tr>
    <td>SMD USB micro B connector(optional)</td>
    <td>1</td>
  </tr>
  <tr>
    <td>EG1218</td>
    <td>1</td>
  </tr>
</table>

## 5.1 PCB soldering

If you bought the fully assembled PCB from JLCPCB, you only need to solder the vertical USB type B connector, the EG1218 on/off button on the back and the 6 pin header to flash the bootloader in the following steps.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-solderPCB-3.png" width="600">

Otherwise, you'll have to solder the SMD USM Micro connector as well, or just 4 wires to the USB holes (highlighted in blue) for the Vocore.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-solderPCB-2.png" width="600">

**NOTE: Flashing the bootloader on the B5 PCB is required, to do this you will need to solder the ISP header to the B5 PCB before proceeding to the next step, remember to remove the header when you have finished flashing the B5 PCB as it will interfere with the rear shell.


## 7. Flashing and Programming the PCB

You'll need another arduino for this process, atmega328p or 32u4 based boards are the same, you can follow the official guide on the arduino website or you can keep reading below, but this is just a summary of the arduino guide.

You can start by uploading the ISP sketch to your Arduino board as shown in the picture:


<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-flashPCB-3.png" width="600">

Then you need to connect your Arduino board to the B5 PCB, you need to connect the 5V, GND, MISO, MOSI, SCK, D10 pin to the corresponding pins on the B5 PCB, D10 goes to Reset.
You can follow the B5 PCB silkscreen as it's self-explanatory.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-flashPCB-3.png" width="600">

You can use this table to understand which pins are MISO, MOSI and SCK on your Arduino board:

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-flashPCB-4.png" width="600">

After you do the connection you can burn the bootloader:

Select the Arduino Micro on the “Board:” section. 
Now you have two options depending on your Arduino (Programmer Board)
Select the Arduino as ISP(Atmega32u4) option on the “Programmer:” section if you have an arduino board based on that MCU (Such as the Micro/Pro Micro)
Select the Arduino as ISP option on the “Programmer:” section for the other boards based on the Atmega328p(such as Arduino nano) 

The image below shows an example of a configuration using an Arduino nano.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-flashPCB-1.png" width="600">

It will take about 2 minutes, you can see the RX TX LED flashing during this process, don't disconnect until the Arduino IDE says it's done.

If it gives an error, check your connection and that the IDE configuration is correct.


## 8. Assembly

In this part we will need this parts:

<table>
  <tr>
    <th>Items needed:</th>
    <th>Quantity</th>
  </tr>
  <tr>
    <td>Screen holder</td>
    <td>1</td>
  </tr>
  <tr>
    <td>M3x4x4 Heat insert</td>
    <td>7</td>
  </tr>
  <tr>
    <td>Socket/Button M3x6</td>
    <td>3</td>
  </tr>
  <tr>
    <td>Socket M3x10</td>
    <td>4</td>
  </tr>
</table>

Insert the hot inserts from the top, taking utmost care that they are flush with the surface. 

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-3.png" width="600">


Now you can place the Vocore in position and secure it in place with some electrical tape at the front and a little dab of hot glue / UHU Patafix at the back.
Now it's time to fix the PCB in position, using 3 M3x6 socket head screws, don't over tighten them as it's not necessary.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-7.png" width="600">

Apply the double-sided tape where indicated and then place the Plexiglass in position, taking care not to leave any hair/fingerprints on the screen or Plexiglass.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-5.png" width="600">
<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-4.png" width="600">

NOTE: If you need to disassemble the unit, simply unscrew the 4 rear M3x10 screws and insert a longer screw (e.g. a M3x20), just not all the way in, to prevent damaging the Plexiglass , then push on all sides until the whole assembly comes loose(You can also use the type-B connetor for pusing out the assembly).

