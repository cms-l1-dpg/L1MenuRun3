# L1Menu_Collisions2023_v1_0_1

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_0_1/L1Menu_Collisions2023_v1_0_1.html)

**Comment:** 
New version of 2023 L1 menu, created in updated version of TME `0.15.2`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The following changes have been done w.r.t. the previous version of the menu.

#### Updated definition of upt seeds to a more compact logic expression [CMSLITDPG-959](https://its.cern.ch/jira/browse/CMSLITDPG-959)
   - `L1_DoubleMu0_Upt5_Upt5`	(bit 51)
   - `L1_DoubleMu0_Upt6_IP_Min1_Upt4` (bit 52)
   - `L1_DoubleMu0_Upt15_Upt7` (bit 53)

#### Updated algos of muon monitoring to use the newly available index bits from uGMT (`MU-INDEX`) instead of eta of the uGMT candidate [CMSLITDPG-1075](https://its.cern.ch/jira/browse/CMSLITDPG-1075)
   - `L1_SingleMuCosmics_BMTF` (bit 1)   
   - `L1_SingleMuCosmics_OMTF` (bit 2) 
   - `L1_SingleMuCosmics_EMTF` (bit 3)
   - `L1_SingleMu0_BMTF` (bit 9)
   - `L1_SingleMu0_OMTF` (bit 10)
   - `L1_SingleMu0_EMTF` (bit 11)
   - `L1_SingleMu12_DQ_BMTF` (bit 16)
   - `L1_SingleMu12_DQ_OMTF` (bit 17)
   - `L1_SingleMu12_DQ_EMTF` (bit 18)
   - `L1_SingleMu22_BMTF` (bit 25)	
   - `L1_SingleMu22_OMTF` (bit 26)	
   - `L1_SingleMu22_EMTF` (bit 27)	


<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
