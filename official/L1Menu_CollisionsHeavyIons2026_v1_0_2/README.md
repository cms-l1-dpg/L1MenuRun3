# L1Menu_CollisionsHeavyIons2026_v1_0_2

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2026_v1_0_2/L1Menu_CollisionsHeavyIons2026_v1_0_2.html)

**Comment:** 
Final version of the L1 menu for the 2026 HeavyIons collisions.
This menu has been created by using the last version of TME `0.17.2`, grammar `0.13.0` and `scales_2024_05_15`.
The menu development for the Heavy Ions runs is documented in [CMSLITDPG-1517](https://its.cern.ch/jira/browse/CMSLITDPG-1517).

<br/>

The following changes, from the last HI menu (`L1Menu_CollisionsHeavyIons2025_v1_0_3`), have been made:

    - removal of unused physics triggers.
    - addition of new beam-background monitoring seeds motivated by the beam-backgrounds observed during the 2025 PbPb run. These are triggers that look at single-side forward activity (ZDC, HF) with BtpxAND and NotBptxOR conditions. A subset of these will have dedicated HLT paths and will be read out at a low rate (few Hz) for offline studies during data taking.
    - addition of a contingency Light-by-Light trigger with a slightly increased energy threshold and an additional Δφ requirement.
    - minor cleanup and consolidation of the menu structure where appropriate.


**Additional Remarks:**
- Synthesized, validated and tested in uGT test crate [CMSLITDPG-1517](https://its.cern.ch/jira/browse/CMSLITDPG-1517)
- Sw tag in condDB uploaded: [L1Menu_CollisionsHeavyIons2026_v1_0_2_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_CollisionsHeavyIons2026_v1_0_2_xml)