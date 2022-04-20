# L1Menu_Collisions2022_v1_0_1

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/caruta/L1MenuRun3/blob/patch-1/development/L1Menu_Collisions2022_v1_0_1/L1Menu_Collisions2022_v1_0_1.html)

**Comment:** 
New version of the menu for Run3 with 3 additional seeds [JIRA:  https://its.cern.ch/jira/browse/CMSLITDPG-961]:
- L1_DoubleIsoTau26er2p1_Jet70_RmOvlp_dR0p5 (bit 284)
- L1_Mu18er2p1_Tau26er2p1_Jet55 (bit 281)
- L1_Mu18er2p1_Tau26er2p1_Jet70 (bit 282)

In order to accomodate the new seeds preserving the order, the following seeds have been moved:
- 278 -> 283
- 282-287 -> 285-291

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
