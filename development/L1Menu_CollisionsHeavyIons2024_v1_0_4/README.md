# L1Menu_CollisionsHeavyIons2024_v1_0_4

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2024_v1_0_4/L1Menu_CollisionsHeavyIons2024_v1_0_4.html)

**Comment:** 
Final version of the L1 menu for the 2024 HeavyIons collisions.
This menu has been created by using the last version of TME `0.17.1`, grammar `0.13` and updated scales to `scales_2023_02_16`.
The menu development for the Heavy Ions runs is documented in [CMSLITDPG-1314](https://its.cern.ch/jira/browse/CMSLITDPG-1314).

<br/>

The following changes, from the last HI menu (`L1Menu_CollisionsHeavyIons2024_v1_0_3`), have been made:

   - Changed names of rapidity gap seeds (now labelled consistently as “RapGap”):
     - `L1_ZDC1n_OR_RapGap_BptxAND`
     - `L1_SingleJet2/4/6/8/12/16/20/24/28_ZDC1n_XOR_RapGap_BptxAND`
   - Removed 9 seeds that won’t be used for the PbPb data taking:
     - `L1_DoubleUncorrJet2/4/6/8/12/16_DeltaPhi2p0_ZDC1n_OR_BptxAND`
     - `L1_DoubleJet8/12/16_DeltaPhi2p0_ZDC1n_OR_BptxAND`
