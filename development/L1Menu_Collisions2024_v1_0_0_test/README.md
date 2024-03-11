# L1Menu_Collisions2024_v1_0_0_test

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2024_v1_0_0_test/L1Menu_Collisions2024_v1_0_0_test.html)

**Comment:** 
Test version of the 2024 L1T menu for the debugging of the [mismatches observed](https://its.cern.ch/jira/browse/CMSLITDPG-1221?focusedId=6304840&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel#comment-6304840) between fw and emulator for the first 2024 menu for data taking.
This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The differences w.r.t. menu `L1Menu_Collisions2024_v1_0_0` are listed below.
   - The seed `L1_DoubleMu6_Upt6_SQ_er2p0` (bit 55) has been split into its main 3 conditions:
      - `L1_DoubleMu6_Upt6_SQ_er2p0_part1` (bit 508): 2 muons in BMTF or EMTF(|eta|<2) with unconstrained pT>6 GeV
      - `L1_DoubleMu6_Upt6_SQ_er2p0_part2` (bit 509): 2 muons in OMTF with pT>6 GeV
      - `L1_DoubleMu6_Upt6_SQ_er2p0_part3` (bit 510): 1 muons in BMTF or EMTF(|eta|<2) with unconstrained pT>6 GeV + 1 muon in OMTF with pT>6GeV
   - In addition, another version of the bit 55 has been created:  
      - `L1_DoubleMu6_Upt6_SQ_er2p0_v2` (bit 511): the MU-INDEX cut has been used as much as possible, substituting the MU-ETA cut in the previous version of the seed. 
