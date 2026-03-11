# L1Menu_Collisions2026_v1_1_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2026_v1_1_0/L1Menu_Collisions2026_v1_1_0.html)

**Comment:** 
First version of the second L1T menu for the 2026 pp data taking.
This menu has been created by using the last version of TME `0.17.2`, grammar `0.13.0` and `scales_2024_05_15`.

<br/>

The following changes, from the previous deployed L1T menu from 2026 `v1_0_0` have been made:


### Updated AXO model v6 to fix a bug in the derivation of the pure rates, with modified seed thresholds [CMSLITDPG-1511](https://its.cern.ch/jira/browse/CMSLITDPG-1511): 
- Modified the following seeds: 
     - `L1_AXO_VLoose`: `AXO-SCORE_VLoose`(2899) -> `AXO-SCORE_VLooseNew`(2016)
     - `L1_AXO_Loose`: `AXO-SCORE_Loose`(3257) -> `AXO-SCORE_LooseNew`(2335)
     - `L1_AXO_Medium`: `AXO-SCORE_Medium`(3541) -> `AXO-SCORE_MediumNew`(2717)
     - `L1_AXO_Tight`: `AXO-SCORE_Tight`(3865) -> `AXO-SCORE_TightNew`(3103)
     - `L1_AXO_VTight`: `AXO-SCORE_VTight`(7874) -> `AXO-SCORE_VTightNew`(7500)
     - `L1_AXO_VVTight`: `AXO-SCORE_VVTight`(111121) -> `AXO-SCORE_VVTightNew`(10338)

### New seeds added for low pileup run [CMSLITDPG-1510](https://its.cern.ch/jira/browse/CMSLITDPG-1510):
- L1_SingleEG23er2p5
- L1_SingleJet35_BptxAND
- L1_DoubleJet20er2p5
- L1_DoubleJet30er2p5
- L1_DoubleJet35er2p5
- L1_DoubleJet45er2p5
- L1_TripleJet20er2p5
- L1_TripleJet30er2p5
- L1_TripleJet30er2p5
- L1_TripleJet35er2p5
- L1_SingleEG21er2p5_BptxAND
- L1_SingleJet60_BptxAND
- L1_SingleJet90_BptxAND

### Additional MinimumBias Seeds for 1.2+1.2 TeV special run [CMSLITDPG-1512](https://its.cern.ch/jira/browse/CMSLITDPG-1512):
- L1_MinimumBiasHF1_AND
- L1_MinimumBiasHF1_OR
- L1_MinimumBiasHF1_AND_BptxAND
- L1_MinimumBiasHF1_OR_BptxAND
- L1_MinimumBiasHF2_AND
- L1_MinimumBiasHF2_OR
- L1_MinimumBiasHF2_AND_BptxAND
- L1_MinimumBiasHF2_OR_BptxAND

--- 
<br/>

**Additional Remarks:**

<!--- Reference JIRA ticket: [CMSLITDPG-1404](https://its.cern.ch/jira/browse/CMSLITDPG-1404)
- Sw tag in condDB: [L1Menu_Collisions2025_v1_3_0_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2025_v1_3_0_xml)
- Fw tag in condDB: [L1Menu_Collisions2025_v1_1_1-d2_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2025_v1_3_0-d1_xml)
- [GT updated](https://cms-talk.web.cern.ch/t/update-of-the-gt-with-the-new-2025-l1t-menu-tag-l1menu-collisions2025-v1-3-0-xml/127751) accordingly
- The "L1Menu_Collisions2025_v1_3_0" was deployed online on August 18 starting from the collisions run 395982.
-->