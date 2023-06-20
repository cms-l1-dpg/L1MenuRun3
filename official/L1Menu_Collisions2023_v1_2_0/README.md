# L1Menu_Collisions2023_v1_2_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_2_0/L1Menu_Collisions2023_v1_2_0.html)

**Comment:** 
New version of the L1 menu for the 2023 physics data taking, targeting the third HLT menu of 2023.
This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The following changes, from the last menu of 2023 (`L1Menu_Collisions2023_v1_1_0`), have been made:

### New (backup) seeds VBF exclusive [CMSLITDPG-1146](https://its.cern.ch/jira/browse/CMSLITDPG-1146)
   - Added new seeds:
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min500_DoubleJetCentral50` (bit 369)
      - `L1_DoubleJet40_Mass_Min450_LooseIsoEG15er2p1_RmOvlp_dR0p2` (bit 371)
      - `L1_DoubleJet45_Mass_Min450_LooseIsoEG20er2p1_RmOvlp_dR0p2` (bit 372)
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min500_Mu3OQ` (bit 374)
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min400_ETMHF65` (bit 376)


### New seeds for VBF inclusive [CMSLITDPG-1146](https://its.cern.ch/jira/browse/CMSLITDPG-1146?focusedCommentId=4846462&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel#comment-4846462)
   - Added new seeds:
      - `L1_DoubleJet_90_30_DoubleJet30_Mass_Min800` (bit 353)
      - `L1_DoubleJet_100_30_DoubleJet30_Mass_Min800` (bit 355)
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min800` (bit 357)

### Removal of unused seeds [CMSLITDPG-1155](https://its.cern.ch/jira/browse/CMSLITDPG-1155)
   - Removed the following 26 seeds
      - `L1_SingleMu6er1p5`
      - `L1_SingleMu7er1p5`
      - `L1_SingleMu8er1p5`
      - `L1_SingleMu9er1p5`
      - `L1_SingleMu10er1p5`
      - `L1_SingleMu12er1p5`
      - `L1_SingleMu14er1p5`
      - `L1_SingleMu16er1p5`
      - `L1_SingleMu18er1p5`
      - `L1_DoubleMu0er2p0_SQ_dR_Max1p4`
      - `L1_DoubleMu0er2p0_SQ_OS_dR_Max1p4`
      - `L1_TripleMu_5_3p5_2p5_OQ_DoubleMu_5_2p5_OQ_OS_Mass_5to17`
      - `L1_SingleIsoEG24er1p5`
      - `L1_SingleIsoEG26er1p5`
      - `L1_DoubleEG_LooseIso20_10_er2p5`
      - `L1_DoubleEG_LooseIso22_10_er2p5`
      - `L1_TripleEG_16_12_8_er2p5`
      - `L1_TripleEG_16_15_8_er2p5`
      - `L1_DoubleIsoTau32er2p1_Mass_Max90`
      - `L1_SingleJet140er2p5_ETMHF70`
      - `L1_SingleJet140er2p5_ETMHF80`
      - `L1_DoubleJet30er2p5_Mass_Min200_dEta_Max1p5`
      - `L1_ETT1200`
      - `L1_ETMHF120_NotSecondBunchInTrain`
      - `L1_ETMHF110_HTT60er_NotSecondBunchInTrain`
      - `L1_DoubleJet_90_30_Mass_Min550`
