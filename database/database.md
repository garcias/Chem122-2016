# Molecular databases

Chemical databases, such as PubChem or the Human Metabolome DataBase, contain a wealth of information on a vast array of molecules. They are special in that they summarize and organize this information according to molecular properties, and they document the primary sources of each type of information so you can research further. One challenge they pose is in recognizing the compound you want to learn about. If your compound has many synonyms, the one you search for might not match how it is entered in the database. Or if your compound is often mixed with others, a general text search will reveal hundreds of records that mention your compound, but it won't be clear which of these contains the information specific to your compound. Finally, the compound you want to research might not have a well-known name yet, and only appears in databases under some sort of ID number.

It is often more reliable to search according to structure of your compound. 

## PubChem database tutorial with ketamine

1. Look up the structure of ketamine and use JSME to determine its SMILES string,
2. Navigate to the PubChem project at [pubchem.ncbi.nlm.nih.gov](https://pubchem.ncbi.nlm.nih.gov)
3. Search for the word "ketamine". You should get over 20 results spanning multiple pages.
4. Replace "ketamine" in the search field with the SMILES string: `CNC1(CCCCC1=O)C1=CC=CC=C1Cl`. This time you should get only one result. Click the result to open its information page.
5. The information page is extensive, so use the table of contents to locate different types of information. For this project the most interesting information will be in the chapters **Drug and Medication information**, **Pharmacology**, **Biochemistry**, and **Biomolecular interactions**. The page shows some sections partially, so for each section below, click the link-out button to open it fully in a new tab.
6. In the chapter **Drug and Medication information**, find and open the section "Therapeutic Uses". Each entry provides an excerpt or abstract, followed by information about the source and a link. Read through the entries and find three therapeutic uses (for humans); record a brief description of each use and record the name and url of the source. At least one of these should have a link that starts with "PMID" followed by a number; this is a link to a PubMed bibliographic page on that source.
7. In the chapter **Pharmacology and Biochemistry**, open the section "Absorption, Distribution and Excretion".
    - Decide whether ingestion (which is subject to first-pass metabolism) would be an effective way to dose ketamine.
    - Estimate approximately the half life of ketamine distribution into tissues. Record a citation for the study.
    - Estimate approximately the half life of ketamine elimination from tissues. Record a citation for the study that produced this estimate, along with relevant details of the study (tested with animals, given with another drug, etc.)
8. Using other sections in this chapter, identify at least two observed metabolites of ketamine. Record a possible or suspected effect for one of them.
9. Read the entries in "Mechanism of action" and identify three enzymes or receptors that ketamine reacts with. For each one, record the role of ketamine (agonist, substrate, binder, etc.), an excerpt that leads you to this conclusion, and a citation for the related study.
10. Find and record the number of government-approved clinical trials that have been registered for ketamine.

## Canadian DrugBank tutorial with ketamine

1. On the PubChem page for ketamine, find any information attributed to "DrugBank", and click the URL in the citation. Alternatively, go directly to https://go.drugbank.com and enter the CAS number for ketamine in the "Drugs" search bar.
3. Skip to the section **Pharmacology/Metabolism** and review the list of metabolites shown; confirm they are consistent with the information listed on the PubChem page.
2. Skip to the section **Pharmacology/Mechanism of action** and review the list of proteins shown. Confirm that the role is consistent with the information listed on the PubChem page. 
4. Click on the link for "Delta-type opioid receptor" to jump to its **Targets** section. 

## Exercise: Check for information on potential metabolite.

1. Draw the structure of ketamine with JSME, except remove the methyl group (CH<sub>3</sub>) on the N atom, and replace with a single H atom. Copy its SMILES string,
2. Look up this compound's information using the SMILES string: [pubchem.ncbi.nlm.nih.gov](https://pubchem.ncbi.nlm.nih.gov)
3. On the information page, use the table of contents to locate different types of properties, such as:
    - common name(s) of this compound
    - therapeutic effects (with citations)
    - efficiency of absorption, especially through ingestion
    - half life of elimination (with citations)
    - child metabolites and their possible effects
    - receptors/enzymes targeted by metabolite, and its action on them (with citations)
    - Number of clinical trials?
