# Drawing molecular structures

## Visual conventions for ball-and-stick notation

Chemists have developed visual conventions to show how a geometrical arrangement looks from different angles. We will practice using these conventions by sketching common views of different molecules. Here are a few common conventions. They correspond roughly to principles of drawing in perspective.

- Draw each atom as a circle, and each bond as a thin cylinder or thick line
- If a bond is coming toward you, or receding into the distance, it should appear shorter than if it were in the plane of the paper.
- If a bond is coming toward you, out of the plane of the page, draw it as a wedge, with the closer end being thicker.
- Atoms and bonds closer to you might obstruct your view of atoms and bonds that are further away.


## Exercise: Drawing with ball-and-stick notation

Load the file Molfile `OCN.mol`:

```Java
    cd https://garcias.github.io/Chem122-2016/vsepr/
    load OCN.mol
    centerat average
```

a. Rotate the molecule OCN<sup>–</sup> until it lies in the plane of the screen (*xy*), with the O atom on the left and N atom on the right (`rotate z 180 spin 100`). Sketch the ball-and-stick representation from this perspective.
b. Rotate about the vertical (*y*) axis by 90 degrees so the CO bond is pointing straight at your eyes, and the other is pointing directly away from you (`rotate y 90 spin 100`). (In other words, the bonds align with the *z* axis. The O atom should obscure the C and N atoms from your perspective. Rotate about the horizontal (*x*) axis, tilting the molecule down so the O atom appears lower than the C atom and the N atom appears higher (`rotate x 30 spin 60`). Sketch from this perspective.

## Visual conventions for Kekulé notation

While ball-and-stick representations show spatial relationships realistically, they have some disadvantages: important atoms and bonds get obscured, and they are slower to draw. Chemists often translate them into **Kekulé notation**, by replacing each circle with the atomic symbol and each bond with simple lines indicating bond order. For single bonds not in the plane of the page, those coming toward you are still wedges, but those going away from you are replaced with a dashed line.

- Draw each atom as its atomic symbol, and each bond as one or more parallel lines indicating bond order.
- If a bond is coming toward you, out of the plane of the page, draw it as a wedge, with the closer end being thicker.
- If a bond is receding into the distance, into the plane of the page, draw it as a *dotted line*. (But in special cases you can draw it as a reverse wedge.)
- Do not allow atoms or bonds to be obscured; offset or distort the perspective slightly to avoid loss of information. (With the usual exception for implicit H or C, or using R as a variable fragment.)


## Exercise: Drawing with Kekulé notation

a. Refer to drawing (a) from the previous exercise above, and redraw with Kekulé notation.
b. Refer to drawing (b) from the previous exercise above, and redraw with Kekulé notation.


## Exercise: Drawing molecules with trigonal geometry (SN=3)

Load the Molfile `NO3.mol`.

a. Arrange so that all 4 atoms lie in the *xy* plane, i.e., the molecular plane is in the screen plane. Draw both the ball-and-stick and Kekulé representations.
b. Rotate so the molecular plane lies in the *xz* plane, i.e., is exactly perpendicular to the screen surface; and with one O atom pointing directly to the right, i.e., one N–O bond aligns with the *x* axis. One of the O atoms should be obscured by another. Draw the ball-and-stick representation.
c. Rotate about the *x* axis 20 degrees, so that the molecular plane tilts down and forms a 20-degree angle with the *xz* plane. All atoms and bonds should now be visible. 
d. Draw the ball-and-stick representation.
e. Draw the Kekulé representation: replace circles with atomic symbols, the front N-O bond with a wedge, and the back N-O bond with a dashed line.


## Exercise: Drawing molecules with tetrahedral geometry (SN=4)

Load the Molfile `CH4.mol`.

a. Arrange so that one bond points straight out of the screen and three others form a tripod pointing into the screen. (Use mouse or touch interface if necessary.) You should see three-fold symmetry. Draw the ball-and-stick representation.
b. Rotate so that two C–H bonds are in the *xy* (screen) plane, one pointing directly up, another to the lower right. The other two bonds should not be in the screen plane.
c. Rotate about the *x* axis -20 degrees, so the "top" C–H bond is still *mostly* pointing up, but tilted slightly toward you out of the screen plane; and so all C–H bonds are clearly visible. Draw the ball-and-stick representation.
d. Redraw with Kekulé notation.
e. Starting with view (b) above, rotate about the *y* axis 90 degrees, so that the C–H that was pointing to the lower right before, is now pointing toward you and slightly downward out of the screen plane. Then rotate about the x axis 30 degrees, so the “top” C–H bond is tilted slightly toward you out of the screen plane. 
f. Draw with Kekulé notation.
g. Rotate CH<sub>4</sub> so that two C–H bonds are in the screen plane, one pointing to the lower left, another to the lower right. The molecule should look as if it stands on two "legs", one to either side; and has two “arms”, twisted 90 degrees from the legs.
h. Draw with Kekulé notation, and be sure to distort the top two "arm" bond so they are not obscuring each other. (It may help to rotate about the *y* axis 10 degrees to see how this should look.)

Load the Molfile `NH3.mol`.

i. Rotate so that one N–H bond is pointing to the lower right in the *xy* plane, and the lone pair (not visible) is pointing straight up.
j. Draw with Kekulé notation, distorting the other two N–H bonds as necessary to show them both.


## Exercise: Drawing molecules with trigonal bipyramidal geometry (SN=5)

Load the Molfile `PCl5.mol`.

a. Rotate so that two bonds lie in the *xy* plane and point directly up and down ("axial" bonds); and three bonds lie in the *xz* plane (equatorial bonds). Rotate about the *y* axis until one equatorial bond points directly at you (parallel to *z* axis).
b. Draw with Kekulé notation, distorting the perspective as necessary to show all atoms.
c. Rotate about the *y* axis 60 degrees, so that one equatorial bond is parallel to the *x* axis.
d. Draw with Kekulé notation, distorting the perspective as necessary to show all atoms.

Load the Molfile `SF4.mol`. In SF<sub>4</sub>, the lone pair occupies an equatorial position, so the overall shape is "seesaw".

a. Rotate so that the lone pair is parallel to the *x* axis.
b. Draw with Kekulé notation.

## Exercise: Drawing molecules with octahedral geometry (SN=6)

Load the Molfile `SF6.mol`.

a. Rotate so that two bonds lie in the *xy* plane and point directly up and down (parallel to *y* axis); two bonds also lie in the *xz* plane and point directly left and right (parallel to *x* axis); and the remaining bonds are parallel to the *z* axis. 
b. Draw with Kekulé notation, distorting the perspective as necessary to show all atoms.
c. Rotate about the *y* axis 45 degrees, so that two bonds are still parallel to the *y* axis, but the other four lie in the *xz* plane and are diagonal to the *x* and *z* axes.
d. Draw with Kekulé notation, distorting the perspective as necessary to show all atoms.
e. Rotate about the *x* axis 45 degrees, so that the formerly up-and-down bonds are now directed parallel to the *y* and *z* axes. Three F atoms should now lie in a plane that parallel to the *xy* plane but closer to you; the other three F atoms should lie in a similar plane further from you.
f. Draw with Kekulé notation.

Load the Molfile `XeF4.mol`. This molecule is square planar, with lone pairs occupying opposite positions.

g. Rotate so that the lone pairs are parallel to the *y* axis, and bonds lie in the *xz* plane diagonal to the *x* and *z* axes; then rotate about the *x* axis 45 degrees. The resulting arrangement should be similar to view (e) above. 
h. Draw with Kekulé notation.
