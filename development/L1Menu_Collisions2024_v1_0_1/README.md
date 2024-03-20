# L1Menu_Collisions2024_v1_0_1

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2024_v1_0_1/L1Menu_Collisions2024_v1_0_1.html)

**Comment:** 
First L1T menu for the 2024 pp data taking, with the updated UTM grammar (`0.12.0`).
Only changes w.r.t. the previous menu (2024_v1_0_0) are in the AXO seeds definition.

This menu has been created by using the last version of TME `0.16.0`, grammar `0.12.0` and scales`scales_2023_02_16`.

<br/>

The following changes, from the first menu of 2024 (`L1Menu_Collisions2024_v1_0_0`), have been made:

### Seeds for AXOL1TL [CMSLITDPG-1208](https://its.cern.ch/jira/browse/CMSLITDPG-1208)
   - Modified the following 5 new seeds to use the new UTM grammar (NN model version used: [v3](https://globaltrigger.web.cern.ch/upgrade/tme/models)) and [fixed the AXO thresholds](https://its.cern.ch/jira/browse/CMSLITDPG-1208?focusedId=6306964&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel#comment-6306964): 
      - `L1_AXO_VLoose`  (bit 438)
      - `L1_AXO_Loose`   (bit 439)
      - `L1_AXO_Nominal` (bit 440)
      - `L1_AXO_Tight`   (bit 441)
      - `L1_AXO_VTight`  (bit 442)


**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.

