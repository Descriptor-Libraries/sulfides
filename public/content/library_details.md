# Library Details

## 

## Molecule Identification

The search for sulfide compounds was performed using Reaxys database on June 6th, 2024.<br>
The structure search was conducted for sulfides: C−S−C <br>



Then the following filters were applied: <br>

• Number of sulfur atoms ≤ 3 <br>

• Molecular weight ≤ 500 <br>

• Commercial availability <br>

• Has NMR spectra: <sup>1</sup>H and <sup>13</sup>C <br>

• Functional group filters: <br>

|If the functional group contains:|Exclude:|
|-|-|
|1 S atom|thiocyanates, thiols, thiocarbonates, isothiocyanates|
|2 S atoms|all|
|1 O atom|containing N−O, N=O, S−O, S=O|
|2 O atoms|peroxides|
|3 O atoms|carboxylic orthoesters, nitrates|
|4 O atoms|all|
|1 N atom|cyanates, isocyanates, oximes, amines (primary, secondary, quaternary, hydroxylamines, thiohemiaminals), amides (sulfinamides, sulfenamides, primary carboxamides), hydroxamic acids|
|2 N atoms|hydrazines, hydrazones, ureas, carboxylic hydrazines|
|3 N atoms|all|
|halogen atom|all except alkyl and aryl|
|P atom|phosphines|
|metal atom|all|



This filtered search generated a dataset of >50,000 compounds. The size of the library was further reduced to 2809 by: (1) removing all sulfide that did not have CAS number listed in the Reaxys export and removing all sulfides with fewer than 4 references listed in the Reaxys export, and (2) keeping asymmetrical sulfides with only one sulfur atom susceptible to oxidation.



## Conformational Search \& DFT Computations

Each sulfide was subjected to a conformational search in CREST (version 2.12) with the GFN2-xTB method and the energetic window of 6 kcal/mol. The resulting lowest energy conformer was submitted to a geometry optimization at the B3LYP-D3(BJ)/6-31G(d,p) level of theory followed by single point energy calculations at M06-2X/def2-TZVP using Gaussian 16. A set of 27 steric and electronic molecular descriptors was then calculated using published code: https://github.com/SigmanGroup/Get\_Properties.



## Citations

Jurić, Z.; Slocumb, H. S.; Sigman, M. S. Sulfide Descriptor Library. **2026** (https://descriptor-libraries.molssi.org/sulfides) <br>

Gaster, E.; Slocumb, H. S.; Jurić, Z.; Myers, T. E.; Lim, N.-K.; Malig, T. C.; Toste, F. D.; Gosselin, F.; Sigman, M. S.; Miller, S. J. *J. Am. Chem. Soc.* **2026**, *148*, 18791–18803. DOI: 10.1021/jacs.5c23100.



