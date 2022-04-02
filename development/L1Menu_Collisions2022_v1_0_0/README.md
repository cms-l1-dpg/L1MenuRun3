# L1Menu_Collisions2022_v1_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/caruta/L1MenuRun3/blob/patch-1/development/L1Menu_Collisions2022_v1_0_0/L1Menu_Collisions2022_v1_0_0.html)

**Comment:** 
New version of the menu for Run3 for integration in CMSSW_12_3. 

Summary of the modifications done (detailed list, especially for reordering, in https://docs.google.com/spreadsheets/d/1WKz3Nl0gIOeoM03cUgKJwZ5rOQ4LS_lyGjZM_5AFCj4/edit#gid=232727380 ):

- Deletion of duplicated seeds (bits 34, 35, 36, 50, 93, 94, 114, 115, 116, 117, 281, 299, 368, 369, 370, 371, 391, 392, 493, 495, 496, 497, 498, 499, 502, 507, 508, 509, 510, 511) -> JIRA: https://its.cern.ch/jira/browse/CMSHLT-2258

- Deletion of unused seeds -> JIRA: https://its.cern.ch/jira/browse/CMSHLT-2249 
    - L1_IsoTau40er2p1_ETMHF80 (bit 291)
    - L1_IsoTau40er2p1_ETMHF90 (bit 292)
    - L1_IsoTau40er2p1_ETMHF100 (bit 293)
    - L1_IsoTau40er2p1_ETMHF110 (bit 294)
    - L1_IsoEG32er2p5_Mt44 (bit 198)
    - L1_IsoEG32er2p5_Mt48 (bit 199)

- Modifications in single tau monitoring seeds -> JIRA: https://its.cern.ch/jira/browse/CMSLITDPG-964
    - removed: 
        - L1_SingleIsoTau30er2p1 (bit 261)
        - L1_SingleIsoTau36er2p1 (bit 263)
    - added:
        - L1_SingleTau70er2p1 (bit 263)

- Modifications of seeds with Upt -> JIRA: https://its.cern.ch/jira/browse/CMSLITDPG-959
    - "L1_DoubleMu0_upt6_IP_Min1_upt4" -> "L1_DoubleMu0_Upt6_IP_Min1_Upt4" (bit 49)
    - “L1_DoubleMu0_upt15_upt7” -> “L1_DoubleMu0_Upt15_Upt7” (bit 50)

- Modifications in seeds for Tau3mu search -> JIRA: https://its.cern.ch/jira/browse/CMSLITDPG-960
    - removed "L1_TripleMu_2_1p5_0OQ_Mass_Max15" (bit 81)
    - modified "L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max15" -> "L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12"  (bit 82)
    - added seed for systematics evaluation: "L1_TripleMu_2SQ_1p5SQ_0OQ" (bit 74)

- Addition of seeds for systematics evaluation for Bmumu -> JIRA: https://its.cern.ch/jira/browse/CMSLITDPG-951
    - "L1_DoubleMu0er2p0_SQ_dEta_Max1p6" (bit 53)
    - "L1_DoubleMu0er2p0_SQ_dEta_Max1p5" (bit 54)
    

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
