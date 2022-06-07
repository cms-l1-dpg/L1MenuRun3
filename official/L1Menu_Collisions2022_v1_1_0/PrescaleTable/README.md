# Prescale and mask tables for the L1Menu_Collisions2022_v1_1_0

**Description of the different formats** 
* The PS table in **csv format** is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
* The PS table in **xlsx format** is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).

- PS Tables for specific data taking modes:
    - Collisions   = L1TPrescaleTable_Collisions_900GeV_Menu2022_v1_1_0
    - Circulations = L1TPrescaleTable_Circulating_Menu2022_v1_1_0
    - Cosmics 	   = L1TPrescaleTable_Cosmics_CRAFT_Menu2022_v1_1_0 

**NOTE:** The default PrescaleSet is set to 3. This column corresponds to the set of prescales for an instantaneous luminosity 2E+34. See below the correspondence between the column identifier and the corresponding instantaneous luminosity scenario under consideration:
* 0: Emergency (all PS=0)
* 1: Unprescaled (all PS=1)
* 2: 2.2E+34
* 3: 2E+34
* 4: 1.7E+34
* 5: 1.5E+34
* 6: 1.3E+34
* 7: 1.1E+34
* 8: 9E+33
* 9: 6E+33
