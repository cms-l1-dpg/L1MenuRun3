# L1Menu_CollisionsPPRef2024_v1_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsPPRef2024_v1_0_0/L1Menu_CollisionsPPRef2024_v1_0_0.html)

**Comment:** 
Final version of the L1 menu for the 2024 ppRef collisions.
This menu has been created by using the last version of TME `0.17.1`, grammar `0.13` and updated scales to `scales_2023_02_16`.
The menu development for the ppRef run is documented in [CMSLITDPG-1207](https://its.cern.ch/jira/browse/CMSLITDPG-1207).

<br/>

The following changes, from the last version of the 2024 ppRef menu (`L1Menu_CollisionsPPRef2024_v0_0_2`), have been made:

### Addition of new seeds for monitoring purposes (not meant to be used at HLT)
   - Added 51 "uncorrected jets" seeds (using the TAU channel):
      - `L1_SingleUncorrJet2/4/6/8/12/16/20/24/28`
      - `L1_DoubleUncorrJet2/4/6/8/12/16_dPhi2p0`  
      - `L1_SingleUncorrJet2/4/6/8/12/16/20/24/28_ZDC1nOR`
      - `L1_SingleUncorrJet2/4/6/8/12/16/20/24/28_ZDC1nOR_Bkp1`
      - `L1_SingleUncorrJet2/4/6/8/12/16/20/24/28_ZDC1nOR_Bkp2`      
      - `L1_SingleUncorrJet2/4/6/8/12/16/20/24/28_ZDC1n_AsymXOR`
   - Added 6 ZDC seeds    
      - `L1_ZDCP8/10/12`
      - `L1_ZDCM8/10/12`
   - Added 2 seeds for DQM:
      - `L1_FirstBunchInTrain_50ns`
      - `L1_LastBunchInTrain_50ns`

