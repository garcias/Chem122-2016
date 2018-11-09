# Molecular databases

Chemical databases, such as PubChem or the Human Metabolome DataBase, contain a wealth of information on a vast array of molecules. They are special in that they organize this information according to molecular properties, and they document the primary sources of each type of information. One challenge they pose is in recognizing the compound you want to learn about. If your compound has many synonyms, the one you search for might not match how it is entered in the database. Or if your compound is often mixed with others, a general text search will reveal hundreds of records that mention your compound, but it's wont' be clear which record has all the information specific to your compound. Finally, the compound you want to research might not have a well-known name yet, and only appears in databases under an ID number.

It is often more reliable to search according to structure of your compound. 

## PubChem databse tutorial with ketamine

1. Look up the structure of ketamine and use JSME to determine its SMILES string,
2. Navigate to the PubChem project at [pubchem.ncbi.nlm.nih.gov](https://pubchem.ncbi.nlm.nih.gov)
3. Click through to "PubChem Search Beta" and initiate a search for "Ketamine". You should get over 20 results spanning multiple pages.
4. Replace "ketamine" in the search field with the SMILES string: `CNC1(CCCCC1=O)C1=CC=CC=C1Cl`. This time you should get only one result. 
5. On its information page, use the table of contents to locate different types of properties, such as its therapeutic uses, known risks, and pharmacology. In particular find answers to these questions:
    - Does ketamine have any therapeutic effects? If so, what are they?
    - Have dependency and tolerance been observed for ketamine?
    - What is its clearance and half life?
    - How many clinical trials have been initiated with ketamine?
    - What receptors does it act on?
6. Under "Related Records", find the link for "Similar Compounds". There should be over 200 entries. 


## Exercise: Check for information on potential metabolite.

1. Draw the structure of ketamine with JSME, except remove the methyl group (CH<sub>3</sub>) on the N atom, and replace with a single H atom. Copy its SMILES string,
2. Look up this compound's information using the SMILES string: [pubchem.ncbi.nlm.nih.gov](https://pubchem.ncbi.nlm.nih.gov)
3. On the information page, use the table of contents to locate different types of properties, such as its therapeutic uses, known risks, and pharmacology. In particular find answers to these questions:
    - Would this metabolite have any therapeutic effects? If so, what are they?
    - Have dependency and tolerance been observed for it?
    - What is its clearance and half life?
    - How many clinical trials have been initiated with ut?
    - What receptors does it act on?
