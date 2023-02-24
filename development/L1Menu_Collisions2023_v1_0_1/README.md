# L1Menu_Collisions2023_v1_0_1

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_0_1/L1Menu_Collisions2023_v1_0_1.html)

**Comment:** 
Second (temporary) version of the L1 menu for the 2023 data taking. 

## Changes from first 2023 menu ("L1Menu_Collisions2023_v1_0_0")
      
### Seeds for Bsmumu ([CMSLITDPG-1098](https://its.cern.ch/jira/browse/CMSLITDPG-1098))      
   - Added five new seeds for 2023:
      - `L1_DoubleMu0er1p4_SQ_OS_dEta_Max1p2` (bit 507)
      - `L1_DoubleMu4er2p0_SQ_OS_dR_Max1p6` (bit 508)
      - `L1_DoubleMu5_SQ_OS_dR_Max1p6` (bit 509)
      - `L1_DoubleMu3er2p0_SQ_OS_dR_Max1p6` (bit 510)
      - `L1_DoubleMu0er1p5_SQ_OS_dEta_Max1p2` (bit 511)


<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
