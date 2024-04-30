# L1Menu_Collisions2024_v1_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2024_v1_0_0/L1Menu_Collisions2024_v1_0_0.html)

**Comment:** 
First version of the L1T menu for the 2024 data taking.
This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The following changes, from the last menu of 2023 (`L1Menu_Collisions2023_v1_3_0`), have been made:

### New seeds BPH  [CMSLITDPG-1209](https://its.cern.ch/jira/browse/CMSLITDPG-1209), [CMSLITDPG-1211](https://its.cern.ch/jira/browse/CMSLITDPG-1211)     
   - Added 3 new seeds:
      - `L1_SingleMu10_SQ14_BMTF` (bit 23)
      - `L1_SingleMu11_SQ14_BMTF` (bit 24)
      - `L1_DoubleMu0er2p0_SQ_OS_dEta_Max0p3_dPhi_0p8to1p2` (bit 72)
      - [`L1_SingleMu0_BMTF` already in the menu (bit 9) `PS:0->2000`]

### New seeds Displaced Muons  [CMSLITDPG-1215](https://its.cern.ch/jira/browse/CMSLITDPG-1215)   
   - Added 6 new seeds:
      - `L1_DoubleMu0_Upt6_SQ_er2p0` (bit 52)
      - `L1_DoubleMu0_Upt7_SQ_er2p0` (bit 53)  
      - `L1_DoubleMu0_Upt8_SQ_er2p0` (bit 54)  
      - `L1_DoubleMu6_Upt6_SQ_er2p0` (bit 55)
      - `L1_DoubleMu7_Upt7_SQ_er2p0` (bit 56)
      - `L1_DoubleMu8_Upt8_SQ_er2p0` (bit 57)
  
### New seeds for VBF parking (increased mjj threshold by 100, 150 GeV for backup option of seeds included in 2023)  [CMSLITDPG-1213](https://its.cern.ch/jira/browse/CMSLITDPG-1213)      
   - Added 11 new seeds:           
      - `L1_DoubleJet45_Mass_Min550_IsoTau45er2p1_RmOvlp_dR0p5` (bit 362)
      - `L1_DoubleJet45_Mass_Min600_IsoTau45er2p1_RmOvlp_dR0p5` (bit 363)
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min600_DoubleJetCentral50` (bit 364)
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min650_DoubleJetCentral50` (bit 365)
      - `L1_DoubleJet45_Mass_Min550_LooseIsoEG20er2p1_RmOvlp_dR0p2` (bit 366)
      - `L1_DoubleJet45_Mass_Min600_LooseIsoEG20er2p1_RmOvlp_dR0p2` (bit 367)
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min600_Mu3OQ` (bit 368)
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min650_Mu3OQ` (bit 369)
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min500_ETMHF65` (bit 370)
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min550_ETMHF65` (bit 371)
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min850` (bit 358)

### New seeds for HHbbWW [CMSLITDPG-1210](https://its.cern.ch/jira/browse/CMSLITDPG-1210) 
   - Added 4 new seeds: 
      - `L1_Mu12_HTT150er` (bit 138)
      - `L1_Mu14_HTT150er` (bit 139)
      - `L1_LooseIsoEG14er2p5_HTT200er` (bit 241)
      - `L1_LooseIsoEG16er2p5_HTT200er` (bit 242)

### New seeds for AXOL1TL [CMSLITDPG-1208](https://its.cern.ch/jira/browse/CMSLITDPG-1208)
   - Added 5 new seeds: 
      - `L1_AXO_VLoose`  (bit 438)
      - `L1_AXO_Loose`   (bit 439)
      - `L1_AXO_Nominal` (bit 440)
      - `L1_AXO_Tight`   (bit 441)
      - `L1_AXO_VTight`  (bit 442)

### New muon monitoring seeds for new BMTF quality selection commissioning [CMSLITDPG-1220](https://its.cern.ch/jira/browse/CMSLITDPG-1220)
   - Added 3 new seeds:   
      - `L1_SingleMu0_SQ13_BMTF` (bit 12) 
      - `L1_SingleMu0_SQ14_BMTF` (bit 13)
      - `L1_SingleMu0_SQ15_BMTF` (bit 14)

### Removed the following seeds:
   - 14 Low pT DoubleEG seeds previously used for Dielectron parking [CMSLITDPG-1212](https://its.cern.ch/jira/browse/CMSLITDPG-1212)
      - `L1_DoubleEG4_er1p2_dR_Max0p9` 
      - `L1_DoubleEG4p5_er1p2_dR_Max0p9` 
      - `L1_DoubleEG5_er1p2_dR_Max0p9` 
      - `L1_DoubleEG5p5_er1p2_dR_Max0p8` 
      - `L1_DoubleEG6_er1p2_dR_Max0p8` 
      - `L1_DoubleEG6p5_er1p2_dR_Max0p8` 
      - `L1_DoubleEG7_er1p2_dR_Max0p8` 
      - `L1_DoubleEG7p5_er1p2_dR_Max0p7` 
      - `L1_DoubleEG8_er1p2_dR_Max0p7` 
      - `L1_DoubleEG8p5_er1p2_dR_Max0p7` 
      - `L1_DoubleEG9_er1p2_dR_Max0p7`  
      - `L1_DoubleEG9p5_er1p2_dR_Max0p6` 
      - `L1_DoubleEG10_er1p2_dR_Max0p6` 
      - `L1_DoubleEG10p5_er1p2_dR_Max0p6`

   - 19 seeds previously used for the VBF parking [CMSLITDPG-1213](https://its.cern.ch/jira/browse/CMSLITDPG-1213)
      - `L1_DoubleJet35_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5`
      - `L1_DoubleJet45_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5`
      - `L1_DoubleJet_80_30_Mass_Min420_DoubleMu0_SQ`
      - `L1_DoubleJet_60_30_DoubleJet30_Mass_Min500_DoubleJetCentral50`
      - `L1_DoubleJet_65_35_DoubleJet35_Mass_Min500_DoubleJetCentral50`
      - `L1_DoubleJet40_Mass_Min450_IsoEG10er2p1_RmOvlp_dR0p2`
      - `L1_DoubleJet40_Mass_Min450_LooseIsoEG15er2p1_RmOvlp_dR0p2`
      - `L1_DoubleJet45_Mass_Min450_LooseIsoEG20er2p1_RmOvlp_dR0p2`
      - `L1_DoubleJet_80_30_DoubleJet30_Mass_Min500_Mu3OQ`
      - `L1_DoubleJet_85_35_DoubleJet35_Mass_Min500_Mu3OQ`
      - `L1_DoubleJet_65_30_DoubleJet30_Mass_Min400_ETMHF65`
      - `L1_DoubleJet_70_35_DoubleJet35_Mass_Min400_ETMHF65`
      - `L1_DoubleJet_90_30_DoubleJet30_Mass_Min620`
      - `L1_DoubleJet_90_30_DoubleJet30_Mass_Min800`
      - `L1_DoubleJet_100_30_DoubleJet30_Mass_Min620`
      - `L1_DoubleJet_100_30_DoubleJet30_Mass_Min800`
      - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min620` 
      - `L1_DoubleJet_115_40_DoubleJet40_Mass_Min620`
      - `L1_DoubleJet_120_45_DoubleJet45_Mass_Min620`

   - 3 seeds previously added for Displaced Muon searches [CMSLITDPG-1215](https://its.cern.ch/jira/browse/CMSLITDPG-1215) 
      - `L1_DoubleMu0_Upt5_Upt5_BMTF_EMTF` 
      - `L1_DoubleMu0_Upt6_IP_Min1_Upt4_BMTF_EMTF`
      - `L1_DoubleMu0_Upt15_Upt7_BMTF_EMTF`

   - 4 seeds added during 2018 seeds and never active during Run 3 [CMSLITDPG-631](https://its.cern.ch/jira/browse/CMSLITDPG-631), [CMSLITDPG-625](https://its.cern.ch/jira/browse/CMSLITDPG-625)
      - `L1_DoubleIsoTau28er2p1_Mass_Max90`  
      - `L1_DoubleIsoTau28er2p1_Mass_Max80`
      - `L1_DoubleIsoTau30er2p1_Mass_Max90`
      - `L1_DoubleIsoTau30er2p1_Mass_Max80`

**Additional Remarks:**

- Reference JIRA ticket: [CMSLITDPG-1221](https://its.cern.ch/jira/browse/CMSLITDPG-1221)
- Sw tag in condDB: [L1Menu_Collisions2024_v1_0_0_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2024_v1_0_0_xml)
- Fw tag in condDB: [L1Menu_Collisions2024_v1_0_0-d1_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2024_v1_0_0-d1_xml)
- [GT updated](https://cms-talk.web.cern.ch/t/update-of-the-2024-l1-menu-tag-l1menu-collisions2024-v1-1-0/35509) accordingly
- Fw created: [L1Menu_Collisions2024_v1_0_0-d1.xml](https://raw.githubusercontent.com/cms-l1-globaltrigger/cms-l1-menu/master/2024/L1Menu_Collisions2024_v1_0_0-d1/xml/L1Menu_Collisions2024_v1_0_0-d1.xml)

- The `L1Menu_Collisions2024_v1_0_0` was deployed online on 26th March, 2024 during (the special ECAL) run `378492`.

- N.B. The new AXO seeds are temporarily disabled in the PS table, as well as the new displaced muon seeds ([CMSHLT-3130](https://its.cern.ch/jira/browse/CMSHLT-3130)) 
