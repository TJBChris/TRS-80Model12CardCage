# Building the power harness

The power harness should supply ample power for a couple of cards (2-3) in the cage.  As of this writing, more cards haven't been tested.  For a full compliment of cards, you may want to re-work the entire system harness.  Doing so is beyond the scope of this document.

## Tools
The following tools are recommended (beyond a 3D printer and filament, of course):

* A TE crimper or another way to crimp TE pins.
* A soldering iron.
* Solder.
* Heat shrink tubing (approx. 1.9cm and 1.3 diameter).

## Materials
The following materials are required:

### Ground Connectors
* Female terminal connectors (.635cm/.25")
* Male flat terminals (.635cm/.25")

### TE Connectors

The materials required for the power and grounding build are as follows.  You can find them on **DigiKey**.

* Male connector housing: 1-480271-0
* Female connector housig: 1-480270-0
* Female pins: 350550-1
* Male pins: 1062-16-1422

### Tools

The following tools/die sets are recommended.  While you can crimp these connectors without the TE tools, it may prove difficult.

* TE Crimper: 354940-1
* Pinned Die Set: 90546-2

### Wire

It's recommended that you use colored wire in the correct gauge (noted below).  This will greatly lessen confusion.  The recommended colors are noted along with the wire.  **IMPORTANT**: Note that the 5v (red) wire is larger than the remaining conductors.

You'll need the following wire, in the color, gauge and length noted:

* Red: 14 AWG stranded wire.  You'll need 30cm.
* White: 16 AWG stranded wire.  You'll need 30cm.
* Orange: 16 AWG stranded wire.  You'll need 30cm.
* Black: 16 AWG stranded wire.  You'll need 90cm (you're making three sets of cables).

## Assembling the power cable

To assemble the splitter, do the following:

1. Cut the red, white, and orange wire into three sections: One **10cm** length, and two **20cm** lengths.  Group the wires together by color.  For each color, you should have one 10cm length of wire and one 20cm length of wire.
1. Cut the black wire into nine sections: three **10cm** sections, and six **20cm** sections.  Group the black wire into three groups of one 10cm wire and two 20cm wires.
1. For each group of wires, strip off about **2-3cm** of the jacket and twist the strands.
1. For each group of wires, splice together one end of the **10cm** section to one end of each of the remaining two **20cm** sections.
1. Solder the spliced connection.
1. Slide the heat shrink tubing over each section (using the larger diameter tubing for the 14 AWG wire set.)
1. Shrink the tubing with a heat gun or lighter.
1. For each group of wires, crimp a male TE connector to the short lead.
1. Solder the wires to the pins.
1. For each group of wires, crimp female TE connectors to each of the longer leads.
1. Solder the wires to the pins.
1. Using the Model 12 motherboard power harness as a guide, insert the crimped ends into the connector housings.

## Assembling the ground harness

You'll need to reproduce the grounding available with the Tandy cage.  You'll need:

* Approximately **15-20cm** of 16 AWG stranded wire.
* One female terminal connector (.635cm/.25")
* Three male flat terminals (.635cm/.25")

To assemble the harness:

1. Cut the wire into four sections, each approximately **5cm**.
1. Strip about **2-3cm** of the jacket off of each end of each wire.
1. Splice one end of each of the four pieces of wire together.
1. Solder the connection on all sides.
1. Slide heat shrink tubing over the soldered joint.
1. Using a heat gun or lighter, shrink the tubing.
1. Crimp the connectors onto each of the stripped ends.

The female terminal of the ground harness is intended to be attached to the ground spade on the right side of the card cage, where the CRT ground normally attaches.  Attach the CRT, keyboard, and video driver grounds to the male ends.  **Wrap the connected grounds with electrical tape.**