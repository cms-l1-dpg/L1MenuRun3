# L1Menu_CollisionsHeavyIons2024_v1_0_1

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2024_v1_0_1/L1Menu_CollisionsHeavyIons2024_v1_0_1.html)

**Comment:** 
New version of the L1 menu for the 2024 HeavyIons collisions.
This menu has been created by using the last version of TME `0.17.1`, grammar `0.13` and updated scales to `scales_2023_02_16`.
The menu development for the Heavy Ions runs is documented in [CMSLITDPG-1314](https://its.cern.ch/jira/browse/CMSLITDPG-1314).

<br/>

The following changes, from the last HI menu (`L1Menu_CollisionsHeavyIons2024_v1_0_0`), have been made:

   - Added 28 seeds:
      - `L1_SingleJet8/12/16/20/24/28_notZDC_OR_BptxAND`
      - `L1_SingleUncorrJet2/4/6/8/12/16/20/24/28_notZDC_OR_BptxAND`
      - `L1_DoubleJet8/12/16_DeltaPhi2p0_NotZDC1n_AND_BptxAND`
      - `L1_DoubleJet8/12/16_DeltaPhi2p0_ZDC1n_OR_BptxAND`
      - `L1_DoubleJet8/12/16_DeltaPhi2p0_notMinimumBiasHF2_BptxAND`
      - `L1_ZDC1n/2n_OR_MinimumBiasHF1_AND_BptxAND_copy`, `L1_MinimumBiasHF1_AND_BptxAND_copy` ([CMSHLT-3347](https://its.cern.ch/jira/browse/CMSHLT-3347))
      - `L1_ZDC1n_AND_AND_NotMBHF2OR_BptxAND`

   - Removed 29 seeds:
      - `L1_SingleUncorrJet2/4/6/8/12/16/20/24/28_ZDC1n_OR_BptxAND`
      - `L1_SingleUncorrJet2/4/6/8/12/16_ZDC1n_AsymXOR/XOR_NotPreBptx_BptxAND`
      - `L1_SingleJet8/12/16/20/24/28_ZDC1n_OR_BptxAND`
      - `L1_SingleIsoEG12_BptxAND`
      - `L1_ZDC1n_OR_AND_NotMBHF2_BptxAND`