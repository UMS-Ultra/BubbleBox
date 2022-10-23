# BubbleBox 1.0: Digital Controller
 The BubbleBox 1.0 is a digital controller for platform fighters and other games:
 
![image](Images/BubbleBox%20Black%20and%20Light%20Grey%20Hex%20Keycaps.jpg)


# Important License Infomation

This project is licensed under the CERN-OHL-S v2 open source license. This is a "strongly reciprocal copyleft" license that allows free use of the files, but requires you to publish any modifications you make to the project under the same license, if you distribute your own files or sell versions that you produce. You are also compelled to link back to this github repository (https://github.com/UMS-Ultra/BubbleBox) in your own repository and/or where you sell them. Please check out the license.txt file to learn how you are allowed to use the files, and check out https://ohwr.org/cernohl for more information and CERNs FAQ.


# Installing and Updating Firmware

To update the firmare on a BubbleBox, hold the Start button when you plug into your computer to boot it into it's firmware flashing mode. It will show up in your file explorer as a storage device like a USB Flash drive. When plugging in a new Pico into a computer for the first time, it will automatically boot in it's firmware flashing mode.

![image](Images/Pico%20File%20Window.PNG)

If your controller or doesn't boot into it's firmware mode under those conditions, hold the white "Bootsel" button on the Pico itself when plugging it in.

![image](Images/Pico%20Bootsel%20Button.jpg)

Once it's in the Firmware mode and you can access it's storage, simply drag and drop the firmware.uf2 file onto it. It's exactly like putting something on a USB Flash Drive.

![image](Images/Firmware%20Gif.gif)

When done successfully, the LED on the Pico should glow Green:

![image](Images/Pico%20Green%20LED.jpg)

And your computer will make the noise that it makes when you plug in a new device. When this happens, the process is done and the controller is reflashed.

To check that your controller is being recognized _as_ a controller, hitt Win+R and run `joy.cpl` to open the USB Game Controller setup window:

![image](Images/Running%20JoyCPL.png)

And if you see "Pico" show up as a device, you've done it correctly.

![image](Images/Pico%20Device%20Window.png)

If not, who knows where you biffed it.


# Controller Setup

## Setting up the controller for Steam Games with SteamInput
* (This is where the Steam Input guide for Rivals and Rushdown Revolt will go if Xinput isn't functional soon.)

## Bugs in SteamInput that we get to contend with
* (This is where I point out and talk about the work arounds for the 2 main bugs you run into when setting up SteamInput, being the stick axis only being bindable once, and the need to bind the right trigger last to be able to save it)

## Dolphin and Slippi setup
To use Haybox firmware on Dolphin and Slippi, I reccomend checking out Haystacks guide on the [Haybox repo.](https://github.com/JonnyHaystack/HayBox) At least until I get around to making one myself.

## Console mode functions

Haybox Firmware supports a wide variety of consoles, most of which it detects and sets automagically on it's own. When plugging into a PC, Wii, Gamecube, or N64, it should just work.

But, to use on the Nintendo Switch, you have to hold 'X' on plug in.

![image](Images/Switch%20Mode.jpg)

## Game Mode Selections

Haybox Firmware is pretty unique in that you can swap between controller game modes on the fly without having to hold anything on plug in. Instead, at any point when the controller is plugged in, you can hit any of these 3-Button combinations to swap between modes.

 * Mod X + Start + L - Melee Mode
 * Mod X + Start + Left - Project M/Project+ Mode
 * Mod X + Start + Down - Smash Ultimate Mode
 * Mod X + Start + Right - Tradition Fighter Hitbox Mode
 * Mod X + Start + B - Rivals of Aether Mode (Works as the Rushdown Revolt mode too)
* Mod Y + Start + L - Default Keyboard Mode

And for the version of the Firmware that I provide, I include my custom Guilty Gear Strive keyboard mode.

* Mod Y + Start + Right - Strive Keyboard Mode

By Default, the Melee mode is selected. Except when plugging in to a Switch where it Defaults to the Smash Ultimate mode.


# BubbleBox Customization and Features

## Layout

![image](Images/BubbleBox%20Layout.jpg)

The BubbleBox uses a Layout that is very similar to a normal B0XX/Frame1/LBX

## Firmware

The BubbleBox uses a [modified version](https://github.com/UMS-Ultra/BubbleBox-Firmware) of the Haybox firmware made by [JonnyHaystack](https://github.com/JonnyHaystack). Haybox has a lot of lovely features, and can be used on PC, Linux, N64, Gamecube, Wii, Switch, and through Gamecube Controller Adapters on things like the Wii-U. It is a very modular firmware that, with very low coding knowledge, can be endlessly customized and tweaked. While it doesn't have runtime Remapping, changing the pinouts to remap buttons is very straight forward. There are also a lot more premade game modes for games like Nickelodeon All Star Brawl, MultiVersus, and other platform and fighting games that just need to be bound to a 3-Button combination. For a more more information on how to customizing the Firmware to your own liking, check out the full [Haybox github repository.](https://github.com/JonnyHaystack/HayBox)

## Select and Home buttons

Haybox firmware supports 2 extra buttons for Select and Home which is very useful for games where they are important. Like most fighting games that have training modes. Because the normal Gamecube Controller doesn't actually those 2 buttons, they are bound to Dpad Left and Right which are save and reset in Uncle Punch when in the Melee mode.

## Modularity

Outside of the Haybox Firmware which empowers digital features, the BubbleBox on it's own has been designed to be very modular and very simple to assemble. While it does still require soldering to wire everything up, which can be a bit daunting for people who haven't done it before, the case and keycaps can all be made on any home 3D printer with a build volume of at least 12in/310mm x 6in/150mm. A split case design that can be made on a Prusa Mini or Ender 3 is being worked on.

The large amount of Modularity in the Design also means that versions with different button layouts are very easy to produce, and I intend to make premade print files to support a wide Variety of hand types and layouts. The only limiting factor is that, for now, firmware that supports these layouts is a little more advanced to make and those are skills I currently lack. One of the biggest requests for customizations is the addition of a "W" key, a second Up Key in the same layout as WASD/Arrow keys on a keyboard, and is being worked on. Another big plus to my files modularity and simplicity, is that left handed versions are also very easy to produce for the people out there born with that very unfortunate disability. As such, every version of the Bubble Box will include Left handed versions. Completely _Ambidextrous_ versions get a bit more tricky, but are still technically possible.

## Switch Sockets

The BubbleBox 1.0 uses hotswap sockets for the keyboard switches that allows the user to quickly and easily remove and replace said keyboard switches. Very handy, and very nice for those keyboard nuts out there that like ever switch to be hand lubed with there owl gold plated 63gram springs or whatever. Go ham. Get your Thock.

![image](Images/MX%20Switch%20Socket%20Example.jpg)

Because of the orientation the BubbleBox prints in, making reliable sockets without a seperate switch plate for the switches to mount into is a little tricky. But I have solved this using some special print geometry that forces a slicer to use better bridges to get the surface of the socket to print without supports.

![image](Images/Slicer%20Bridge%20Example%201.png)
![image](Images/Slicer%20Bridge%20Example%202.png)

However, with a printer that doesn't print bridges very well, it can ruin a case. Thankfully most printers nowadays can do it no problem, with little to no tuning. But, included in the files is a test piece that you can print out and inspect to make sure your slicer profile is correct and your printer is up to the task. Make sure you check out the recommended print settings too. The case and the keycaps where designed to be printed with a 4mm nozzle and a .2mm layer height. The Nozzle Size is probably fine to be adjusted, but for the Case, it's the layer height that is crucial to the special print geometry.

![image](Images/Inverted%20Socket%20Coupon.PNG)

Alternatively, there are versions of the case that do not include these inverted sockets. They forego the main body of the switch socket, and leave the button of the switches and their pins bare inside the case. You can still use the hotswap sockets because it makes soldering easier and retains the ability to easily _remove_ switches.

![image](Images/Socketless%20Switch%20Socket%20Example.jpg)

The socketless version of the BubbleBox is also compatible with Low Profile Gateron switches. If you use these though, you will probably need different hot swap sockets because the normal MX style hot swap sockets are the wrong size and you'd really have to jam em on to get it to work.

![image](Images/Low%20Profile%20Switch%20Example%20Front.jpg)
![image](Images/Low%20Profile%20Switch%20Example%20Back.jpg)

## USB-C

The BubbleBox uses is the USB-C port from the [Bird-D Breakout board](https://github.com/HTangl/Model-UD). It is compatible pretty much any normal USB-C Cable to plug into PC or Switch, and it is compatible with USB-C to Gamecube cables to plug into Gamecube, Wii, and GCC adapters. It is also compatible with Smash64 through a USB-C to N64 cable if that's your thing. 

![image](Images/USBC%20BirdD.jpg)
![image](Images/USBC%20Front.jpg)

# Variations

* Standard BubbleBox with Switch Sockets
* Standard BubbleBox without Switch Sockets
* Left Handed BubbleBox with Switch Sockets
* Left Handed BubbleBox without Switch Sockets

Ther are also a few more variations in the works.

* Upcoming Split case that cane be printed on smaller printers, aiming for Prusa Mini sized chunks
* Upcoming BubbleBox with W key, w&w/o switch sockets, L/R Handed versions
* Upcoming H-tangled version that is smaller, w&w/o switch sockets, L/R Handed versions
* Upcoming Big Hand Reverse Htangle version that is the same case size as the Standard BubbleBox, but where the movement hand row is moved up one and the thumb clusters are moved more inward, w and w/o switch sockets
* Upcoming versions with extra 15-30 degree _cant_ between the top and bottom rows for better ergonomics maybe we'll see.

# Keycaps

In this repo you'll find print files for my variation of 3D Printable Keycaps. There are 3 Styles right now: Round, Hex, and Square. Round is the most standard, Hex is nice for pressing multiple buttons with one finger, and Square is just kinda neat. To fully equip a full BubbleBox, you will need 22 total for Round and Hex, and for the Square you will need 15 20mm Square, and 7 of the Truncated Square or 19mm Square keycaps for the thumb clusters as those keys come closer together than any of the other ones and will rub if you use the full sized keycaps. You will also want to print a few extras, incase any break during heavy use or come off the printer weak.

![image](Images/BubbleBox%20Black%20and%20Light%20Grey%20Hex%20Keycaps.jpg)
![image](Images/BubbleBox%20Black%20and%20Light%20Grey%20Round%20Keycaps.jpg)
![image](Images/BubbleBox%20Black%20and%20Light%20Grey%20Square%20Keycaps.jpg)

You can also Mix 'N Match as you please.

![image](Images/Chex%20Mix%20Keycaps.jpg)

The stems require a high degree of dimensional accuracy, make sure your printer is not over extruding at all or you're going to have a bad time.

![image](Images/Keycap%20Underside.jpg)

These keycap designs are Flat Faced with a chamfilleted edges (Half chamfered, Half Filleted for 3D printing reasons), which some people might not not find to their liking. Any MX compatible keycaps should work if you do not want to print these and are into that style. I plan to offer convex and concave keycaps too, but they are difficult to print on a hobby-grade printer. I have further plans to make versions that could be professionally printed in Nylon or Resin from JLC or wherever.

## The Interesting Nuance of the Truncated Keycaps

The Square Truncated keycaps come with one side shortened are designed to be installed in such a way to allow more vertical distance between the A & C-Up Buttons, and the C-Down & C-Left Buttons.

![image](Images/Thumb%20Clusters%20with%20Square%20Keycaps.jpg)
![image](Images/Thumb%20Clusters%20with%20Square%20Truncated%20Keycaps.jpg)

I dunno why, but the B0XX, Frame 1, and LBX all do this for some reason. Some say this extra distance can be more comfortable for some people, so I included them.

# Bill of Materials

## Screws

* 9x  M3x6mm Button Head Cap Screws
* 9x  M3 Initeq Heatset Threaded Inserts (Other inserts can work too, but will need to have their hole sizes adjusted)
* 2x  M3x4mm Button Head Cap Screws or Socket Head Cap Screws
* 2x  M2x6mm Socket Head Cap Screws or Button Head Cap Screws
* 2x  M2 In-Sail Heatset Threaded Inserts (Optional)

## Electronic Components

* 1x  Raspberry Pi Pico
* 1x  Bird-D USB-C Breakout Board

## Wire and Glue

* 25ft/8m appox. of 22/24/30awg Softcore Wire. Solidcore works too but can be harder to work with.
* 1x Bottle of Medium/Thick CyanoAcrylate Glue (C.A. Glue or just Super Glue)

## Switches

* 22x Gateron Hotswap Sockets (Kailh might work, I haven't tested), or Low Profile Gateron Hotswap Sockets if using low profile switches in a socketless BubbleBox
* 22x MX Style Switches of your choice

## Printed components

* 22x Printed Keycaps or Other Keycaps of your choice
* 1x  BubbleBox Case
* 1x  Case Bottom Panel


# Tools Required for Assembly

* Soldering Iron, to solder and insert heatset threaded inserts, threaded insert soldering iron tips to insert the threaded inserts is helpful but optional
* Wire Strippers or Utility Knife & Wire Cutters, to cut and strip wires
* 2mm and 1.5mm Hex Wrench, to screw screws
* Keyboard Switch Puller, to pull the keyboard switches if you need to
* Small Needle Nose Pliers or Tweezers, to tweeze and plie as needed. Useful for inserting the hotswap sockers and holding wires when soldering
* Helping Hands can help with soldering wires if you need them

## Print settings

As mentioned above, the files are made to print with a .4mm nozzle at a .2mm layer height. I print in Polymaker ABS and ASA at with 265C nozzle and 110C bed. You really need to make sure your first layers are tuned in, and that large prints aren't going to warp on your printer. I pretty much exclusively print in ABS and ASA, so anything else like PLA and PETG mway work but is "Your Milage May Very" and you gotta watch out for warping if a case printed in less heat-resistant materials. Materials like these will likely be ruined if left in direct sunlight or in a car on a hot day. 


# Assembly Instuctions

 ## 1:  Print your case components and Keycaps, and gather your materials and tools

![image](Images/Grey%20Case%20on%20Print%20Bed.jpg)
![image](Images/Hex%20Keycap%20Print%20Plate.jpg)

 ## 2:  Install Heatset Threaded inserts in their correct holes.
 The 9 M3s go into the 4 along the top, the 4 Along the Bottom, and the one in the Center.

![image](Images/M3%20Insert%20Locations.jpg)
 
 The 2 M2s go into the posts with the larger holes to mount the Pico.

![image](Images/M2%20Insert%20Locations.jpg)
 
  If you're not using threaded inserts to help mount the Pico, the 2 posts with Smaller holes are sized to directly accept the M2 screws. Just don't screw them too tight or you'll strip the plastic. Less than 0.1 Uggas of torque is required to keep the Pico in place.

 ## 3:  Glue Hotswap Sockets into the switch sockets.
 Yes there are two things called sockets, blame Gateron and Kailh for that.
 Every switch socket needs a hotswap socket super glued into the 2 holes. They need to be in the right orientation or the hotswap sockets will prevent the switches from being installed

![image](Images/Correct%20Hotswap%20Socket%20Orientation.jpg)

 ## 4:  Solder a short wire onto the Pico between the AGND to any GND pin.
 I typically run this wire from pin 8 to pin 33 accross the backside of the Pico. I do not understand why, but people smarter than me say it's important for magic electricity reasons.

 * `(Remember to add photo of the AGND and GND connection)`

 ## 5:  Connect the Pico to the Bird-D.
 I typically run about 5-6in/120mm-150mm lengths of wire to connect the Pico and the Bird-D Breakout Board. There are 6 total connections you will need to make.
 1. TP2 on the Pico to D- on the Bird-D
 3. TP3 on the Pico to D+ on the Bird-D
 3. GP28 on the Pico to GCD/D3V on the Bird-D
 4. VBUS on the Pico to 5V on the Bird-D
 5. VSYS on the Pico to 3V on the Bird-D
 6. GND(I use pin 38 or 33) on the Pico to GND on the Bird-D

 ![image](Images/Wiring%20Diagram.jpg)

 When done correctly it should look something like this:

![image](Images/Wired%20BirdD.jpg)
 * `(Remember to udate this photo later with just a Pico wired to a Bird-D)` 

 ## 6:  Verify that the USB-C connection is working.
 At this point, it is good to check that everything is working by plugging into your PC through the freshly installed USB-C port. If it's a new Pico, then it should register as a storage device on your computer. If you haven't done so already, now is a good time to install the firmware using the guide at the top of this readme.

 ## 7: Next we gotta solder the Signal wires to the Pico.
 These will run from the Numbered GPIO Pins on the Pico, to one side of their respective hot swap socket. These wire lengths are slightly over sized, so you have a little bit of wiggle room, and so you can trim them later if you want to.

    1.  Solder 8in/200mm length wire to pins GP17(Up), GP18(MS), and GP5(L/LT)
    2.  Solder 7in/175mm length wire to pins GP19(Z/RB), GP20(LS), and GP4(Left)
    3.  Solder 6in/150mm length wire to pins GP21(X), GP22(Y), and GP3(Down)
    4.  Solder 5in/125mm length wire to pins GP27(R/RT), GP26(B), and GP2(Right), and GP10(Select)
    5.  Solder 4in/100mm length wire to pins GP16(C-Right), and GP11(Home)
    6.  Solder 3in/75mm  length wire to pins GP6(ModX), and GP7(ModY)
    7.  Solder 2in/50mm  length wire to pins GP14(A), GP12,(C-Up), GP13(C-Left), and GP0(Start)
    8.  Solder 1in/25mm  length wire to pins GP15(C-Down)

 * `(Remember to add photo of Octopus Pico with all the wires flopping around)`

 ## 15: Mount Pico and Solder Signal wires to the Switch Sockets.
  Once every wire is soldering onto every relevant pin on the Pico, you can do some wire management, screw the Pico onto it's mount, trim any excess length of wire you desire for aesthetics or to ease routing, and solder ever wire to one side of its buttons hotswap socket. Making extra damn sure you don't trim the wrong wire or solder any wires to the wrong switches because at this point it'll be a pain in the ass to fix it.
 
![image](Images/Pico%20Signal%20Lines.jpg)
 
 ## 15: Solder the Ground Loop.
 I use 2x 5in/125mm lengths of wire for reaching between Right and Mod X, and between Mod Y and C-Down. Then 19x 3in/75mm lengths of wire between every other switch, and 1x 3in/75mm length of wire between GND pin 23 and the ground side of the Mod Y socket.
 
![image](Images/Pico%20Ground%20Loop.jpg)

 ## 16: Install all 22x switches into their sockets.
 You have to make sure to orrient them correctly otherwise you will mash up the pins on the switches. Once they are installed, you can install the keycaps.

 ## 17: Test everything out.
 Once you verify everything is functioning, you're done constucting your BubbleBox!
 ___
## Adding Gription

When resting the controller on your lap, you might find that with bare plastic it's a bit slick and slips around. The entire controller will probably weigh less than a pound, as all of mine do, so you're not getting any help there either. You have a couple options though. So far, my #1 recommended solution if you're doing this at home is to get some 8x12 sheets of adhesive EVA Foam Paper, and cut out a sheet that fits the bottom panel, and slap it on the bottom. I use this material for my controllers, except I laser cut it.

![image](Images/Cut%20EVA%20Foam%20Grip%20Sheet.jpg)

Alternatively, you could also get some phone grip tape or other rubbery grip tapes. This is generally a soft-ish rubber material (not like skateboard sandpaper grip tape, unless you're into that I suppose). I find this doesn't work as well as the EVA Foam, but it's another option.

![image](Images/Old%20BubbleBox%20Purple%20Phone%20Grip%20Tape.jpg)

# Contributions
[Haybox Firmware](https://github.com/JonnyHaystack/HayBox) from [Haystack the Goat](https://github.com/JonnyHaystack)

[Hadoe](https://github.com/HTangl) and [Crane](https://github.com/Crane1195) for the [Bird-D USB-C Breakout Board](https://github.com/HTangl/Model-UD)

Cranes Lab Discord server