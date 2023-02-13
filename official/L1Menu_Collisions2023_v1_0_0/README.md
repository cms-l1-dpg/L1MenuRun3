# L1Menu_Collisions2023_v1_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/official/L1Menu_Collisions2023_v1_0_0/L1Menu_Collisions2023_v1_0_0.html)

**Comment:** 
First version of the L1 menu for the 2023 data taking. It will be used as a starting point for the developments and updates of the L1 menu targeting the first round of integration (March 8th).

<br/>

The following changes, from the last menu of 2022 ("L1Menu_Collisions2022_v1_4_0"), have been done:

#### Seeds for the Tau3mu search ([CMSLITDPG-960](https://its.cern.ch/jira/browse/CMSLITDPG-960))
   - Removed the seeds included in 2022: 
      - L1_TripleMu_2SQ_1p5SQ_0OQ (bit 74) 
      - L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12 (bit 82)
      - L1_TripleMu_3SQ_2p5SQ_0OQ_Mass_Max12 (bit 83)
   - Added two new seeds for 2023:
      - L1_TripleMu_3SQ_2p5SQ_0_OS_Mass_Max12 (bit 82) 
      - L1_TripleMu_4SQ_2p5SQ_0OQ_OS_Mass_Max12 (bit 83) 


<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
