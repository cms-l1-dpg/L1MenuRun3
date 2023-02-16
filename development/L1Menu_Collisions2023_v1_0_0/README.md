# L1Menu_Collisions2023_v1_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_0_0/L1Menu_Collisions2023_v1_0_0.html)

**Comment:** 
First version of the L1 menu for the 2023 data taking. It will be used as a starting point for the developments and updates of the L1 menu targeting the first round of integration (March 8th).

## Changes from last 2022 menu ("L1Menu_Collisions2022_v1_4_0")

### Seeds for Tau3mu search ([CMSLITDPG-960](https://its.cern.ch/jira/browse/CMSLITDPG-960))
   - Removed the seeds included in 2022: 
      - `L1_TripleMu_2SQ_1p5SQ_0OQ` (bit 74) 
      - `L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12` (bit 82)
      - `L1_TripleMu_3SQ_2p5SQ_0OQ_Mass_Max12` (bit 83)
   - Added two new seeds for 2023:
      - `L1_TripleMu_3SQ_2p5SQ_0_OS_Mass_Max12` (bit 82) 
      - `L1_TripleMu_4SQ_2p5SQ_0OQ_OS_Mass_Max12` (bit 83) 
      
### Seeds for Bsmumu ([CMSLITDPG-951](https://its.cern.ch/jira/browse/CMSLITDPG-951))      
   - Removed the unused seed `L1_DoubleMu3er2p0_SQ_OS_dR_Max1p4` (bit 63) 

### Double Jet + One Tau new Run 3 seed ([CMSLITDPG-962](https://its.cern.ch/jira/browse/CMSLITDPG-962)) 
   - Added a backup seed: `L1_DoubleJet45_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5` (bit 363) 

### New seeds for W3pi search ([CMSLITDPG-1093](https://its.cern.ch/jira/browse/CMSLITDPG-1093))
   - Added two new seeds:
      - `L1_DoubleIsoTau32er2p1_Mass_Max90` (bit 277) 
      - `L1_DoubleIsoTau32er2p1_Mass_Max80` (bit 278) 
      
### New seeds for central pair of jets with reduced mjj threshold ([CMSLITDPG-1095](https://its.cern.ch/jira/browse/CMSLITDPG-1095))
   - Added the seed `L1_DoubleJet30er2p5_Mass_Min225_dEta_Max1p5` (bit 350) for testing purposes

### Eta change for L1 FWD triggers ([CMSLITDPG-1086](https://its.cern.ch/jira/browse/CMSLITDPG-1086)) 
   - Added four new seeds:
      - `L1_SingleJet35_FWD2p5` (bit 320)
      - `L1_SingleJet60_FWD2p5` (bit 321)
      - `L1_SingleJet90_FWD2p5` (bit 322)
      - `L1_SingleJet120_FWD2p5` (bit 323)

<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
