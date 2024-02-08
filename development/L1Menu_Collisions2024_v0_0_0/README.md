# L1Menu_Collisions2024_v0_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2024_v0_0_0/L1Menu_Collisions2024_v0_0_0.html)

**Comment:** 
First preliminary version of the L1T menu for the 2024 data taking.
This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The following changes, from the last menu of 2023 (`L1Menu_Collisions2023_v1_3_0`), have been made:

### New seeds BPH  [CMSLITDPG-1209](https://its.cern.ch/jira/browse/CMSLITDPG-1209), [CMSLITDPG-1211](https://its.cern.ch/jira/browse/CMSLITDPG-1211)     
   - Added 3 new seeds:
      - `L1_SingleMu10_SQ14_BMTF` (bit 198)
      - `L1_SingleMu11_SQ14_BMTF` (bit 199)
      - `L1_DoubleMu0er2p0_SQ_OS_dEta_Max0p3_dPhi_0p8to1p2` (bit 33)

### New seeds Displaced Muons [CMSLITDPG-1215](https://its.cern.ch/jira/browse/CMSLITDPG-1215)   
   - Added 3 new seeds:
      - `L1_DoubleMu6_Upt6_SQ_er2p0` (bit 509)
      - `L1_DoubleMu7_Upt7_SQ_er2p0` (bit 510)
      - `L1_DoubleMu8_Upt8_SQ_er2p0` (bit 511)

### New seeds for VBF parking (increased mjj threshold by 100, 150 GeV for backup option of exclusive seeds included in 2023)  [CMSLITDPG-1213](https://its.cern.ch/jira/browse/CMSLITDPG-1213)      
   - Added 11 new seeds:           
      - `L1_DoubleJet45_Mass_Min550_IsoTau45er2p1_RmOvlp_dR0p5` (bit 34)
      - `L1_DoubleJet45_Mass_Min600_IsoTau45er2p1_RmOvlp_dR0p5` (bit 35)
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min600_DoubleJetCentral50` (bit 36)
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min650_DoubleJetCentral50` (bit 37)
      - `L1_DoubleJet45_Mass_Min550_LooseIsoEG20er2p1_RmOvlp_dR0p2` (bit 38)
      - `L1_DoubleJet45_Mass_Min600_LooseIsoEG20er2p1_RmOvlp_dR0p2` (bit 39)
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min600_Mu3OQ` (bit 40)
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min650_Mu3OQ` (bit 41)
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min500_ETMHF65` (bit 58)
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min550_ETMHF65` (bit 59)
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min850` (bit 364)

### New seeds for HHbbWW [CMSLITDPG-1210](https://its.cern.ch/jira/browse/CMSLITDPG-1210) 
   - Added 4 new seeds: 
      - `L1_Mu12_HTT150er` (bit 434)
      - `L1_Mu14_HTT150er` (bit 435)
      - `L1_LooseIsoEG14er2p5_HTT200er` (bit 436)
      - `L1_LooseIsoEG16er2p5_HTT200er` (bit 437)

### New seeds for AXOL1TL [CMSLITDPG-1208](https://its.cern.ch/jira/browse/CMSLITDPG-1208)
   - Added 5 new seeds: 
      - `L1_AXO_VLoose`  (bit 438)
      - `L1_AXO_Loose`   (bit 439)
      - `L1_AXO_Nominal` (bit 440)
      - `L1_AXO_Tight`   (bit 441)
      - `L1_AXO_VTight`  (bit 442)

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.

