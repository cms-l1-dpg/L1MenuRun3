# L1Menu_CollisionsHeavyIons2024_v1_0_6

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2024_v1_0_6/L1Menu_CollisionsHeavyIons2024_v1_0_6.html)

**Comment:** 
Final version of the L1 menu for the 2024 HeavyIons collisions.
This menu has been created by using the last version of TME `0.17.1`, grammar `0.13` and updated scales to `scales_2023_02_16`.
The menu development for the Heavy Ions runs is documented in [CMSLITDPG-1314](https://its.cern.ch/jira/browse/CMSLITDPG-1314).

<br/>

The following changes, from the last HI menu (`L1Menu_CollisionsHeavyIons2024_v1_0_5`), have been made:

   - Modification of the thresholds of the L1 ZDC seeds to match the new ZDC LUTs, which increase the granularity of the selection from 1 count = 50 GeV to 1 count = 10 GeV.

   - Addition of 74 monitoring seeds (EG, jets and ZDC seeds…):
     - `L1_ZDCP/ZDCM110/_BptxAND`
     - `L1_ZDC1n_Bkp2_OR_BptxAND, L1_ZDC1n_Bkp1/2_AND_AND_NotMBHF2_BptxAND`
     - `L1_SingleEG6/7er2p1/8/9/10/10er2p1/15/18_BptxAND`
     - `L1_DoubleEG2er1p5/2er2p1/4/5er1p5/5er2p1/6er2p5/7er2p5/8er2p5/_NotMinimumBiasHF2_AND_BptxAND`
     - `L1_DoubleEG2er1p5/2er2p1_DeltaPhi2p0_NotMinimumBiasHF2_AND_BptxAND`
     - `L1_SingleJet8/12/16/20/24/28_notZDC_Bkp1/2_OR/XOR_BptxAND, L1_SingleJet8/12/16/20/24/28_ZDC1n_Bkp1/2_AsymXOR_BptxAND`
     - `L1_DoubleJet8/12/16_DeltaPhi2p0_notZDC_Bkp1/2_OR_BptxAND, L1_DoubleJet8/12/16_DeltaPhi2p0_NotZDC1n_Bkp1/2_AND_BptxAND`
     - `L1_SingleMuOpen_Centrality_50_100_BptxAND`

  - Removal of 68 seeds not used by HLT (ZDC monitoring seeds and low threshold UncorrJets):
     - `L1_ZDCP/ZDCM14/16/18/22/28_AND/_OR/_BptxAND/_AND/OR_BptxAND`
     - `L1_SingleUncorrJet2/4/6_ZDC1n_Bkp1_XOR/AsymXOR/OR_BptxAND`
     - `L1_SingleUncorrJet2/4/6_NotMinimumBiasHF2_AND_BptxAND, L1_DoubleUncorrJet2/4/6_DeltaPhi2p0_notMinimumBiasHF2_BptxAND`
     - `L1_SingleUncorrJet2/4/6_notZDC_OR_BptxAND, L1_DoubleUncorrJet2/4/6_DeltaPhi2p0_NotZDC1n_AND_BptxAND`
     - `L1_ZDC1n_AND_AND_NotMBHF2OR_BptxAND`

**Additional Remarks:**
- Synthesized, validated and tested in uGT test crate [CMSLITDPG-1322](https://its.cern.ch/jira/browse/CMSLITDPG-1322)
- Sw tag in condDB uploaded: [L1Menu_CollisionsHeavyIons2024_v1_0_6_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_CollisionsHeavyIons2024_v1_0_6_xml)
- The L1Menu_CollisionsHeavyIons2024_v1_0_6_xml was deployed online for the HeavyIons runs starting from run 387973 on 9th Nov 2024.