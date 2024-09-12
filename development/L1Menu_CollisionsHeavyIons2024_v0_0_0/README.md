# L1Menu_CollisionsHeavyIons2024_v0_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2024_v0_0_0/L1Menu_CollisionsHeavyIons2024_v0_0_0.html)

**Comment:** 
First version of the L1 menu for the 2024 HeavyIons collisions.
This menu has been created by using the last version of TME `0.17.1`, grammar `0.13` and updated scales to `scales_2023_02_16`.
The menu development for the Heavy Ions runs is documented in [CMSLITDPG-1314](https://its.cern.ch/jira/browse/CMSLITDPG-1314).

<br/>

The following changes, from the last 2023 HI menu (`L1Menu_CollisionsHeavyIons2023_v1_1_5`), have been made:

### New muon seeds
   - Added 76 new seeds:
      - 3 new L1 seeds to improve the efficiency for quarkonia in peripheral hadronic collisions
          - `L1_SingleMu0_Centrality_40_100_BptxAND` 
          - `L1_DoubleMu0_SQ_BptxAND` 
          - `L1_SingleMuOpen_Centrality_30_100_BptxAND` 
      - 73 new L1 seeds for ultraperipheral collisions (UPC). N.B.: the tau object is used in these seeds as a “jet w/o jet JECs and PU subtraction” (referred to as “UPCJet” in seed naming). The agreement with HI team is to modify only the Calo firmware, such that the Tau collection is filled with the uncorrected jets (no modification at emulator foreseen).
          - `L1_ZDC1n_OR_AND_NotMBHF2_BptxAND` 
          - `L1_ZDC1n_AND_AND_NotMBHF2_BptxAND`     
          - `L1_SingleUPCJet2/4/6/8/12/16/20/24/28_ZDC1n_XOR_BptxAND`
          - `L1_SingleUPCJet2/4/6/8/12/16/20/24/28_ZDC1n_OR_BptxAND` 
          - `L1_SingleUPCJet6/8/12/16/20/24/28_ZDC1n_AsymXOR_NotPreBptx_BptxAND`
          - `L1_SingleUPCJet6/8/12/16/20/24/28_ZDC1n_XOR_NotPreBptx_BptxAND`
          - `L1_SingleUPCJet2/4/6/8/12/16/20/24/28_ZDC1n_AsymXOR_BptxAND`
          - `L1_SingleUPCJet2/4/6/8/12/16/20/24/28_NotMinimumBiasHF2_AND_BptxAND`
          - `L1_DoubleUPCJet2/4/6/8/12_DeltaPhi2p0_ZDC1n_OR_BptxAND`
          - `L1_DoubleUPCJet2/4/6/8/12_DeltaPhi2p0_NotZDC1n_AND_BptxAND`
          - `L1_DoubleUPCJet2/4/6/8/12_DeltaPhi2p0_notMinimumBiasHF2_BptxAND`
          - `L1_SingleJet8/12/16/20/24/28_ZDC1n_OR_BptxAND`
   - Removed 36 seeds:
          - `L1_SingleJet24_ETM10/15/30/50_ZDC1n_XOR_BptxAND`
          - `L1_SingleJet24_HTM10/15/30/50_ZDC1n_XOR_BptxAND`
          - `L1_SingleJet24_ETM10/15/30/50_ZDC1n_AsymXOR_BptxAND`
          - `L1_SingleJet24_HTM10/15/30/50_ZDC1n_AsymXOR_BptxAND`
          - `L1_SingleJet8/12/16/20/24/28_ZDC1n_XOR_MidEta2p5_BptxAND`
          - `L1_SingleJet8/12/16/20/24/28_ZDC1n_AsymXOR_MidEta2p5_BptxAND`
          - `L1_DoubleJet_16_12_ZDC1n_AsymXOR/XOR_BptxAND`
          - `L1_DoubleJet_24_16_ZDC1n_AsymXOR/XOR_BptxAND`
          - `L1_DoubleJet_8_8_ZDC1n_AsymXOR/XOR_BptxAND`
          - `L1_DoubleJet_12_8_ZDC1n_AsymXOR/XOR_BptxAND`
   

