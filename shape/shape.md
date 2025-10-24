# Molecular shape and architecture

Most molecules consist of several atoms connected in a particular network **architecture**, with chains, rings, branches, cages, or some combination thereof. While each center has its own local geometry, these may combine to form a complex molecular **shape**. In this tutorial, you will:

- draw the structural formula of linear-chain and branched molecules
- generate the SMILES string representing how a molecule's atoms are connected
- generate the three-dimensional coordinates from the SMILES string
- display each structure with Jmol 
- draw the projection of a 3D molecular structure 

## JSME tuorial

The **JavaScript Molecular Editor** is an interactive tool for editing chemical formulas, and then converting this information into machine-friendly notation for database queries.  It also allows you to sketch out site-specific variations on a given structure, which is useful for studying metabolites of a parent compound.

### Skeletal notation

JSME structures are shown in **skeletal notation**, which is helpful when a structure contains many C and H atoms. It represents C atoms as the endpoints of bonds, and omits the H atoms and C-H bond lines entirely (we say that the C and H atoms are **implicit**). When interpreting skeletal notation, we must infer how many H atoms are bonded to each C atom, and which ways the C–H bonds point, since they’re not shown explicitly.

### Start JSME

JSME is a web app that runs in your browser. Search for an available JSME implementation. (As of Nove 2018, [Peter Ertl's demonstration page](https://jsme-editor.github.io/dist/JSME_test.html) works well.) 

### Generate SMILES notation for ethane

1. In JSME, clear any existing structures using the white rectangle in the top toolbar.
2. Click the single-bond tool (a simple line).
3. Click in the canvas area. It adds a single line, which represents ethane, CH<sub>3</sub>CH<sub>3</sub>, in skeletal notation. 
4. Click the double arrow button and **Copy as SMILES** (or click the smiley face button if available). Copy this string; it should be simply `CC`. 

### Visualize the structure of ethane

1. Start up [Jmol Console](https://garcias.github.io/jmol-console/). 
2. Use `cd` to point to this URL, and `load` to construct a model from the SMILES string. The `$` tells Jmol to that `CC` is SMILES notation and not a file name.

```Java
    cd https://garcias.github.io/Chem122-2016/shape/
    load $CC
    centerat average
```

3. Rotate the molecule and observe its appearance from different perspectives.
4. Rotate the molecule so that the C chain lies in the plane of the screen. Read the guidelines below and then sketch this model.

{: .note }
Jmol may fail to load a model using the `$` notation if the NIH Cactus server is down due to government shutdown. (Jmol relies on the Cactus service to convert the SMILES string to a 3D structure file that it can load.) If this happens, then replace the `$` symbol with the phrase `:smiles:`, which will cause Jmol to request the structure from PubChem instead. For example, `load :smiles:CC` will load the model in PubChem's record for ethane. (This method may also fail if PubChem doesn't contain a 3D structure file for the compound.)

### Including perspective in a chemical structure

Drawing a ball-and-stick model shows the spatial arrangement accurately — but is time-consuming. In practice, chemists replace the circles with atomic symbols, and use wedged and dotted lines to show when bonds are not in the screen plane.

When drawing a C chain, we prefer to keep the C–C bonds in the same plane as much as possible. But then the H atoms pointing out of the screen will obscure the H atoms pointing behind the screen. How can we show all the atoms? Chemists take artistic license, offsetting the front H to one side and the back H to the other side. This is not a perfectly accurate depiction, but does manage to represent all the important aspects of molecular shape.

## Exercise: Generating the structure of alkanes

Using JSME, Jmol models, and these visual conventions, sketch each molecule below in Kekule notation and in skeletal notation. Record both the name and SMILES string for each one next to the structure.

- ethane: CH<sub>3</sub>CH<sub>3</sub>
- propane: CH<sub>3</sub>CH<sub>2</sub>CH<sub>3</sub>
- butane: CH<sub>3</sub>CH<sub>2</sub>CH<sub>2</sub>CH<sub>3</sub>
- 2-methylbutane: (CH<sub>3</sub>)<sub>2</sub>CH<sub></sub>CH<sub>2</sub>CH<sub>3</sub> *(This is based on butane, except you replace a H with a methyl group (CH<sub>3</sub>) branching at the 2nd C atom.)*
- isopentanol: (CH<sub>3</sub>)<sub>2</sub>CH<sub></sub>CH<sub>2</sub>CH<sub>2</sub>OH *(This is based on 2-methylbutane, except you replace a H with a hydroxyl group (–OH) at the end of the chain.)*
- cyclohexane: C<sub>6</sub>H<sub>12</sub>, six CH<sub>2</sub> groups connected in a ring
- cyclohexanol: C<sub>6</sub>H<sub>11</sub>OH, *(This is based on cyclohexane, except you replace a H with a hydroxyl group (–OH).)* 


## Exercise: Visualizing isomerism between molecules

1. Look up and record the structural formulas of the following compounds. (The Wikipedia article for some will show two structures; record both).
    - n-propanol
    - isopropanol
    - 2-butene (double bond is in the middle) 
    - glycine, without charges 
    - alanine, without charges 
    - carvone (label "R" and "S" forms)
2. Using JSME, Jmol models, and these visual conventions, sketch the Kekule or skeletal structure of n-propanol using wedge notation. Repeat this for isopropanol. Compare your models and describe the difference in overall shape.
3. For each pair of molecules below, assign one to yourself and the other to a partner, so you can compare the results visually. Generate the model of each and sketch the structure on paper using wedge notation. Compare your models and describe the difference in overall shape.
    1. **cis-2-butene vs trans-2-butene.** 
    2. **alanine.** Draw alanine in a way that the N atom is in the same plane as the two C atoms and the two O atoms. Use the wedged-bond tool for the methyl (CH<sub>3</sub>) group. One partner should indicate that the methyl group is in front of the plane of the page; the other partner should put it behind the plane of the page. Use the SMILES string to generate a model. Show all C and H atoms, evne those that were implicit in JSME. Try to rotate your 3D model so it matches your partner's model.
    3. **glycine.** Draw glycine in a similar way to alanine and generate each model. Draw the corresponding Kekulé structure on paper. Try to rotate your model so it matches your partner's model.
    4. **R- vs S-carvone.** Draw with JSME, using the ring tool as a shortcut for making the 6-C ring and then modifying it. Pay careful attention to the wedge notation. Some but not all C atoms in the ring are in the same plane. Try to rotate your model so it matches your partner's model.

When using the JSME wedge tool, click on a wedge bond (pointing toward you) to convert it to a dashed wedge (pointing away from you).

