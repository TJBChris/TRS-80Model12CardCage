# Tandy Emeritus - Related Items

## If you're looking for the Backplane doc, I've been asked to remove it while updates are made.  It will re-appear here soon.  Please check back again!

## About
This page contains items created by Tandy Emeritus in support of their Model 12/16B/6000 backplane.  See the descriptions below for each item here.  I didn't create these items, but it made sense to host them here as part of the larger Model 12 expansion project. 

Please see backplane documentation, **Backplane-Instructions-Rev_B1.pdf**, for complete information on all of the TE components here as well as the backplane itself.  If you have any questions about any of these items, the documentation contains contact information.

## Items

These are the TE-provided items I have here for the card cage project:

* ~~**Backplane-Instructions-Rev_B1.pdf** - Complete assembly instructions and technical documentation for the TE Backplane, Test Fixture, and Diagnostic Spacer.~~
* **BackPlane_Covers_RibbonClip_STLs.zip** - Insulative parts and clips for use with the new Tandy Emeritus backplane to prevent shorts and help with cable management.  There are three parts in the ZIP file:

  **TE-Cage-Insulator.stl** - For use when the TE backplane is paired with the original Tandy metal card cage assembly.  Prevents contact between the card cage top and **This part is not necessary for the 3D-printed card cage in this repository.**  

  **TestFixture-ribbons-clip.stl** - Allows you to clip together the ribbon cables used to extend the system bus from the backplane's connectors out to the Test Fixture assembly.

  **BP_Power-IDE_Cover_V1.stl** - The new backplane has components in places that the legacy Tandy backplane did not.  This part prevents the solder joints for the dual 40-pin bus expansion headers and the power connector from contacting the metal chassis behind the backplane. 
  
* **External_Test_Fixture_STLs.zip** - Contains all of the parts necessary to build a housing for the TE Test Fixture board.  Also contains the cable ribbon clips found in BackPlane_Covers_RibbonClip_STLs.zip.

* **large_bracket_modified.zip** - Contains modified STIL files for the External Test Fixture.  These files separate the lettering from the fixture itself, simplifying printing by allowing you to print the Test Fixture bracket with the large section on the print bed.  The lettering is provided on a separate file, which itself can be printed large-side down.  This eliminates the need for supports to print the lettering.
	**ExtTestFixture_LongSide_noletters_V3.stl** - The modified Test Fixture bracket without lettering.
	**logo_V4.stl** - Side panel including the lettering, which can be attached to the Test Fixture bracket after printing.

## Notes

* All of the STLs that use screws/nuts use M3.  Be sure to use metal screws/nuts.