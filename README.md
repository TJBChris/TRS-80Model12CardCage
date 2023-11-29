# TRS-80 Model 12 Card Cage

## About
This is a crude card cage replacement for the TRS-80 Model 12 business microcomputer.  The Model 12 did not include the seven-slot card cage by default; it was available as an add-on.  Its bigger borthers (the TRS-80 Model 16B and later the Tandy 6000) include this cage.  This project should also be usable in those machines should you find yourself with a pillaged system.  Naturally, you'll need a seven-slot backplane in order for this to be useful.

Please note this is only the second thing I've ever "made".  It's also the first multi-part "thing" I've made.  I'm still learning and am very new at this.  It shows.  Even so, this is a crude-but-servicable item.  As such, you should expect that things aren't perfect and I may not be able to fix issues in a short time.  But, in the spirit of open source, if you find areas you'd like to improve and have more experience than I, feel free to fork the project, make your improvements, and submit a Pull Request back to me.  I'd be happy to incorporate any fixes you may have.

This project assumes a basic familiarity with 3D printing and working with computers of the Model 12's vintage. This documentation is written from that perspective.

My YouTube videos for this project can be found here: https://youtube.com/playlist?list=PLNLZVk0TSZFJRB-gEgNvk96HBEzzWrhk3&si=kmpUlS4L6hQPK3qs

The videos also contains some detail on the caveats below.

## Differences from Tandy's Cage

This cage is different from the Tandy design in the following ways:

* It is missing the **card stop** that stops one from inserting a card into the slot at an angle.
* It lacks the **screw-on braces** which attach at the rear of the cages to hold the cards in place.
* The top does not have the **rear overhang** which meets with the backplane.
* It's not metal (and thus won't help you in the RFI department, and it creates some additional considerations around grounding).

## What you'll need

To make this cage, you'll need:

* A seven-slot backplane for your TRS-80 Model 12.
* A 3D Printer with sufficient volume.  I'm using an Anycubic Kobra Plus.  You can also have it professionally printed; I've not tried this yet...YMMV.
* Slicing software.  I'm using Ultimaker Cura.  
* PLA or the material of your choice.  I've used PLA thus far with success.
* PCB board guides (14 total; 7 per side).  I used DigiKey P/N **36-8623-ND** (made by Keystone Electronics, part #8623).  The guide holes in the cage are spaced for these particular guides.  This link was valid as of this writing: https://www.digikey.com/en/products/detail/keystone-electronics/8623/317060?s=N4IgTCBcDaIMwDYC0AOBY5IHIBEQF0BfIA
* M3 screws and matching nuts to attach the cage to the backplane.  The screw holes in these parts are sized with the major diameter of M3 screws in mind.  I used this 280-piece set from Amazon: https://a.co/d/1WeQXiK
* Optionally, threadlock to secure the screws and nuts.
* Six screws to attach the cage to the chassis of the system.  Metal is recommended here; you can re-use the screws currently holding the Model 12's existing metal housing, as you'll be removing it.

## Making and Using the Cage

There are three STL files here, one for each side. Slice them according to your material and printer (I use Ultimaker Cura for this task) and print them one-at-a-time.  I use the following settings:

* Infill Density: 20%
* Infill pattern: triangle (grid also seems to work well)
* Print temp: My PLA has a range from 200-210 C, I print at 200 C.  Your temp will vary based on material.
* The default orientation of the STL files should avoid the need to print supports.

After printing, you may find the screw holes may have material preventing you from inserting the screws; a stright pick should allow you to work the excess material out.  I routinely run the pick through each screw hole before attempting to assemble it to make life easier.

Once printed, put it together:

* Attach the PCB card guides to the cage sides.  You may want to use glue or another adhesive, though I've found the DigiKey guides noted above snap in and reimain in place without glue.
* Attach the sides to your backplane using M3 screws and nuts.  You'll note that the screws are smaller than the holes in the Model 12 backplane; this is intended to allow you some wiggle room to adjust in case the width is a milimeter off in any direction.  This also helps to account for any variation in printing.  With my printer, for example, the parts are rarely perfectly straight, and this may affect your ability to insert/remove cards.
* Attach the top, again with four M3 screw/nut pairs.
* Disconnect and remove the video card from the Model 12.
* Test card fit by using the video card and attempting to insert it into each of the slots.  Loosen the screws/nuts where needed to adjust the alignment as-needed for best fit.
* Remove and disassemble the existing metal cage holding the cooling fan from your Model 12.  Set the fan aside, along with its screws/nuts.  (See **Caveats** below). 
* Attach the printed cage to the chassis and screw it in place, ensuring any factory grounds are installed between the metal chassis and the cage sides.  Use the screws you removed from the metal cage.  **You may find the metal doesn't line up perfectly; my 16B looks as though it had been "tweaked" (bent) a bit to fit Tandy's card cage; use the screw holes to trim out as best as you can, and don't be afraid to adjust the chassis a bit.
* Make and run your grounding solution (providing spade terminals onto which the keyboard and video ground cables can be attached).
* Install the fan on the outside of the cage using the screws that you removed earlier.  Be sure the airflow is directed toward the back of the drives (so the fan pulls air through the cage, rather than pushing air into it).
* Crete and run your power harness; my Model 12 does not have the spare connector.  YMMV.
* Insert the video card and any other cards you have.
* Enjoy the feeling of running a non-neutered Model 12!

## Caveats And Considerations

Please note the following considerations:

* **Grounding** You will need to provide grounding for the keyboard and video connectors.  The Tandy cage is metal, and contains spade connectors onto which you can attached the grounding leads.  You'll need to provide a way to ground these connectors.  Additionally, there are a couple of chassis ground leads that you'll need to make sure are attached as you install the card cage into your Model 12.
* **Heat** For a setup with a one-three cards, the existing fan should suffice.  It's worth noting the Tandy card cage design did not allow for proper heat dissipation in the Models 12 and 16B; as a result, a modification often referred to as the **Turbo Fan Mod** became popular.  This was accomplished by cutting a large hole into the back cover of the system and attaching a 120V fan to the cover.  The fan was then wired to the AC line voltage at a terminal block by the power supply.  The system can easily overheat if you don't mitigate heat issues.  If you're planning to load up the expansion slots with cards, you should strongly consider doing the Turbo Fan Mod.  There is a 3D-printable rear panel replacement on Thingiverse (not my project).  It has space for two fans.  See: https://www.thingiverse.com/thing:5172782
* **Fit** Variataions in your printer, material, and the demensions of the system chassis and backplane may lead to situations where parts don't quite align perfectly.  As an example, the backplane in my Model 12 has a slight curve to it, and the metal chassis in the system is not perfectly straight.  I've tried to take this into account, but you may need to finagle things a bit or adjust hole sizes to fit your paritcular system.  Similarly, the chassis in my 12 was bent slightly outward in such a way that things didin't fit quite right.  My 16B, which has a factory-installed card cage, looked as though the chassis had been bent to fit the cage.  You may have to...adjust...things a bit for a best fit.  This is a situation where manufacturing variations may come into play...

## License / Copyright

 TRS-80 Model 12 Card Cage © 2023 by TJBChris (Christopher Hyzer) is licensed under CC BY-NC-SA 4.0 
