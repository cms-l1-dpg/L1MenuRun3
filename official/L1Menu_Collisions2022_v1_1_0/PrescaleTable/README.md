# Prescale and mask tables for the L1Menu_Collisions2022_v1_1_0

**Description of the different formats** 
* The PS table in **csv format** is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
* The PS table in **xlsx format** is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).

- PS Tables for specific data taking modes:
    - Collisions   = L1TPrescaleTable_Collisions_900GeV_Menu2022_v1_1_0
    - Circulating  = L1TPrescaleTable_Circulating_Menu2022_v1_1_0
    - Cosmics 	   = L1TPrescaleTable_Cosmics_CRAFT_Menu2022_v1_1_0 

