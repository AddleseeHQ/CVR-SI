# Building the CVR-SI

This work has been accepted to be published at EMNLP's Workshop on Natural Language Processing for Positive Impact.

I will be including the following resources in this repository before the paper is published:

## Links to All Required Components
In order to build the CVR-SI, you will need (quantity needed for ONE CVR-SI in brackets):
1. List incoming with links

## Step-by-step Construction Guide (with photos)

Assuming you have all the materials listed above, you should be able to set out your table with them all:
![all materials on the table](./images/1-materials.jpg)

First, you should use the drill with the 12mm drillbit to create a hole in the lid of the case. This hole will be for the button, you MUST do this and put the button in this whole BEFORE soldering. Once the button is soldered to the circuit board, it cannot fit through this hole:
![CVR-SI case with button hole](./images/2-12mm-hole.jpg)

You should also use the 12mm drill bit to make a large hole on the back of the CVR-SI case. This will let the power cable and microphone cable pass through (must be big enough for a USB cable to pass through):
![CVR-SI case with large hole in back for cables](./images/3-cable-hole.jpg)

Then you can switch the 12mm drill bit out for the 5mm drill bit. This is used to drill two smaller holes on either side of the button. Note again that the button is already in place:
![CVR-SI with LED holes](./images/4-5mm-holes.jpg)

Now it is time to plug in your soldering iron, wet its sponge, and gather the cables (note again that the button should already be in the lid - I took this photo earlier):
![cables and soldering iron](./images/5-solder-prep.jpg)

Get the circuit board and fit it in the circuit board holder. You can use the second 'claw' to hold the cable in place while you solder the cable end to the board:
![circuit board in circuit board holder](./images/6-start-solder.jpg)

Solder the board following this circuit diagram:
![rough circuit diagram](./images/circuit-diagram.jpg)

To note, the Raspberry Pi pins are numbered in this diagram. The pins are numbered by the little circles, not the GPIO numbers. Source [here](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html):
![Raspberry Pi pin layout](./images/pi-pins.png)

Once done, the resistor wires will need to be trimmed as they are quite long:
![scissors trimming wires on circuit boars](./images/7-snip.jpg)

You should now have a fully soldered circuit board with the button through the hole in the lid:
![CVR-SI lid and circuit board](./images/8-solder-fin.jpg)

Next we need to attach the correct cables to the correct Raspberry Pi pins (see the circuit diagram for the numbers):
![Raspberry Pi attached to the cables](./images/9-plug-cables.jpg)

The LEDs can now be fixed in place. Put a dab of glue on the bulb edge, and pop them in their holes. It does not matter whether the red or green LED is on the left or right:
![glue next to the CVR-SI lid](./images/11-glue-leds.jpg)

While this is drying, we can get the software ready. Find the SD card of the desired size (16Gb or larger):
![a 16Gb SD card](./images/10-flash-sd.jpg)

You can use any disc burning software, but I use balenaEtcher. Firstly, select the cvr-si.img to be burned on your SD card:
![balenaEtcher settings](./images/10-flash-sd-setup.png)

The software will be burned onto the SD card and then validated:

![balenaEtcher validating](./images/10-flash-sd-verify.png)

Once complete you can eject the SD card:

![balenaEtcher burning completed](./images/10-flash-sd-x.png)

The SD can then be inserted into your Raspberry Pi:
![Raspberry Pi with SD card inserted](./images/12-insert-sd.jpg)

We can now start to put everything together. Put the Raspberry Pi power cable in through the rear hole and into the Raspberry Pi:
![power plugged into Raspberry Pi](./images/13-pi-power.jpg)

Next, unbox the microphone, put the cable through the rear case hole, and plug it into the Raspberry Pi:
![microphone plugged into Raspberry Pi](./images/14-mic-in.jpg)

Apply a light layer of glue to the bottom of the microphone:
![bottom of microphone with glue on it](./images/15-glue-mic.jpg)

Hold microphone down. You will only have to do this for 1-2 mins and then you can let it go and let it set:
![CVR-SI with microphone attached](./images/16-attach-mic.jpg)

Pop the 'lugs' (I don't know the real name) into each corner of the CVR-SI:
![CVR-SI with lugs in place](./images/17-lid-lugs.jpg)

You have to push these down quite hard. Each one should make a loud bang when clicking into place:
![CVR-SI almost complete](./images/18-push-in.jpg)

You can now screw the lugs to secure the lid in place:
![screwing lugs in lid](./images/19-screw-lid.jpg)

And that's it! Your CVR-SI is complete:
![Completed CVR-SI](./images/20-fin.jpg)

## Img Files to Burn Your Own Device
