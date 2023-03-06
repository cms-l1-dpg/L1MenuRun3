# L1Menu_Collisions2023_v1_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_0_0/L1Menu_Collisions2023_v1_0_0.html)

**Comment:** 
First version of the L1 menu for the 2023 data taking. It will be used as a starting point for the developments and updates of the L1 menu targeting the first round of integration (March 8th).

<br/>

The following changes, from the last menu of 2022 ("L1Menu_Collisions2022_v1_4_0"), have been done:

### Seeds for the Tau3mu search ([CMSLITDPG-960](https://its.cern.ch/jira/browse/CMSLITDPG-960))
   - Removed the seeds included in 2022: 
      - `L1_TripleMu_2SQ_1p5SQ_0OQ` 
      - `L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12` 
      - `L1_TripleMu_3SQ_2p5SQ_0OQ_Mass_Max12` 
   - Added four new seeds for 2023:
      - `L1_TripleMu_3SQ_2p5SQ_0_OS_Mass_Max12` (bit 91) 
      - `L1_TripleMu_4SQ_2p5SQ_0_OS_Mass_Max12` (bit 92) &rarr; backup seed
      - `L1_TripleMu_3SQ_2p5SQ_0` (bit 84) &rarr; control seed, PS = 100
      - `L1_TripleMu_3SQ_2p5SQ_0_Mass_Max12` (bit 85) &rarr; control seed, PS = 100
      
      
### Seeds for Bsmumu ([CMSLITDPG-1098](https://its.cern.ch/jira/browse/CMSLITDPG-1098))      
   - Added five new seeds for 2023:
      - `L1_DoubleMu0er1p4_SQ_OS_dEta_Max1p2` (bit 66)
      - `L1_DoubleMu4er2p0_SQ_OS_dR_Max1p6` (bit 72)
      - `L1_DoubleMu5_SQ_OS_dR_Max1p6` (bit 78)
      - `L1_DoubleMu3er2p0_SQ_OS_dR_Max1p6` (bit 68)
      - `L1_DoubleMu0er1p5_SQ_OS_dEta_Max1p2` (bit 64)  
   - Removed the unused seed included in 2022: 
      - `L1_DoubleMu3er2p0_SQ_OS_dR_Max1p4` &rarr; [CMSLITDPG-951](https://its.cern.ch/jira/browse/CMSLITDPG-951)) 


### Eta change for L1 FWD triggers ([CMSLITDPG-1086](https://its.cern.ch/jira/browse/CMSLITDPG-1086))
   - Removed the following seeds:
      - `L1_SingleJet60er2p5` 
      - `L1_SingleJet90er2p5` 
      - `L1_SingleJet60_FWD3p0` 
      - `L1_SingleJet90_FWD3p0` 
   - Added four new seeds:
      - `L1_SingleJet35_FWD2p5` (bit 320)
      - `L1_SingleJet60_FWD2p5` (bit 321)
      - `L1_SingleJet90_FWD2p5` (bit 322)
      - `L1_SingleJet120_FWD2p5` (bit 323)


### New seeds with central pair of jets with reduced mjj threshold ([CMSLITDPG-1095](https://its.cern.ch/jira/browse/CMSLITDPG-1095))
   - Added the following seed for testing:
      - `L1_DoubleJet30er2p5_Mass_Min225_dEta_Max1p5` (bit 350) 
   - Removed the following seed: 
      - `L1_DoubleJet30er2p5_Mass_Min150_dEta_Max1p5`


### Double Jet + One Tau new Run 3 seed ([CMSLITDPG-962](https://its.cern.ch/jira/browse/CMSLITDPG-962))
   - Added a backup seed:
      - `L1_DoubleJet45_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5` (bit 363)


### New seeds for W &rarr; 3pi search ([CMSLITDPG-1093](https://its.cern.ch/jira/browse/CMSLITDPG-1093))
   - Added two new seeds:
      - `L1_DoubleIsoTau32er2p1_Mass_Max90` (bit 277)
      - `L1_DoubleIsoTau32er2p1_Mass_Max80` (bit 278)


### Seeds for BTag POG ([CMSLITDPG-1100](https://its.cern.ch/jira/browse/CMSLITDPG-1100))
   - Added two new seeds:
      - `L1_DoubleJet16er2p5_Mu3_dR_Max0p4` (bit 123)
      - `L1_DoubleJet60er2p5_Mu3_dR_Max0p4` (bit 126)
   - Seeds modified (because they are only used in Btag POG HLT paths)
      - `L1_Mu3_Jet35er2p5_dR_Max0p4` &rarr; `L1_DoubleJet35er2p5_Mu3_dR_Max0p4` (bit 124)
      - `L1_Mu3_Jet80er2p5_dR_Max0p4` &rarr; `L1_DoubleJet80er2p5_Mu3_dR_Max0p4` (bit 127)
      - `L1_Mu3_Jet120er2p5_dR_Max0p8` &rarr; `L1_DoubleJet120er2p5_Mu3_dR_Max0p8` (bit 128)
   - Removed the following seed:
      - `L1_Mu3_Jet120er2p5_dR_Max0p4`


### Seeds for muon monitoring split by TF ([CMSLITDPG-1101](https://its.cern.ch/jira/browse/CMSLITDPG-1101)) 
   - Seeds added:
      - `L1_SingleMuOpen_BMTF` (bit 5)
      - `L1_SingleMuOpen_OMTF` (bit 6)
      - `L1_SingleMuOpen_EMTF` (bit 7)


<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
