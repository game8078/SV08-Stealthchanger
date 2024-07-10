# SV08-Stealthchanger
Welcome, below you will find all the steps needed to convert the Sovol SV08 to work with the Stealthchanger project my DraftShift Design.

# List-of-Major-Steps:
- 2020 extrusion additon to frame
* Raise bed
+ Add Extra Powersupply
- Flash Mainline Klipper To Board MCU
* Setup Printer.cfg
+ Setup Canbus Network
- Flash Toolboard MCU
* Change Belts
+ Build Toolheads
- Add Stealthchanger Shuttle and Your Choice of Toolhead
* Add Tap Features
+ Tune Printer With One Toolhead
- Add Docks
* Add StealthChanger Sofware
+ Add Tools
- Tune Printer

# SV08-2020-Extrusion-Mount-Stealthchanger
An addition to the Stealthchanger tool changer that allows for the SV08 to have a piece of 2020 extrusion mounted in the top of the printer for the docks used by Stealthchanger.

![TopView](https://github.com/game8078/SV08-2020-Extrusion-Mount-Stealthchanger-/blob/main/photos/TopdownView%231.PNG)
Source a piece of 2020 extrusion that is 420mm long (cut yourself or custom order) and print the brackets found on printables. https://www.printables.com/model/887692-sv08-2020-top-rail-adapter-bracket-toolchanger-or  

# Raise Bed
Due to switching out the toolhead the height of where the nozzle sits is higher that that of the stock SV08 nozzle. This means the nozzle can't touch the bed once installed onto the StealthChanger Shuttle. To fix this issue 9.5mm spacers are used to raise the bed from its original location. (This change also allows you to put insulation under your bed)

Spacers: https://www.amazon.com/dp/B0CQ87Y4VQ?_encoding=UTF8&psc=1&ref_=cm_sw_r_cp_ud_dp_0SBBW6MAYBM8K1HCDFKS 

Bolts m4x35 SHCS: https://www.amazon.com/gp/product/B0CYGKLHTP/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8 

Insulation: https://www.amazon.com/gp/product/B08XQ3CK81/ref=ewc_pr_img_3?smid=A17REXMFA4MBN8&psc=1 

# Add Extra Powersupply
Adding an extra powersupply is a neccesity on the SV08 as it comes stock with harldly enough watts to begin with, let alone have multiple toolheads. WARNING!!!!! This part of the conversion is dangerous as you need to mess with mains power  WARNING!!!!! First is to determine how much power you will need, this is system to system dependant as your electronics. Please use the DraftShift Power Calculator: https://github.com/DraftShift/PowerCalc?tab=readme-ov-file 
Once you determain your powersupply mount the powersupply to the bottom of your printer, here you can do one of two options, leave the 150w powersupply in place and run your board and motors off of that and your toolheads off of your new psu or remove the 150w and just use your new psu. If using both psu units all you need to do is using Wago connectors to splice into the existing wires and run the AC to your new psu. 
![TopView](https://github.com/game8078/SV08-Stealthchanger/blob/main/photos/Added%20Powersupply.jpg)
I used some din rail mounts I found of printables to attach to the SV08.
# Flash Mainline Klipper To Board MCU
Please you this github project for this step. PSA it is still in beta. https://github.com/Rappetor/Sovol-SV08-Mainline 
# Setup Printer.cfg
Please you this github project for this step. PSA it is still in beta. https://github.com/Rappetor/Sovol-SV08-Mainline 
# Setup Canbus Network
I used the U2C plugged into the compute modual on the mainboard. 
The best resource for setting up canbus is this guide. https://canbus.esoterical.online/ 
Next is to remove the stock toolhead cable and route a canbus cable from your usb to canbus converter up to your canbus breakout board(BTT CEB in my case) and from your breakout board to your toolhead PCB. PSA: Remember to have both the 120R jumper on both your canbus adapter and your toolhead PCB.
# Flash Toolboard MCU
The best resource for this part is https://canbus.esoterical.online/ 
# Change Belts
The stock 6mm belts are not long enough for the stealthchanger shuttle so they need to be redone with longer belts. At the bottom of this document I have listed all the components that I used that includes the belts I used. (5 meters is the amount of belt needed)
To change the belts remove the stock metal bracket that holds on the belts and attach the new belt to the old belt and pull the belt till the new belt replaces the old ones. 
# Build Toolheads
![TopView](https://github.com/game8078/SV08-2020-Extrusion-Mount-Stealthchanger-/blob/main/photos/Hummingbird%20Extruder.jpg)
# Add Stealthchanger Shuttle and Your Choice of Toolhead
Please use the StealthChanger documentation for this step.
# Add Tap Features
next on my todo list
# Tune Printer With One Toolhead
todo list
# Add Docks
![TopView](https://github.com/game8078/SV08-2020-Extrusion-Mount-Stealthchanger-/blob/main/photos/Modular%20Docks%20on%202020%20Extrusion.jpg)
![TopView](https://github.com/game8078/SV08-2020-Extrusion-Mount-Stealthchanger-/blob/main/photos/Modular%20Docks%20With%20Tools.jpg)
# Add StealthChanger Sofware
todo list
# Add Tools
todo list
# Tune Printer
todo list

# My Part List
https://docs.google.com/spreadsheets/d/1JrJ9xVd0SPiwflk1HpY03_PSYyF7ZYIquvCaTutLPTw/edit?usp=sharing 