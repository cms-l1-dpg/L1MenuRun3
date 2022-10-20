# L1Menu_CollisionsHeavyIons2022_v1_1_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2022_v1_1_0/L1Menu_CollisionsHeavyIons2022_v1_1_0.html)

**Comment:** L1Menu for the Heavy Ions test planned for November 2022.
Ten additional seeds, w.r.t. the previous version (v1_0_1), were included to make the L1 menu compatible with the HLT one, as reported in JIRA [CMSHLT-2507](https://its.cern.ch/jira/browse/CMSHLT-2507).
The seeds added are the following:
- L1_DoubleEG2_BptxAND (bit 396)
- L1_DoubleEG5_BptxAND (bit 397)

- L1_SingleMu3Open_BptxAND (bit 185)
- L1_DoubleMuOpen_Centrality_50_100_BptxAND (bit 249)
- L1_DoubleMuOpen_Centrality_40_100_BptxAND (bit 248)
- L1_DoubleMuOpen_Centrality_30_100_BptxAND (bit 247)

- L1_SingleEG3 (bit 70)
- L1_SingleEG5 (bit 71)
- L1_Centrality_30_100_MinimumBiasHF1_AND_BptxAND (bit 321)
- L1_FirstCollisionInOrbit_Centrality30_100_BptxAND (bit 322)


**Baseline HI menu:** The menu content is same as previous version. [L1Menu_CollisionsHeavyIons2022_v1_0_0](https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2022_v1_0_0/L1Menu_CollisionsHeavyIons2022_v1_0_0.xml) 
The menu contains same algos as L1Menu_CollisionsHeavyIons2022_v1_0_0 with updated cabling name from "L1ExternalConditionsCabling_20220830" to "L1ExternalConditionsCabling_20221005". [CMSLITDPG-1015](https://its.cern.ch/jira/browse/CMSLITDPG-1015)

The new cabling contains following changes to External Conditions:
- on channel 36: ZDCnM_0 (bit 0 of encoded ZDC triggers - ZDC M part)
- on channel 37: ZDCnM_1 (bit 1 of encoded ZDC triggers - ZDC M part)
- on channel 38: ZDCnP_0 (bit 0 of encoded ZDC triggers - ZDC P part)
- on channel 39: ZDCnP_1 (bit 1 of encoded ZDC triggers - ZDC P part)
- Removed obsolete CASTOR definitions

**Reference JIRA:** The change in external conditions by uGT team in correspondence to ZDC configuration is documented in the JIRA. [CMSLITDPG-1015](https://its.cern.ch/jira/browse/CMSLITDPG-1015).
