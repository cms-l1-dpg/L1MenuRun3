# L1Menu_Collisions2025_v1_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2025_v1_0_0/L1Menu_Collisions2025_v1_0_0.html)

**Comment:** 
Official version of the 1st L1T menu for the 2025 pp data taking.
This menu has been created by using the last version of TME `0.17.2`, grammar `0.13.0` and `scales_2024_05_15`.

<br/>

The following changes, from the latest 2024 pp menu (2024_v1_0_3) have been made:

### Added low pT Single Muon seed for BPH [CMSL1TDPG-1341](https://its.cern.ch/jira/browse/CMSLITDPG-1341)
   - Added the following seed: 
      - `L1_SingleMu5_BMTF`

### Added high quality Single Muon seed for EXO [CMSL1TDPG-1350](https://its.cern.ch/jira/browse/CMSLITDPG-1350)
   - Added the following seed: 
      - `L1_SingleMu13_SQ14_BMTF`

### Added DoubleTau+Jet seeds for HIG [CMSL1TDPG-1337](https://its.cern.ch/jira/browse/CMSLITDPG-1337)
   - Added the following seeds: 
      - `L1_DoubleTau_Iso34_Iso26_er2p1_Jet55_RmOvlp_dR0p5` 
      - `L1_DoubleTau_Iso38_Iso26_er2p1_Jet55_RmOvlp_dR0p5` 
      - `L1_DoubleTau_Iso40_Iso26_er2p1_Jet55_RmOvlp_dR0p5` 

### Added low pT DoubleEG seeds for EXO [CMSL1TDPG-1347](https://its.cern.ch/jira/browse/CMSLITDPG-1347)
   - Added the following seeds: 
      - `L1_DoubleEG15_11_er1p2_dR_Max0p6` 
      - `L1_DoubleEG16_11_er1p2_dR_Max0p6` (backup)
      - `L1_DoubleEG17_11_er1p2_dR_Max0p6` (backup)
      - `L1_DoubleEG15_er1p5_dEta_Max1p5` 
      - `L1_DoubleEG16_er1p5_dEta_Max1p5` (backup)
      - `L1_DoubleEG17_er1p5_dEta_Max1p5` (backup)

### Added 16 seeds with tighter mjj thresholds for VBF parking seeds [CMSL1TDPG-1348](https://its.cern.ch/jira/browse/CMSLITDPG-1348)
   - Added the following seeds: 
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min1000`
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min1100`
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min1200`
      - `L1_DoubleJet45_Mass_Min700_IsoTau45er2p1_RmOvlp_dR0p5`
      - `L1_DoubleJet45_Mass_Min800_IsoTau45er2p1_RmOvlp_dR0p5` 
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min750_DoubleJetCentral50`
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min850_DoubleJetCentral50`
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min950_DoubleJetCentral50`
      - `L1_DoubleJet45_Mass_Min700_LooseIsoEG20er2p1_RmOvlp_dR0p2` 
      - `L1_DoubleJet45_Mass_Min800_LooseIsoEG20er2p1_RmOvlp_dR0p2`
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min700_Mu3OQ` 
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min800_Mu3OQ` 
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min900_Mu3OQ`
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min600_ETMHF65`
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min700_ETMHF65`
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min800_ETMHF65` 

### Modified NN model and thresholds for AXO seeds [CMSL1TDPG-1344](https://its.cern.ch/jira/browse/CMSLITDPG-1344)
- Modified the following seeds (bits 421-427): 
     - `L1_AXO_VLoose` 
     - `L1_AXO_Loose` 
     - `L1_AXO_Medium`
     - `L1_AXO_Tight` 
     - `L1_AXO_VTight` 
     - `L1_AXO_VVTight` (new seed in 2025)
     - `L1_AXO_VVVTight` (new seed in 2025)

### Modified NN model and thresholds for CICADA seeds [CMSL1TDPG-1343](https://its.cern.ch/jira/browse/CMSLITDPG-1343)
- Modified the following seeds (bits 428-435): 
     - `L1_CICADA_VLoose` 
     - `L1_CICADA_Loose` 
     - `L1_CICADA_Medium`
     - `L1_CICADA_Tight`
     - `L1_CICADA_VTight`
     - `L1_CICADA_VVTight` (new seed in 2025)
     - `L1_CICADA_VVVTight` (new seed in 2025)
     - `L1_CICADA_VVVVTight` (new seed in 2025)

### Added low pT EG and Jet seeds for rate monitoring in view of the HI data taking [CMSL1TDPG-1352](https://its.cern.ch/jira/browse/CMSLITDPG-1352)
- Added the following 27 seeds (bits 444-470): 
     - `L1_SingleJet8/12/16/20/24_BptxAND`
     - `L1_SingleJet8/12/16/20/24er1p3_BptxAND`
     - `L1_SingleJet8`
     - `L1_SingleJet8er1p3`
     - `L1_SingleJet8er2p13`
     - `L1_SingleEG5/7_BptxAND`
     - `L1_SingleEG5/7`
     - `L1_SingleEG5/7er1p52`
     - `L1_DoubleEG2/3/4_BptxAND`
     - `L1_DoubleEG2/3/4er2p13_BptxAND`
     - `L1_DoubleEG2`
     - `L1_DoubleEG2er2p13`

### Added calo monitoring seeds [CMSL1TDPG-1345](https://its.cern.ch/jira/browse/CMSLITDPG-1345)
- Added the following 13 seeds: 
     - SingleJet seeds (bits 297-300)
         - `L1_SingleJet60er1p3`
         - `L1_SingleJet60er1p3to2p5`
         - `L1_SingleJet60er2p5to3p0`
         - `L1_SingleJet60er3p0to5p0`
     - SingleLooseIsoEG seeds (bits 194-196)
         - `L1_SingleLooseIsoEG28er1p3`
         - `L1_SingleLooseIsoEG28er1p3to2p5`
         - `L1_SingleLooseIsoEG28er2p5to3p0`
     - SingleIsoEG seeds (bits 206-208)
         - `L1_SingleIsoEG28er1p3`
         - `L1_SingleIsoEG28er1p3to2p5`
         - `L1_SingleIsoEG28er2p5to3p0`
     - SingleEG seeds (bits 177-179)
         - `L1_SingleEG28er1p3`
         - `L1_SingleEG28er1p3to2p5`
         - `L1_SingleEG28er2p5to3p0`

### Removed some unused seeds [CMSL1TDPG-1357](https://its.cern.ch/jira/browse/CMSLITDPG-1357) 
- Removed the following seeds: 
     - `L1_TripleEG_18_17_8_er2p5`, `L1_TripleEG_18_18_12_er2p5`
     - `L1_LooseIsoEG24/26/28er2p1_HTT100er`
     - `L1_LooseIsoEG26/28/30er2p1_Jet34er2p5_dR_Min0p3`
     - `L1_SingleMu0_Upt10_SQ14_BMTF`, `L1_SingleMu0_Upt25_SQ14_BMTF`
     - `L1_DoubleMu6/7/8_Upt6/7/8_SQ_er2p0`
     - `L1_DoubleIsoTau26er2p1_Jet55/70_RmOvlp_dR0p5`
     - `L1_AXO_Nominal`

--- 
<br/>

**Additional Remarks:**

- Reference JIRA ticket: [CMSLITDPG-1359](https://its.cern.ch/jira/browse/CMSLITDPG-1359) 
- Sw tag in condDB: [L1Menu_Collisions2025_v1_0_0_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2025_v1_0_0_xml)
- Fw tag in condDB: [L1Menu_Collisions2025_v1_0_0-d1_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2025_v1_0_0-d1_xml)
- [GT updated](https://cms-talk.web.cern.ch/t/gt-mc-data-relval-update-of-the-gt-with-the-2025-l1t-menu-tag-l1menu-collisions2025-v1-0-0-xml/122657?u=caruta) accordingly
- The "L1Menu_Collisions2025_v1_0_0" was deployed online on April 25 starting from the cosmics run 391069.
