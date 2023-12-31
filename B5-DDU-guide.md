# **B5-DDU**

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-8.png" width="600">

**Copyright by VELOCITAS IMPERIUM - All rights reserved**

**Files are intended only for personal use, not commercial or for resale**


* 1 - [Introduction](#1-introduction)
* 2 - [Safety notes](#2-safety-notes)
* 3 - [BOM and parts](#3-bom-and-parts)
* 4 - [Preparing 3D Printed parts](#4-preparing-3d-printed-parts)
* 5 - [PCB Assembly steps](#5-pcb-assembly-steps)
* 6 - [Flashing and Programming the PCB](#6-flashing-and-programming-the-PCB)
* 7 - [Assembly](#7-assembly)
* 8 - [Troubleshooting](#8-troubleshooting)
* 9 - [Extras](#9-extras)



## 1. Introduction

We hope you find the order and assembly process smooth, and a reminder that we are always available to help through the discord. Simply post your questions in the #diy-and-simgear channel and one of our staff (or helpful members) will try to assist. This guide covers all the necessary information to assemble your DDU. Without further ado, let's begin.

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
There is an extra USB port on the PCB that you can use for the Vocore screen to avoid the extra charge for standard PCBA assembly or you can solder the micro USB by yourself.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-4.png" width="600">

Hit confirm, upload the BOM and CPL(POS) file like this

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-3.png" width="600">

After hitting process BOM & CPL you will get into the list of all the components needed for the build, it is all pre-configured by us, so you will need to hit NEXT, as they can't solder the Micro USB connector used for the vocore they will ask if you want to switch to their standard PCBA service (premium service) for a big markup so they will be able to solder that connector, you can decline and go with the extra port in the PCB or get the Micro USB port from lcsc and solder if afterwards.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-2.png" width="600">
<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-6.png" width="600">

After you have confirmed the parts you will have to select the Product description:

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-orderPCB-5.png" width="600">

and you're done, you can finish the order.

**NOTE** :It should cost around 110e without the microUSB connector, if you get a much lower price check you have done everything correctly.


## 4. Preparing 3D Printed parts

The following settings are intended for use with a 0.4mm nozzle and wall line count (perimeters) of 4 (printing times with an ender 3)

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

For a better finish, sanding and painting are suggested, the necessary steps are as follows:

1. Spray filler primer
2. Dry sanding from 200 up to 600 grit
3. Wet sanding from 800 to 1000 grit

**NOTE**: Be careful with power tools on plastic, due to risk of melting.

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

**NOTE: Flashing the bootloader on the B5 PCB is required, to do this you will need to solder the ISP header to the B5 PCB before proceeding to the next step, remember to remove the header when you have finished flashing the B5 PCB as it will interfere with the rear shell.**


## 6. Flashing and Programming the PCB

Before finalizing the assembly we want to make sure the buttons work, so we will start by explaining the process for flashing the bootloader. Unlike some other projects, the Arduino board we had you order in the BOM is simply there to flash the chip on the PCB itself and will be removed later. Before starting these steps it is recommended you remove any other arduino devices you may have plugged into your PC and close any programs that may be using/interfering such as SimHub.

## 6.1 Flashing bootloader - Arduino IDE


Flashing the bootloader is mandatory as they come without one, unlike the regular boards you can buy online.

You will need another Arduino for this process (or you can use whatever tools you like, but they are not covered in this guide, I use another Arduino as it's pretty common to have a spare), atmega328p(nano) or 32u4(micro) based boards are the same, you can follow the official guide on the [**Arduino website**](https://docs.arduino.cc/built-in-examples/arduino-isp/ArduinoISP) or you can read on below, but this is just a summary of the Arduino guide.

You can start by uploading the ISP sketch to your Arduino board as shown in the picture:


<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-flashPCB-3.png" width="600">

Then you need to connect your Arduino board to the B5 PCB, you need to connect the 5V, GND, MISO, MOSI, SCK, D10 pin to the corresponding pins on the B5 PCB, D10 goes to Reset.

You can follow the B5 PCB silkscreen as it's self-explanatory.

**NOTE** : If you are having trouble flashing the bootloader, you may have accidentally connected the RESET pin of your Arduino board to the Taurus PCB, the RESET pin on the Arduino board is not needed in this procedure, you will need to use the D10 pin instead.


<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-flashPCB-2.png" width="600">

You can use this table to understand which pins are MISO, MOSI and SCK on your Arduino board:

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-flashPCB-4.png" width="600">

Note:you can use this table with your Pro micro following the Leonardo pinout, or the UNO if you're using an arduino Nano

Here is an example if you're using a Pro micro as programmer 

<img src="https://github.com/VelocitasImperium/Taurus-GT3/blob/main/images/Guide/TaurusGt3-guideFlash4.png" width="600">

Here is another example if you're using an Arduino nano as programmer

<img src="https://github.com/VelocitasImperium/Taurus-GT3/blob/main/images/Guide/TaurusGt3-guideFlash7.png" width="600">

Once you have completed the wiring you can plug the Arduino board into your PC, if you have done everything correctly you will notice that the PWR LED on the B5 PCB is ON, now you can burn the bootloader:

Select the **Arduino Micro** on the "Board:" section.

Now you have two options depending on your Arduino (Programmer Board)

Select the **Arduino as ISP(Atmega32u4)** option on the "Programmer:" section if you have an arduino board based on that MCU (Such as the **Micro/Pro Micro**)

Select the **Arduino as ISP** option on the "Programmer:" section for the other boards based on the Atmega328p(such as **Arduino nano** )

The image below shows an example of a configuration using an Arduino nano.

<img src="https://github.com/VelocitasImperium/Taurus-GT3/blob/main/images/Guide/TaurusGt3-guideFlash5.png" width="600">

It will take about 2 minutes, you can see the RX TX LED(on the programmer) flashing during this process, don't disconnect until the Arduino IDE says it's done.

Now you can proceed without the Arduino Board and plug your Taurus PCB directly to the USB.

**NOTE** : If it gives an error, check your connection and that the IDE configuration is correct.


## 7. Assembly

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
  <tr>
    <td>12x5mm Magnets</td>
    <td>4</td>
  </tr>
</table>

The first step is to glue the magnets inside the shell and allow them to set.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-1.png" width="600">

Do the same for the bracket you're going to use. 

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-2.png" width="600">

**NOTE**: Make sure the magnets are in the correct orientation as it will be impossible to remove them without damaging them once they have cured.

Now go back to the screen holder:
Insert the hot inserts from the top, taking utmost care that they are flush with the surface. 

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-3.png" width="600">

Now you can place the Vocore in position and secure it in place with some electrical tape at the front and/or a little dab of hot glue / UHU Patafix at the back.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-10.png" width="600">

Now it's time to fix the PCB in position, using 3 M3x6 socket head screws, don't over tighten them as it's not necessary.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-7.png" width="600">

Fix the backshell to the screen holder with 4 M3x10 socket head screws.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-6.png" width="600">

Apply the double-sided tape where indicated and then place the Plexiglass in position, taking care not to leave any hair/fingerprints on the screen or Plexiglass.

<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-5.png" width="600">
<img src="https://github.com/VelocitasImperium/B5-DDU/blob/main/images/Guide/B5-mounting-4.png" width="600">

**NOTE**: If you need to disassemble the unit, simply unscrew the 4 rear M3x10 screws and insert a longer screw (e.g. a M3x20), just not all the way in, to prevent damaging the Plexiglass , then push on all sides until the whole assembly comes loose(You can also use the type-B connetor for pusing out the assembly).

## 9. Troubleshooting

## 10. Extras
