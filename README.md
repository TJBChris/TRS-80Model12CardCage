# TRS-80 Model 12 Card Cage

**Check out the tandy_emeritus folder Tandy Emeritus-provided resources related to their expansion backplane.**  You can find the TE-designed insulator, which is needed when using their backplane with the original metal Tandy card cage chassis, in this folder.

## About
This is a card cage chassis replacement for the TRS-80 Model 12 business microcomputer.  The Model 12 did not include the seven-slot card cage by default; it was available as an add-on.  Its bigger borthers (the TRS-80 Model 16B and later the Tandy 6000) include this cage.  This project should also be usable in those machines should you find yourself with a pillaged system.  Naturally, you'll need a seven-slot backplane in order for this to be useful.

Please note this is only the second thing I've ever "made".  It's also the first multi-part "thing" I've made.  I'm still learning and am very new at this.  It shows.  Even so, this is a crude-but-servicable item.  As such, you should expect that things aren't perfect and I may not be able to fix issues as quickly as a more-experienced person.  For example, screw holes may not align perfectly, or you may find other issues.  But, in the spirit of open source, if you find areas you'd like to improve and have more experience than I, feel free to fork the project, make your improvements, and submit a Pull Request back to me.  I'd be happy to incorporate any fixes you may have.

This project assumes a basic familiarity with 3D printing and working with computers of the Model 12's vintage. This documentation is written from that perspective.  If you're new to 3D printing, I'd suggest any one of the plethora of Hello World-style tutorials that are available on the web.

My YouTube videos for this project can be found here: https://youtube.com/playlist?list=PLNLZVk0TSZFJRB-gEgNvk96HBEzzWrhk3&si=kmpUlS4L6hQPK3qs

The videos also contains some detail on the caveats below.

## Differences from Tandy's Cage

This cage is different from the Tandy design in the following ways:

* It is missing the **card stop** that stops one from inserting a card into the slot at an angle.
* It lacks the **screw-on braces** which attach at the rear of the cages to hold the cards in place.
* The top does not have the **rear overhang** which meets with the backplane.
* It's not metal (and thus won't help you in the RFI department, and it creates some additional considerations around grounding).

## Making and Using the Cage

If you don't have your own 3D printer, yours isn't large enough, or you just don't want to babysit your printer for about three days, you can have one of many 3D printing houses print the cage for you.  I've personally used these two with success:

* ShapeWays - https://www.shapeways.com/
	* Material: PA12 (SLS) [Versatile Plastic]
	* Color: Black (Shapeways only allowed black or white for these parts.)
	* Finish: Natural
	* I let Shapeways determine infill and such.  

* CraftCloud - https://craftcloud3d.com/
	* Material: PLA (FDM)
	* Color: Black 
	* Finish: Standard
	* I let CraftCloud determine infill and such.  	

It will probably be fairly pricey to get all three parts printed.  A plastic material with some tolerance for temperature variations would be preferable.  

If you're printing it yourself, check out the **doc/cage** folder for instructions building the cage, along with the required materials and tools.

## Caveats And Considerations

Please note the following considerations:

* **Grounding** You will need to provide grounding for the keyboard and video connectors.  The Tandy cage is metal, and contains spade connectors onto which you can attached the grounding leads.  You'll need to provide a way to ground these connectors.  Additionally, there are a couple of chassis ground leads that you'll need to make sure are attached as you install the card cage into your Model 12.
* **Heat** For a setup with a one-three cards, the existing fan should suffice.  It's worth noting the Tandy card cage design did not allow for proper heat dissipation in the Models 12 and 16B; as a result, a modification often referred to as the **Turbo Fan Mod** became popular.  This was accomplished by cutting a large hole into the back cover of the system and attaching a 120V fan to the cover.  The fan was then wired to the AC line voltage at a terminal block by the power supply.  The system can easily overheat if you don't mitigate heat issues.  If you're planning to load up the expansion slots with cards, you should strongly consider doing the Turbo Fan Mod.  There is a 3D-printable rear panel replacement on Thingiverse (not my project).  It has space for two fans.  See: https://www.thingiverse.com/thing:5172782
* **Fit** Variataions in your printer, material, and the demensions of the system chassis and backplane may lead to situations where parts don't quite align perfectly.  As an example, the backplane in my Model 12 has a slight curve to it, and the metal chassis in the system is not perfectly straight.  I've tried to take this into account, but you may need to finagle things a bit or adjust hole sizes to fit your paritcular system.  Similarly, the chassis in my 12 was bent slightly outward in such a way that things didin't fit quite right.  My 16B, which has a factory-installed card cage, looked as though the chassis had been bent to fit the cage.  You may have to...adjust...things a bit for a best fit.  This is a situation where manufacturing variations may come into play...
* **Power** Your Model 12 may not have the additional harness needed to power the card cage.  My Model 12 is one of these systems.  As a result, you'll need to find a way to get +12, -12, and 5V to the cage along with their grounds.

## License / Copyright

 TRS-80 Model 12 Card Cage © 2023 by TJBChris (Christopher Hyzer) is licensed under CC BY-NC-SA 4.0 
