# L1Menu_Collisions2023_v1_3_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_3_0/L1Menu_Collisions2023_v1_3_0.html)

**Comment:** 
New version of the L1 menu for the 2023 physics data taking, targeting the fourth HLT menu of 2023.
This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The following changes, from the last menu of 2023 (`L1Menu_Collisions2023_v1_2_0`), have been made:

### New seeds for barrel jets monitoring [CMSLITDPG-1171](https://its.cern.ch/jira/browse/CMSLITDPG-1171)
   - Added 2 new seeds:
      - `L1_SingleJet35er1p3` (bit 311)
      - `L1_SingleJet120er1p3` (bit 314)

### Removal of unused seeds [CMSHLT-2854](https://its.cern.ch/jira/browse/CMSHLT-2854) ([CMSLITDPG-1155](https://its.cern.ch/jira/browse/CMSLITDPG-1151)), [CMSHLT-2858](https://its.cern.ch/jira/browse/CMSHLT-2858)
   - Removed the following 10 seeds
      - `L1_DoubleEG8er2p5_HTT260er`
      - `L1_DoubleEG8er2p5_HTT340er`
      - `L1_Mu22er2p1_IsoTau28er2p1`
      - `L1_Mu22er2p1_IsoTau36er2p1`
      - `L1_DoubleJet30er2p5_Mass_Min360_dEta_Max1p5`
      - `L1_DoubleJet_115_40_DoubleJet40_Mass_Min620_Jet60TT28`
      - `L1_DoubleJet_120_45_DoubleJet45_Mass_Min620_Jet60TT28`
      - `L1_DoubleJet35_Mass_Min450_IsoTau45_RmOvlp`
      - `L1_DoubleJet_80_30_Mass_Min420_IsoTau40_RmOvlp`
      - `L1_DoubleJet_80_30_Mass_Min420_Mu8`

<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
