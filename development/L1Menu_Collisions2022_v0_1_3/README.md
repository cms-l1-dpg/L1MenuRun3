# L1Menu_Collisions2022_v0_1_3

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/priyasajid/L1MenuRun3/blob/master/development/L1Menu_Collisions2022_v0_1_3/L1Menu_Collisions2022_v0_1_3.html)

**Comment:** Menu for Run3 adding 3 new Tau seeds, two with overlap removal and one with increased threshold of an existing double tau seed. [Scale set reference, for grammar version 0.10]

- new L1 Double Tau + Jet seed & increasing threshold of old Double tau seed [https://its.cern.ch/jira/browse/CMSLITDPG-961]:
    - L1_DoubleIsoTau26er2p1_Jet55_OvRm_dR0p5
    - L1_DoubleIsoTau35er2p1 (increased threshold from previous seed L1_DoubleIsoTau32er2p1)

- new Double Jet + One Tau seed [https://its.cern.ch/jira/browse/CMSLITDPG-962]:
    - L1_DoubleJet35_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5

**NOTE:** The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
