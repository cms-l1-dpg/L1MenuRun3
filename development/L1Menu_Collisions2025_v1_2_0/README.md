# L1Menu_Collisions2025_v1_2_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2025_v1_2_0/L1Menu_Collisions2025_v1_2_0.html)

**Comment:** 
First version of the third L1T menu for the 2025 pp data taking.
This menu has been created by using the last version of TME `0.17.2`, grammar `0.13.0` and `scales_2024_05_15`.

<br/>

The following changes, from the previous deployed L1T menu `v1_0_0` have been made:

### Removed 3 unused seeds [CMSL1TDPG-1381](https://its.cern.ch/jira/browse/CMSLITDPG-1381) 
- Removed the following seeds (already removed by HLT): 
     - `L1_DoubleTau_Iso38_Iso26_er2p1_Jet55_RmOvlp_dR0p5`
     - `L1_DoubleTau_Iso40_Iso26_er2p1_Jet55_RmOvlp_dR0p5`

### Added new thresholds for the CICADA seeds [CMSLITDPG-1379](https://its.cern.ch/jira/browse/CMSLITDPG-1379) 
- Modified the following seed thresholds: 
     - `L1_CICADA_VLoose` : `CICADA-CSCORE_50`  -> `CICADA-CSCORE_55p75`
     - `L1_CICADA_Loose`  : `CICADA-CSCORE_60`  -> `CICADA-CSCORE_60p75`	
     - `L1_CICADA_Medium` : `CICADA-CSCORE_70`  -> `CICADA-CSCORE_62p25`
     - `L1_CICADA_Tight`  : `CICADA-CSCORE_80`  -> `CICADA-CSCORE_63p5`	
     - `L1_CICADA_VTight` : `CICADA-CSCORE_90`  -> `CICADA-CSCORE_66p25`
     - `L1_CICADA_VVTight`: `CICADA-CSCORE_110` -> `CICADA-CSCORE_116p5`	
--- 
<br/>

**Additional Remarks:**

- Reference JIRA ticket: [CMSLITDPG-1367](https://its.cern.ch/jira/browse/CMSLITDPG-1367) 
- Sw tag in condDB: [L1Menu_Collisions2025_v1_1_1_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2025_v1_1_1_xml)
- Fw tag in condDB: [L1Menu_Collisions2025_v1_1_1-d2_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2025_v1_1_1-d2_xml)
- [GT updated](https://cms-talk.web.cern.ch/t/gt-mc-data-relval-update-of-the-gt-with-the-new-2025-l1t-menu-tag-l1menu-collisions2025-v1-1-1-xml/124487) accordingly
- The "L1Menu_Collisions2025_v1_1_1" was deployed online on May 15 starting from the collisions run 392175.
