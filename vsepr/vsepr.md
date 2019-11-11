# Local geometry

The arrangement of atoms and lone pairs around a central atom defines a specific **local geometry**. The valence-shell-electron-pair-repulsion (VSEPR) model can predict these geometries. In this tutorial, you will:

- view the three-dimensional structure of molecules that illustrate various local geometries
- draw the projection of each molecule's structure, as it appears from different perspectives


## Jmol Console tutorial

**Jmol Console** is an implementation of the open-source JMol/JSMol Project. Jmol allows you to build, rotate, and observe spatial models of molecules, orbitals, and composite structures such as proteins and crystals; the Console interface enables precise and reproducible control of the models. 

### Start Jmol Console

Simply point your browser to the URL: [garcias.github.io/jmol-console/](https://garcias.github.io/jmol-console/). A web app should start up within 1 or 2 seconds. By default, it should show a 3D representation of caffeine on the left, with two panes on the right. These panes are the console interface. You type commands in the top pane, and messages from JMol will appear in the bottom pane.

### Rotate a molecule in JSMol using the console interface

1. In the Jmol console, enter the command `rotate z 10` and press Enter. The model should rotate within the screen plane by 10 degrees.
2. Enter the command `rotate y 30`. The model should rotate out of the screen plane, about a vertical axis, by 30 degrees. Repeat this command two more times until you are looking at the model on edge. 
3. Use `rotate z 30`, three times, to rotate the model in the screen plane until it is oriented horizontally. It should still be presented on edge. 
4. Finally, use `rotate x 30`, three times, to rotate the model about a horizontal axis, until it is lying in the screen plane again.

### Rotate a molecule in JSMol using the mouse/touch interface

1. Hold down the `option` key and click-drag left-to-right. The model should rotate within the screen plane, as above.
2. Move the cursor to the left side of the canvas, and click-drag left-to-right. The model should rotate about a vertical axis; rotate 90 degrees until you are viewing the model on edge. 
3. Use the `option`-click to rotate in the screen plane until it is oriented horizontally but still presented on edge. 
4. Finally move the cursor to the top of the canvas, and click-drag top-to-bottom. The model should rotate about a horizontal axis, until it is lying in the screen plane again.

### Zoom a model

1. In the console to the right, enter `Zoom 80`. The molecule should zoom out, to 80% of its original size. 
2. Enter `Zoom 125` to zoom in to 125% of its original size. Hold down the `shift` key and click-drag up and down; this should zoom in and out.

### Save a static image

1. Rotate the molecule until you like the perspective. Enter the command `write image caffeine.png`. JSMol will generate an image and prompt you to download it to your computer. Open the file and verify that it resembles the scene in Jmol Console.
2. Enter the same command, but append the letter "t" at the end: `write image caffeine.pngt`. When prompted to download the file, delete the letter "t" at the end so the name is now "caffeine.png". Download the file and open it. This time the background should appear transparent, which is useful for pasting into other scenes.

### Display a different molecule

1. This site contains contains several files with a `.mol` ending. You can tell Jmol Console to focus on this URL using the `cd` command. 
2. Load a file using the `load` command as shown below. Each **Molfile** contains the coordinates of a molecule. For example the file `OCN.mol` contains coordinates for OCN<sup>-</sup>.
3. Use the `centerat` command to set the origin to the center of gravity (i.e., average) of the molecule.

```Java
    cd https://garcias.github.io/Chem122-2016/vsepr/
    load OCN.mol
    centerat average
```

## Exercise: Visual conventions for molecular structures

Chemists have developed visual conventions to show how a geometrical arrangement looks from different angles. We will practice using these conventions by sketching common views of different molecules. Here are a few common conventions. They correspond roughly to principles of drawing in perspective.

- If a bond is coming toward you, out of the plane of the page, draw it as a wedge.
- If a bond is receding into the distance, into the plane of the page, draw it as a dotted line.
- If a bond is coming toward you, or receding into the distance, it should appear shorter than if it were in the plane of the page.
- Atoms and bonds closer to you might obstruct your view of atoms and bonds that are further away; offset them slightly to avoid this loss of information, even if doing so distorts the perspective.

Load each of the Molfiles in `vsepr/`. Follow the directions in class for orienting and sketching each of the molecules:

- [OCN.mol](OCN.mol)
- [NO3.mol](NO3.mol)
- [NO2.mol](NO2.mol)
- [CH4.mol](CH4.mol)
- [NH3.mol](NH3.mol)
- [water.mol](water.mol)
- [PCl5.mol](PCl5.mol)
- [SF4.mol](SF4.mol)
- [SF6.mol](SF6.mol)
- [XeF4.mol](XeF4.mol)

