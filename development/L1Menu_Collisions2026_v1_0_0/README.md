# L1Menu_Collisions2025_v1_3_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2026_v1_0_0/L1Menu_Collisions2026_v1_0_0.html)

**Comment:** 
First version of the first L1T menu for the 2026 pp data taking.
This menu has been created by using the last version of TME `0.17.2`, grammar `0.13.0` and `scales_2024_05_15`.

<br/>

The following changes, from the previous deployed L1T menu from 2025 `v1_3_0` have been made:


### New AXO model v6, with modified seed thresholds, removed the VVVTight Seed [CMSLITDPG-1506](https://its.cern.ch/jira/browse/CMSLITDPG-1506) 
- Modified the following seeds: 
     - `L1_AXO_VLoose`: `AXO-SCORE_VLoose`(2010) -> `AXO-SCORE_VLoose`(2899)
     - `L1_AXO_Loose`: `AXO-SCORE_Loose`(2375) -> `AXO-SCORE_Loose`(3257)
     - `L1_AXO_Medium`: `AXO-SCORE_Medium`(2801) -> `AXO-SCORE_Medium`(3541)
     - `L1_AXO_Tight`: `AXO-SCORE_Tight`(3318) -> `AXO-SCORE_Tight`(3865)
     - `L1_AXO_VTight`: `AXO-SCORE_VTight`(4762) -> `AXO-SCORE_VTight`(7874)
     - `L1_AXO_VVTight`: `AXO-SCORE_VVTight`(26375) -> `AXO-SCORE_VVTight`(11121)
     - `L1_AXO_VVVTight`: `AXO-SCORE_VVVTight`(44447) -> removed

### Modified CICADA seed thresholds, and added three new seeds for Parking at HLT [CMSLITDPG-1502](https://its.cern.ch/jira/browse/CMSLITDPG-1502) 
- Modified the following seeds: 
     - `L1_CICADA_VLoose`: `CICADA-CSCORE_55p75`(55.75) -> `CICADA-CSCORE_63`(63)
     - `L1_CICADA_Loose`: `CICADA-CSCORE_60p75`(60.75) -> `CICADA-CSCORE_66`(66)
     - `L1_CICADA_Medium`: `CICADA-CSCORE_62p25`(62.25) -> `CICADA-CSCORE_67`(67)
     - `L1_CICADA_Tight`: `CICADA-CSCORE_63p5`(63.5) -> `CICADA-CSCORE_68p75`(68.75)
     - `L1_CICADA_VTight`: `CICADA-CSCORE_66p25`(66.25) -> `CICADA-CSCORE_71p25`(71.25)
     - `L1_CICADA_VVTight`: `CICADA-CSCORE_116p5`(116.5) -> `CICADA-CSCORE_126`(126.0)
     - `L1_CICADA_VVVTight`: `CICADA-CSCORE_125`(125) -> `CICADA-CSCORE_133p25`(133.25)
     - `L1_CICADA_VVVTight`: `CICADA-CSCORE_135`(135) -> `CICADA-CSCORE_145`(145)
     - Added `L1_CICADA_Parking1`: `CICADA-CSCORE_83p35`(83.35)
     - Added `L1_CICADA_Parking2`: `CICADA-CSCORE_133p25`(133.25)
     - Added `L1_CICADA_Parking3`: `CICADA-CSCORE_145`(145)




--- 
<br/>

**Additional Remarks:**

<!--- Reference JIRA ticket: [CMSLITDPG-1404](https://its.cern.ch/jira/browse/CMSLITDPG-1404)
- Sw tag in condDB: [L1Menu_Collisions2025_v1_3_0_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2025_v1_3_0_xml)
- Fw tag in condDB: [L1Menu_Collisions2025_v1_1_1-d2_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2025_v1_3_0-d1_xml)
- [GT updated](https://cms-talk.web.cern.ch/t/update-of-the-gt-with-the-new-2025-l1t-menu-tag-l1menu-collisions2025-v1-3-0-xml/127751) accordingly
- The "L1Menu_Collisions2025_v1_3_0" was deployed online on August 18 starting from the collisions run 395982.
-->