# BubbleBox 1.0: Digital Controller
 The BubbleBox 1.0 is a Smashbox/F1/B0XX/LBX Style game controller for Platfighters:
 
![image](BubbleBox%201.0/BubbleBox%20Image%201%20Gray%20and%20Pink.jpg)


# Important License Stuff

Yadda Yadda Strongly Recipricol Copyleft License Yadda Yadda if you use and modify these files you are obligated to publish your files under the same license because thats how this works.

* (Don't Forget to finish this. Seems important.)


# Installing and Updating Firmware

When plugging in a new Pico into a computer for the first time, it should open a file explorer window into which you can drop a .uf2 file to flash the pico with that Firmware. It's exactly like putting something on a USB Flash Drive. When done successfully, the LED on the Pico should glow Green and your computer should be the noise that it makes when you plug in a new device. When you want to reflash the pico with newer, shinier, firmware, there are 2 ways. The first way is to hold down the white "bootsel" button on the Pico when you plug it in. If your Pico is already flashed with Haybox firmware, the second way is to simply hold down the Start button on plug in and that will do the same thing as holding the bootsel button.

* (Rememeber to include photos and screenshots of this process and build out this guide a little bit more.)


# Controller Setup and Usage

## Setting up the controller for Steam Games with SteamInput
* (This is where the Steam Input guide for Rivals and Rushdown Revolt will go, as well as the dolphin setup guide for Melee)

## Bugs in SteamInput that we get to contend with
* (This is where I point out and talk about the work arounds for the 2 main bugs you run into when setting up SteamInput, being the stick axis only being bindable once, and need to bind the right trigger last to be able to save it)

## Console mode functions

Haybox Firmware supports a wide variety of consoles, most of which it detects and sets automagically on it's own. When plugging into a PC, Wii, Gamecube, or N64, it should just work. Some consoles and GCC adapters, however, are less cooperative and you have to hold down a button on pluggin to tell the BubbleBox what console it's plugging in to.

To use on the Nintendo Switch, you have to hold X on plug in
To use through a GCC Adapter, you have to hold A on plug in

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

The BubbleBox uses the Haybox firmware made by Haystack. Haybox firmware has a lot of lovely features, and can be used on PC, Linux, N64, Gamecube, Wii, Switch, and through Gamecube Controller Adapters on things like the Wii-U. It is a very modular firmware that, with very low coding knowledge, can be endlessly customized and tweaked. While it doesn't have runtime Remapping, changing the pinouts to remap buttons is very straight forward. There are also a lot more premade game modes for games like Nickelodeon All Star Brawl, MultiVersus, and other platform and fighting games that just need to be bound to a 3-Button combination. For a much more complete guide to customizing the Firmware, check out the full Haybox github repo `(link to Haybox repo)`

## Modularity and Build Simplicity

Outside of the Firmware which empowers digital features, the BubbleBox on it's own has been designed to be very modular and very simple to assemble. While it does still require soldering to wire everything up, which can be a bit daunting for people who haven't done it before, the case and keycaps can all be made on any home 3D printer with a big enough build volume. At least 12in/310mm x 6in/150mm. A split case deisgn that can be made on an Ender 3 or Prusa Mini is being worked on.

The large amount of Modularity in the Design also mean that versions with different button layouts are very easy to produce, and I intend to make premade print files to support a wide Variety of hand types and layouts. The only limiting factor is that, for now, firmware that supports layouts that deviate too much or with too many buttons more than the normal B0XX/Frame 1/LBX style is a little strange to make. But because Haybox is so modular, it's not super difficult to make and modify modes that support layouts with _more_ buttons than the normal 20. One of the biggest requests for customizations is the addition of a "W" key, a second Up Key in the same layout as WASD/Arrow keys on a keyboard. This would be kinda nice, because it's puts an Up input in a more intuitive spot than being way off in Timbuktu on the right pinky. Another big plus to my files modularity and simplicity, is that left handed versions are also very easy to produce for the people out there born with that very unfortunate disability. As such, every version of the Bubble Box will include Left handed versions. Completely _Ambidextrous_ versions get a little more tricky, but are still possible.

## Switch Sockets

The because of the orientation the BubbleBox uses to print, making reliable sockets without a seperate switch plate for the switches to mount into is a little tricky. But I have solved this using some special print geometry that forces a slicer to use better bridges to get the surface of the socket to print without supports. However, with a printer that doesn't print bridges very well, it can ruin a case. Thankfully most printers nowadays can do it no problem, with little to no tuning. But, included in the files is a test piece that you can print out and inspect to make sure your slicer profile is correct and your printer is up to the task. Make sure you check out the recommended print settings too. The case and the keycaps where designed to be printed with a 4mm nozzle and a .2mm layer height. The Nozzle Size is probably fine to be adjusted, but for the Case, it's the layer height that is crucial to the special print geometry.

Alternatively, there are versions of the case that do not include these inverted sockets. They forego the main body of the switch socket, and leave the button of the switches and their pins bare inside the case. You can still use the hotswap sockets because it makes soldering easier and retains the ability to easily _remove_ switches.

## USB-C

The main port on the BubbleBox is the USB-C port from the Model Bird-D. It is compatible pretty much any normal USB-C Cable to plug into PC or Switch, and it is compatible with USB-C to Gamecube cables to plug into Gamecube, Wii, and GCC adapters. It is compatible with Smash64 through a USB-C to N64 cable.

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
* Upcoming versions with extra 15-30 degree cant between the top and bottom rows

# Keycaps

In the files you'll find print files for my variation of 3D Printable Keycaps. There are 3 Styles right now: Round, Hex, and Square. Round is the most standard, Hex is nice for pressing multiple buttons with one finger, and Square is kinda neat. To fully equip a full BubbleBox, you will need 22 total for Round and Hex, and for the Square you will need 15 20mm Square, and 7 of the Truncated Square or 19mm Square keycaps for the thumb clusters as those keys come closer together than any of the other ones and will rub if you use the full sized keycaps. You will also want to print a few extras, incase any break during heavy use or come off the printer weak.

* (Remember to add photos of those 3 Keycap styles)

You can also Mix 'N Match as you please.

* (Remember to add photos of versions that mix 'n match keycap types)

The stems require a high degree of dimensional accuracy, make sure your printer is not over extruding at all or you're going to have a bad time.

* (Remember to add photo of a Stem)

These keycap designs are Flat Faced with a chamfilleted edges (Half chamfered, Half Filleted for 3D printing reasons), which some people might not not find to their liking. Any MX compatible keycaps should work if you do not want to print these and are into that style. I plan to offer convex and concave keycaps too, but they are difficult to print on a hobby-grade printer. I have further plans to make versions that could be professionally printed in Nylon or Resin from JLC or wherever.

## The Interesting Nuance of the Truncated Keycaps

The Truncated Square keycap comes with one side shortened can be installed in such a way to allow more vertical distance between the A Button and C-Up Button, and the C-Down Button and C-Left Button. I dunno why, but the B0XX, Frame 1, and LBX all do this for some reason. Some say it's more comfortable for certain options, but I find it more difficult to plink and piano with my right Thumb so the Keys are layed out in that way, and these square keycaps are the compromise for that. Though, if you ask nicely I can probably make Circular or Hex versions that do more or less the same thing. Or you can edit the CAD files to add this distance between the sockets in the Case itself and have the distance with any keycaps you want.

* (Remember to add photos showing the difference)

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

* 22x Gateron Hotswap Sockets (Kailh might work, I haven't tested)
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
* Helping Hands can help with soldering the wires to the Pico if you need them

## Print settings

As mentioned above, the files are made to print with a .4mm nozzle at a .2mm layer height. I print in Polymaker ABS and ASA at with 265C nozzle and 110C bed. You really need to make sure your first layers are tuned in, and that large prints aren't going to warp on your printer. I pretty much exclusively print in ABS and ASA, so anything else like PLA and PETG mway work but is "Your Milage May Very" and you gotta watch out for warping if a case printed in less heat-resistant materials. They will likely be ruined if left in direct sunlight or in a car on a hot day. 


# Assembly Instuctions

 ## 1:  Print your case components and Keycaps, and gather your materials and tools

   * (Remember to add photo of Case and B Panel on Print bed)
   * (Remember to add photo of keycaps on Print bed)
   * (Remember to add Knilled photo of all Materials for one completed standard BubbleBox)
   * (Remember to add Knolled photo of Tools)

 ## 2:  Install Heatset Threaded inserts in their correct holes.
 The 9 M3s go into the 4 along the top, the 4 Along the Bottom, and the one in the Center. The 2 M2s go into the posts with the larger holes to mount the Pico. If you're not using threaded inserts to help mounting the Pico, the 2 posts with Smaller holes are sized to directly accept the M2 screws. Just don't screw them too tight or you'll strip the plastic. Less than 0.1 Uggas of torque is required to keep the Pico in place.

 * (Remember to add photo of the posts that need inserts and the posts that don't)
 * (Remember to add photo of posts with threaded inserts installed)

 ## 3:  Glue Hotswap Sockets into the switch sockets.
 Yes there are two things called sockets, blame Gateron and Kailh for that.
 Every switch socket needs a hotswap socket super glued into the 2 holes. They need to be in the right orientation or the hotswap sockets will prevent the switches from being installed

 * (Remember to add photo(s) showing correct and incorrect orientation of the hotswap sockets)
 * (Remember to add photo of case with glued in hotswap sockets)

 ## 4:  Solder a short wire onto the Pico between the AGND to any GND pin.
 I typically run this wire from pin 8 to pin 33 accross the backside of the Pico. I do not understand why, but people smarter than me say it's important for magic electricity reasons.

 * (Remember to add photo of the AGND and GND connection)

 ## 5:  Connect the Pico to the Bird-D.
 I typically run about 5-6in/120mm-150mm lengths of wire to connect the Pico and the Bird-D Breakout Board. There are 6 total connections you will need to make.
 1. TP2 on the Pico to D- on the Bird-D
 3. TP3 on the Pico to D+ on the Bird-D
 3. GP28 on the Pico to GCD/D3V on the Bird-D
 4. VBUS on the Pico to 5V on the Bird-D
 5. VSYS on the Pico to 3V on the Bird-D
 6. GND(I use pin 38 or 33) on the Pico to GND on the Bird-D
 * (Remember to add photo of of Pico wired to Bird-D)
 * (Remember to add Arte's wiring photo or to make one yourself) 

 ## 6:  Verify that the USB-C connection is working.
 Plug in the Pico to your Computer through the freshly soldered USB-C port. Then flash the Pico with the provided firmware and verify that it's registering as a controller by hitting Win+R and running `joy.cpl`, if the LED turns Green and it shows up in the device window as "Pico Controller" you've done everything correctly. If not, who knows where you biffed it.

 (Remember to add screenshot of the joy.cpl and pico rectangle windows)

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

 (Remember to add photo of Octopus Pico with all the wired flopping around)

 ## 15: Mount Pico and Solder Signal wires to the Switch Sockets.
  Once every wire is soldering onto every relevant pin on the Pico, you can do some wire management, screw the Pico onto it's mount, trim any excess length of wire you desire for aesthetics or to ease routing, and solder ever wire to one side of its buttons hotswap socket. Making extra damn sure you don't trim the wrong wire or solder any wires to the wrong switches because at this point it'll be a pain in the ass to fix it.
 
 (Insert Photo of Pico with all Soldered Signal Wires)
 
 ## 15: Solder the Ground Loop.
 I use 2x 5in/125mm lengths of wire for reaching between Right and Mod X, and between Mod Y and C-Down. Then 19x 3in/75mm lengths of wire between every other switch, and 1x 3in/75mm length of wire between GND pin 23 and the ground side of the Mod Y socket.
 
 (Inset Photo of Soldered Ground Loop)

 ## 16: Install all 22x switches into their sockets.
 You have to make sure to orrient them correctly otherwise you will mash up the pins on the switches. Once they are installed, you can install the keycaps.

 ## 17: Test everything out.
 Once you verify everything is functioning, you're done constucting your BubbleBox!
 ___
## Adding Gription

When resting the controller on your lap, you might find that with bare plastic it's a bit slick and slips around. The entire controller will probably weigh less than a pound, as all of mine do, so you're not getting any help there either. You have a couple options though. So far, my #1 recommended solution if you're doing this at home is to get some 8x12 sheets of adhesive EVA Foam Paper, and cut out a sheet that fits the bottom panel, and slap it on the bottom. I use this material for my controllers, except I laser cut it.

* (Remember to add photo of laser cut EVA Foam Sheets)

Alternatively, you could also get some phone grip tape or other rubbery grip tapes. This is generally a soft-ish rubber material (not like skateboard sandpaper grip tape, unless you're into that I suppose). I find this doesn't work as well as the EVA Foam, but it's another option.

* (Remember to add photo of the Gator Grips)

# Contributions
lotta stuff to add here eh?