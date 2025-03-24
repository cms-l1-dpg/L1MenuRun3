# L1Menu_Collisions2025_v0_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2025_v0_0_0/L1Menu_Collisions2025_v0_0_0.html)

**Comment:** 
Intermediate version of the L1T menu, towards the first official L1T menu version for the 2025 pp data taking.
This menu has been created by using the last version of TME `0.17.2`, grammar `0.13.0` and `scales_2024_05_15`.

<br/>

The following changes, from the last pp menu of 2024 (`L1Menu_Collisions2024_v1_3_0`), have been made:

### Added low pT Single Muon seed for BPH [CMSL1TDPG-1341](https://its.cern.ch/jira/browse/CMSLITDPG-1341)
   - Added the following seed: 
      - `L1_SingleMu5_BMTF` (bit 207)

### Added high quality Single Muon seed for EXO [CMSL1TDPG-1350](https://its.cern.ch/jira/browse/CMSLITDPG-1350)
   - Added the following seed: 
      - `L1_SingleMu13_SQ14_BMTF` (bit 208)

### Added DoubleTau+Jet seeds for HIG [CMSL1TDPG-1337](https://its.cern.ch/jira/browse/CMSLITDPG-1337)
   - Added the following seeds: 
      - `L1_DoubleTau_Iso34_Iso26_er2p1_Jet55_RmOvlp_dR0p5` (bit 273)
      - `L1_DoubleTau_Iso38_Iso26_er2p1_Jet55_RmOvlp_dR0p5` (bit 274)
      - `L1_DoubleTau_Iso40_Iso26_er2p1_Jet55_RmOvlp_dR0p5` (bit 275)

### Added low pT DoubleEG seeds for EXO [CMSL1TDPG-1347](https://its.cern.ch/jira/browse/CMSLITDPG-1347)
   - Added the following seed: 
      - `L1_DoubleEG15_11_er1p2_dR_Max0p6` (bit 212)
      - `L1_DoubleEG15_er1p5_dEta_Max1p5` (bit 213)      
   - Possible (usefulness of) backup seeds currently under discussion.

### Added 18 seeds with tighter mjj thresholds for VBF parking seeds [CMSL1TDPG-1348](https://its.cern.ch/jira/browse/CMSLITDPG-1348)
   - Added the following seeds: 
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min1000` (bit 354)
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min1100` (bit 355)
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min1200` (bit 356)
      - `L1_DoubleJet45_Mass_Min700_IsoTau45er2p1_RmOvlp_dR0p5` (bit 359)
      - `L1_DoubleJet45_Mass_Min800_IsoTau45er2p1_RmOvlp_dR0p5` (bit 360)
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min750_DoubleJetCentral50` (bit 372)
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min850_DoubleJetCentral50` (bit 373)
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min950_DoubleJetCentral50` (bit 374)
      - `L1_DoubleJet45_Mass_Min700_LooseIsoEG20er2p1_RmOvlp_dR0p2` (bit 375)
      - `L1_DoubleJet45_Mass_Min800_LooseIsoEG20er2p1_RmOvlp_dR0p2` (bit 376)
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min700_Mu3OQ` (bit 377)
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min800_Mu3OQ` (bit 378)
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min900_Mu3OQ` (bit 379)
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min600_ETMHF65` (bit 380)
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min700_ETMHF65` (bit 381)
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min800_ETMHF65` (bit 382)

### Added new seeds (placeholders) for AXO [CMSL1TDPG-1344](https://its.cern.ch/jira/browse/CMSLITDPG-1344) - AD model and seeds thresholds to be changed for final version of 1st menu!
   - Added the following seeds: 
     - `L1_AXO_Medium` (bit 444) 
     - `L1_AXO_VVTight` (bit 507) 
     - `L1_AXO_VVVTight` (bit 508) 

### Added tighter versions (placeholders) of the CICADA seeds [CMSL1TDPG-1343](https://its.cern.ch/jira/browse/CMSLITDPG-1343) - AD model and seeds thresholds to be changed for final version of 1st menu!
   - Added the following seeds: 
     - `L1_CICADA_VVTight` (bit 509) 
     - `L1_CICADA_VVVTight` (bit 510) 
     - `L1_CICADA_VVVVTight` (bit 511) 
