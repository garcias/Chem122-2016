# Molecular databases

Chemical databases, such as PubChem or the Human Metabolome DataBase, contain a wealth of information on a vast array of molecules. They are special in that they organize this information according to molecular properties, and they document the primary sources of each type of information. One challenge they pose is in recognizing the compound you want to learn about. If your compound has many synonyms, the one you search for might not match how it is entered in the database. Or if your compound is often mixed with others, a general text search will reveal hundreds of records that mention your compound, but it won't be clear which of these contains the information specific to your compound. Finally, the compound you want to research might not have a well-known name yet, and only appears in databases under some sort of ID number.

It is often more reliable to search according to structure of your compound. 

## PubChem database tutorial with ketamine

1. Look up the structure of ketamine and use JSME to determine its SMILES string,
2. Navigate to the PubChem project at [pubchem.ncbi.nlm.nih.gov](https://pubchem.ncbi.nlm.nih.gov)
3. Search for the word "ketamine". You should get over 20 results spanning multiple pages.
4. Replace "ketamine" in the search field with the SMILES string: `CNC1(CCCCC1=O)C1=CC=CC=C1Cl`. This time you should get only one result. Click the result to open its information page.
5. The information page is extensive, so use the table of contents to locate different types of information. For this project the most interesting information will be in the chapters **Medication information**, **Pharmacology**, **Biochemistry**, and **Biomolecular interactions**. Some sections are only shown partially, so for each section below, look for a link to open it fully.
6. Open the section "Therapeutic Uses" under **Medication information**. Briefly describe three therapeutic uses and record the sources of this information. At least one of these should have a "PMID", which is a link to a PubMed bibliographic page on that source.
7. Open the section "Absorption, Distribution and Excretion" in **Pharmacology**. 
    - Determine if ketamine is difficult to absorb.
    - Predict if ingestion (which is subject to first-pass elmination) would be an effective way to administer ketamine.
    - Estimate approximately the half life of ketamine elimination from the bloodstream. Record a citation for the study that produced this estimate, along with relevant details of the study (tested with animals, given with another drug, etc.)
8. Using the appropriate section in **Biochemistry**, identify at least two observed metabolites of ketamine. Record at least one suspected or observed effect you can attribute to one of these metabolites.
9. Search through the sections "Mechanism of action" and "DrugBank interactions" and identify three enzymes or receptors that ketamine reacts with. For each one, record the action of ketamine (agonist, substrate, binder, etc.) and a citation for the related study.
10. Find and record the number of government-approved clinical trials that have been registered for ketamine.


## Exercise: Check for information on potential metabolite.

1. Draw the structure of ketamine with JSME, except remove the methyl group (CH<sub>3</sub>) on the N atom, and replace with a single H atom. Copy its SMILES string,
2. Look up this compound's information using the SMILES string: [pubchem.ncbi.nlm.nih.gov](https://pubchem.ncbi.nlm.nih.gov)
3. On the information page, use the table of contents to locate different types of properties, such as:
    - therapeutic effects (with citations)
    - efficiency of absorption, especially through ingestion
    - half life of elimination (with citations)
    - child metabolites and their possible effects
    - receptors/enzymes targeted by metabolite, and its action on them (with citations)
    - Number of clinical trials?
