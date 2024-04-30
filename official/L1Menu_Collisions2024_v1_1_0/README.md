# L1Menu_Collisions2024_v1_1_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2024_v1_1_0/L1Menu_Collisions2024_v1_1_0.html)

**Comment:** 
Second L1T menu for the 2024 pp data taking, with the updated UTM grammar (`0.12.0`).
This menu has been created by using the last version of TME `0.16.0`, grammar `0.12.0` and `scales_2023_02_16`.

<br/>

The following changes, from the first menu of 2024 (`L1Menu_Collisions2024_v1_0_0`), have been made:

### Seeds for AXOL1TL [CMSLITDPG-1208](https://its.cern.ch/jira/browse/CMSLITDPG-1208)
   - Modified the following 5 new seeds to use the new UTM grammar (NN model version used: [v3](https://globaltrigger.web.cern.ch/upgrade/tme/models)), and [fixed the AXO thresholds](https://its.cern.ch/jira/browse/CMSLITDPG-1208?focusedId=6306964&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel#comment-6306964): 
      - `L1_AXO_VLoose`  (bit 438)
      - `L1_AXO_Loose`   (bit 439)
      - `L1_AXO_Nominal` (bit 440)
      - `L1_AXO_Tight`   (bit 441)
      - `L1_AXO_VTight`  (bit 442)

### Removal of 12 unused seeds (transparent to HLT) [CMSLITDPG-1228](https://its.cern.ch/jira/browse/CMSLITDPG-1228)
   - Removed the following seeds: 
      - `L1_SingleIsoTau32er2p1` 
      - `L1_SingleTau70er2p1`
      - `L1_Mu12er2p3_Jet40er2p1_dR_Max0p4_DoubleJet40er2p1_dEta_Max1p6`
      - `L1_DoubleMu3_dR_Max1p6_Jet90er2p5_dR_Max0p8`
      - `L1_DoubleMu3_SQ_HTT240er`
      - `L1_DoubleMu3_SQ_HTT260er`
      - `L1_TripleEG16er2p5`
      - `L1_LooseIsoEG30er2p1_HTT100er`
      - `L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p1`
      - `L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p6`
      - `L1_SingleJet140er2p5_ETMHF90`
      - `L1_ETT1600`

### Addition of 3 MHT monitoring seeds [CMSLITDPG-1229](https://its.cern.ch/jira/browse/CMSLITDPG-1229)
   - Added the following seeds: 
      - `L1_MHT120` (bit 434)
      - `L1_MHT150` (bit 435)
      - `L1_MHT200` (bit 436)

 ### Addition of 4 BMTF high quality single muon displaced seeds [CMSLITDPG-1231](https://its.cern.ch/jira/browse/CMSLITDPG-1231)
   - Added the following seeds: 
      - `L1_SingleMu0_Upt10_SQ14_BMTF` (bit 198)
      - `L1_SingleMu0_Upt15_SQ14_BMTF` (bit 199)
      - `L1_SingleMu0_Upt20_SQ14_BMTF` (bit 200)
      - `L1_SingleMu0_Upt25_SQ14_BMTF` (bit 201)
    
**Additional Remarks:**

- Reference JIRA ticket: [CMSLITDPG-1221](https://its.cern.ch/jira/browse/CMSLITDPG-1221)
- Sw tag in condDB: [L1Menu_Collisions2024_v1_1_0_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2024_v1_1_0_xml)
- Fw tag in condDB: [L1Menu_Collisions2024_v1_1_0-d1_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2024_v1_1_0-d1_xml)
- [GT updated](https://cms-talk.web.cern.ch/t/update-of-the-2024-l1t-menu-tag-l1menu-collisions2024-v1-1-0/37795) accordingly
- Fw [L1Menu_Collisions2024_v1_1_0-d1_xml](https://raw.githubusercontent.com/cms-l1-globaltrigger/cms-l1-menu/L1Menu_Collisions2024_v1_1_0-d1/2024/L1Menu_Collisions2024_v1_1_0-d1/xml/L1Menu_Collisions2024_v1_1_0-d1.xml)
- The "L1Menu_Collisions2024_v1_1_0" was deployed online during run 378492.

