# L1Menu_CollisionsHeavyIons2025_v1_0_3

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2025_v1_0_3/L1Menu_CollisionsHeavyIons2025_v1_0_3.html)

**Comment:** 
Final version of the L1 menu for the 2025 HeavyIons collisions.
This menu has been created by using the last version of TME `0.17.2`, grammar `0.13.0` and `scales_2024_05_15`.
The menu development for the Heavy Ions runs is documented in [CMSLITDPG-1455](https://its.cern.ch/jira/browse/CMSLITDPG-1455).

<br/>

The following changes, from the last HI menu (`L1Menu_CollisionsHeavyIons2024_v1_0_6`), have been made:

    - removal of unused triggers (e.g. uncorrected jets, rapidity-gap triggers, SingleEG SingleMu cross-triggers)
    - addition of ZDC monitoring seeds inspired from the 2025 OO menu
    - addition of triggers with non-zero prescales from menus used in cosmics and circulating runs
    - addition of double jet delta phi + ZDC triggers (e.g. L1_DoubleJet*_DeltaPhi2p0_UPCZDC1n_Th#_XOR_BptxAND), with *=8,12,16 and #=1,2,3
    - addition of a new set of seeds for soft photonuclear interactions - L1_UPCZDC1n_Th#_XOR_MinimumBiasHF&_OR_SameSide_BptxAND, with #=1,2,3 and &=1,2 thresholds
    - addition of backup eta- and Bptx-gated EG triggers.

**Additional Remarks:**
- Synthesized, validated and tested in uGT test crate [CMSLITDPG-1455](https://its.cern.ch/jira/browse/CMSLITDPG-1455)
- Sw tag in condDB uploaded: [L1Menu_CollisionsHeavyIons2025_v1_0_3_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_CollisionsHeavyIons2025_v1_0_3_xml)
- The L1Menu_CollisionsHeavyIons2025_v1_0_3_xml was deployed online in the spare crate for the HeavyIons runs starting from run 398409 on 22nd Oct 2025.