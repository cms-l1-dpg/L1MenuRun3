# L1Menu_Collisions2023_v1_1_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_1_0/L1Menu_Collisions2023_v1_1_0.html)

**Comment:** 
First version of the L1 menu for the 2023 physics data taking (starting from 1200b), targeting the second HLT menu of 2023.
This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The following changes, from the last menu of 2023 (`L1Menu_Collisions2023_v1_0_1`), have been done:

### Seed for HMT triggers [CMSLITDPG-1087](https://its.cern.ch/jira/browse/CMSLITDPG-1087)
   - Added a new seed:
      - `L1_TwoMuShower_Loose` (bit 106)

### Seed for VBF inclusive [CMSLITDPG-1110](https://its.cern.ch/jira/browse/CMSLITDPG-1110)
   - Added a new seed:
      - `L1_DoubleJet_90_30_Mass_Min550` (bit 354)

### Seeds for VBF exclusive [CMSLITDPG-1099](https://its.cern.ch/jira/browse/CMSLITDPG-1099)
   - Added four new seeds:
      - `L1_DoubleJet_60_30_DoubleJet30_Mass_Min500_DoubleJetCentral50` (bit 368)
      - `L1_DoubleJet40_Mass_Min450_IsoEG10er2p1_RmOvlp_dR0p2` (bit 369)
      - `L1_DoubleJet_80_30_DoubleJet30_Mass_Min500_Mu3OQ` (bit 370)
      - `L1_DoubleJet_65_30_DoubleJet30_Mass_Min400_ETMHF65` (bit 371)

### Monitoring seeds for the upt muons [CMSLITDPG-1123](https://its.cern.ch/jira/browse/CMSLITDPG-1123)
   - Added four new seeds:
      - `L1_SingleMu0_Upt10` (bit 12)
      - `L1_SingleMu0_Upt10_BMTF` (bit 13)
      - `L1_SingleMu0_Upt10_OMTF` (bit 14)
      - `L1_SingleMu0_Upt10_EMTF` (bit 15)

<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
