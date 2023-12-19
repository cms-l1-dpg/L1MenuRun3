# L1Menu_Collisions2023_v1_3_0_for2024_v2

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_3_0_for2024_v2/L1Menu_Collisions2023_v1_3_0_for2024_v2.html)

**Comment:** 
Second version of the L1 menu for a skim in view of the 2024 physics data taking, including tigher thresholds for VBF parking seeds.
This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The following changes, from the last menu of 2023 (`L1Menu_Collisions2023_v1_3_0`), have been made:

### New seeds BPH   
   - Added 2 new seeds:
      - `L1_SingleMu10_SQ14_BMTF` (bit 198)
      - `L1_SingleMu11_SQ14_BMTF` (bit 199)

### New seeds Displaced Muons  
   - Added 2 new seeds:
      - `L1_DoubleMu6_Upt6_SQ_er2p0` (bit 510)
      - `L1_DoubleMu7_Upt7_SQ_er2p0` (bit 511)

### New seeds for VBF parking exclusive
Increased mjj threshold by 100 and 150 GeV for backup option of exclusive seeds included in 2023.     
   - Added 10 new seeds:           
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

### New seeds for VBF parking inclusive
Increased mjj threshold by 100 and 150 GeV for VBF inclusive seed used as baseline for 2024.
   - Added 2 new seeds:           
      - `L1_DoubleJet_100_30_DoubleJet30_Mass_Min900` (bit 360)
      - `L1_DoubleJet_100_30_DoubleJet30_Mass_Min950` (bit 361)

### New seeds for HHbbWW  
   - Added 2 new seeds: 
      - `L1_Mu12_HTT150er` (bit 434)
      - `L1_LooseIsoEG16er2p1_HTT200er` (bit 435)


**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
