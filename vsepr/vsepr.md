# Local geometry

The arrangement of atoms and lone pairs around a central atom defines a specific **local geometry**. The valence-shell-electron-pair-repulsion (VSEPR) model can predict these geometries. In this tutorial, you will:

- view the three-dimensional structure of molecules that illustrate various local geometries
- draw the projection of each molecule's structure, as it appears from different perspectives

Before you start, make sure you have cloned the entire `Chem122-2016` repository into your Cloud9 workspace, which includes a Jmol server.


## Start a JSmol web app

Change into the directory `vsepr`. List its contents. These are all MOL files containing models of single-center molecules. Then change back to the parent directory.

```bash
    $ cd vsepr
    $ ls
#   CH4.mol  NH3.mol  NO2.mol  NO3.mol  OCN.mol  PCl5.mol  SF4.mol  SF6.mol  XeF4.mol  vsepr.md  water.mol    
    $ cd ..
```

 and confirm that the file `jmol-console.html` exists. Open this file using the command `c9 open`.
 
 ```bash
    $ ls
#   README.md  jmol-console.html  molvis-tools/  orbitals/  shape/  vsepr/  welcome/
    $ c9 open jmol-console.html
```
 
The code in this file defines a web app based on a visualization library called JSMol. To run it, go to the Cloud9 menu and select **Run > Run with... > Apache**; or click the **Run** button if it is available. This should cause a new console to appear, with the message `Starting Apache httpd, serving ...` and showing a link. Click on the link and open it (or copy and paste the link into a new tab. A new browser tab should open and display the web app. By default, it should show a 3D representation of caffeine. 

## Rotate a molecule in JSMol

### Using the Jmol console interface (with Jmol script commands)

In the Jmol console to the right, enter the command `rotate z 10` and press Enter. The model should rotate within the screen plane by 10 degrees. Enter the command `rotate y 30`. The model should rotate out of the screen plane, about a vertical axis, by 30 degrees. Repeat this command two more times until you are looking at the model on edge. Use `rotate z 30`, three times, to rotate the model in the screen plane until it is oriented horizontally. It should still be presented on edge. Finally, use `rotate x 30`, three times, to rotate the model about a horizontal axis, until it is lying in the screen plane again.

### Using mouse/touch interface

Hold down the `option` key and click-drag left-to-right. The model should rotate within the screen plane, as above. Move the cursor to the left side of the canvas, and click-drag left-to-right. The model should rotate about a vertical axis; rotate 90 degrees until you are viewing the model on edge. Use the `option`-click to rotate in the screen plane until it is oriented horizontally but still presented on edge. Finally move the cursor to the top of the canvas, and click-drag top-to-bottom. The model should rotate about a horizontal axis, until it is lying in the screen plane again.

## Zoom a model

In the console to the right, enter `Zoom 80`. The molecule should zoom out, to 80% of its original size. Enter `Zoom 125` to zoom in to 125% of its original size. Hold down the `shift` key and click-drag up and down; this should zoom in and out.


## Save a static image

Rotate the molecule until you like the perspective. In the Jmol console to the right, enter the command `write image caffeine.png`. JSMol will generate an image and prompt you to download to your computer (if you want). 


## Displaying a different molecule

The `vsepr` directory contains several files with a `.mol` ending. You can tell the Jmol console to focus on this directory using the `cd` cinnabd. They are **Molfile**s, each containing the coordinates of a molecule. For example `OCN.mol` contains coordinates for OCN<sup>-</sup>. You can display the molecule in any Molfile by using the `load` command. Use the `centerat` command to set the origin to the center of gravity (i.e., average) of the molecule.

```Java
    cd vsepr
    load OCN.mol
    centerat average
```

(If in doubt, switch back to the Cloud9 console and use `ls` to find out what Molfiles are available.)

## Exercise: Visual conventions for molecular structures

Chemists have developed visual conventions to show how a geometrical arrangement looks from different angles. We will practice using these conventions by sketching common views of different molecules. Here are a few common conventions. They correspond roughly to principles of drawing in perspective.

- If a bond is coming toward you, out of the plane of the page, draw it as a wedge.
- If a bond is receding into the distance, into the plane of the page, draw it as a dotted line.
- If a bond is coming toward you, or receding into the distance, it should appear shorter than if it were in the plane of the page.
- Atoms and bonds closer to you should obstruct your view of atoms and bonds that are further away. 

Load each of the Molfiles in `vsepr/`. Follow the directions in class for orienting each molecule and then sketching it.

