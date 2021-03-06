# FVTT-Teleport
A module for FVTT to teleport tokens between two points

### Instalation
Manifest: https://raw.githubusercontent.com/knassher/FVTT-Teleport/master/module.json

### How to Use it
On the Note controls there is a new button that toggles the feature to add teleportation points.
On a doble left click over the canvas a new dialog will appear asking for the name of the teleportation point.
if the continue button is hitted the teleportation point will appear, in here someone can choose the destination point that consist of an scene and a teleportation point.
Once a teleportation point is added to the canvas toggle off control button from the note control bar in case is on, then with a double left click you will be teleported to the destination point, with a double right click the config form will be displayed.
if tokens were selected before double clicking a teleportation point, these tokens are going to be carried over to the destination point.

### New Features
* TP config sheet has a new tap called Offsets in which the user can save offsets (as many as you want) for the token when they teleported to that TP. To use this feature just controlle a token or tokens an move it/them to the desire possition, then hit the capture button.
* The middle button of a mouse (wheel button) can be use to start a drag and drop workflow to teleport tokens, just controll a set of tokens, press the middle button and drag those tokens to a TP, once you drop the tokens over the TP those tokens will be teleported to the destination TP.
* A new setting flag was added to the foundry's config to hide tokens from the departed scene when they are teleported to a different scene.
* Added a button to the TP config sheet to highlight the offsets of the TP on the canvas as a visual help.

### Changelog
## V 2.0.5
* Fixed an issue with the TPConfig sheet that didn't render due to changes on FVTT core.
* Fixed an issue that won't trigger TPoints that don't have a scene and/or destination set. 
* A warning message was set up letting know the user that needs to set a scene and/or a destination note.
* Fixed an issue with the toggle button for adding a TPoint, now only one dialog to collect the name of the TPoint will be render after a doble left click.
* Fixed an issue capturing the position for the TPoint.
* Now the TPConfig sheet will be rendered only if the "teleport" key is in the note's flag dictionary.
* Now the TPoint will trigger only if the "teleport" key is in the note's flag dictionary.
* Made some cleaning to the code.

### Dependencies
Modules:
  1.- Furnace 1.3.2 Autor: KaKaRoTo (https://github.com/kakaroto/fvtt-module-furnace)
  
### Special Thanks
The code is based on the pin-cushion module from Evan Clark [errational#2007] (https://github.com/death-save/pin-cushion).
