# L1Menu_Collisions2023_v1_3_1 (for initial 2024 commissioning)

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_3_1/L1Menu_Collisions2023_v1_3_1.html)

**Comment:** 
New version of the L1T menu for initial 2024 commissioning, based on the last 2023 menu v1_3_0 (never deployed due to the LHC accident). This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The only difference w.r.t. the last 2023 menu (`L1Menu_Collisions2023_v1_3_0`), is the following: 

### Addition of three single muon monitoring seeds for new quality selection commissioning [CMSLITDPG-1220](https://its.cern.ch/jira/browse/CMSLITDPG-1220):
   - `L1_SingleMu0_SQ13_BMTF` (bit 33) 
   - `L1_SingleMu0_SQ14_BMTF` (bit 34)   
   - `L1_SingleMu0_SQ15_BMTF` (bit 35)

<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.