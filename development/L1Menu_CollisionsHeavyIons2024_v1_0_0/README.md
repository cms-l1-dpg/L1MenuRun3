# L1Menu_CollisionsHeavyIons2024_v1_0_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_CollisionsHeavyIons2024_v1_0_0/L1Menu_CollisionsHeavyIons2024_v1_0_0.html)

**Comment:** 
New version of the L1 menu for the 2024 HeavyIons collisions.
This menu has been created by using the last version of TME `0.17.1`, grammar `0.13` and updated scales to `scales_2023_02_16`.
The menu development for the Heavy Ions runs is documented in [CMSLITDPG-1314](https://its.cern.ch/jira/browse/CMSLITDPG-1314).

<br/>

The following changes, from the last HI menu (`L1Menu_CollisionsHeavyIons2024_v0_0_0`), have been made:

   - Changed the name of 75 existing seeds using uncorrected jets: from “UPCJet” to “UncorrJet”

   - Added 31 seeds:
      - 1 muon seed
      - 2 seeds for DQM (`L1_First/LastBunchInTrain_50ns`)
      - Additional jet ET thresholds for UncorrJet seeds
      - ZDC backup seeds for UncorrJets
      - 10 seeds as for a L1 rapidity gap ("OneSideGap"), currently using ASYMETHF as placeholder
    
   - Removed 41 seeds:
      - `L1_SingleJet8/12/16/20/24/28_ZDC1n_Bkp1/2/3_AsymXOR/XOR_BptxAND`
      - `L1_ZDC1n_Bkp2/3_OR_BptxAND`
      - `L1_SingleEG2_ZDC1n_Bkp1/2/3_OR_NotMinimumBiasHF2_AND_BptxAND`