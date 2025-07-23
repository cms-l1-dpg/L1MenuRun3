# L1Menu_Collisions2025_v1_3_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2025_v1_3_0/L1Menu_Collisions2025_v1_3_0.html)

**Comment:** 
First version of the fourth L1T menu for the 2025 pp data taking.
This menu has been created by using the last version of TME `0.17.2`, grammar `0.13.0` and `scales_2024_05_15`.

<br/>

The following changes, from the previous deployed L1T menu `v1_2_0` have been made:


### Modified thresholds for the VVTight and VVVTight AXO seeds [CMSLITDPG-1398](https://its.cern.ch/jira/browse/CMSLITDPG-1398) 
- Modified the following seed thresholds: 
     - `L1_AXO_VVTight`: `AXO-SCORE_VVTight`(22628) -> `AXO-SCORE_VVVTight`(26375)
     - `L1_AXO_VVVTight`: `AXO-SCORE_VVVTight`(26375) -> `AXO-SCORE_NewVVVTight`(44447)

### Added three seeds (prescaled to zero) to help debug the rate increase of L1_SingleJet20er2p5_NotBptxOR [CMSL1TDPG-1397](https://its.cern.ch/jira/browse/CMSLITDPG-1397) 
- Added the following seeds:
     - `L1_SingleJet20er1p3_NotBptxOR`: up to abseta 1.305
     - `L1_SingleJet20er1p3to2p5_NotBptxOR`: spanning from abseta 1.392 to 2.52
     - `L1_SingleJet30er2p5_NotBptxOR`: higher pT

--- 
<br/>
