# Prescale tables for L1Menu_Collisions2023_v1_1_0

**Description of the csv PS table** 

At the current stage, the main configuration for the **column 2.00E34** considers as baseline:
* core 2022 L1 Menu
* plus Option 3 new Bsmumu seeds
* plus new Tau3Mu seed
* plus `L1_DoubleEG11_er1p2_dR_Max0p6` seed for B Parking
* plus `L1_HTT280er` and `L1_HTT280er_QuadJet_70_55_40_35_er2p5` (DiHiggs Parking)
* plus W3pi seed `L1_DoubleIsoTau32_Mass_Max80`
* plus central dijet seed with inv. mass cut `L1_DoubleJet30er2p5_Mass_Min250_dEta_Max1p5` (included in Scouting) 

**NOTE** : The following definitions for the backup columns (2p1e34, 2p2e34, 2p3e34) has been adopted:
* **2p1e34**: same as 2p0e34, but without 
  * `L1_DoubleJet_90_30_DoubleJet30_Mass_Min620`, 
  * `L1_DoubleIsoTau32er2p1_Mass_Max80`, 
  * `L1_DoubleJet30er2p5_Mass_Min250_dEta_Max1p5`, and 
  * change in ps of `L1_DoubleEG11_er1p2_dR_Max0p6` (from 1 to 2)
* **2p2e34**: same as 2p1e34 but without 
  * `L1_DoubleIsoTau26er2p1_Jet55_RmOvlp_dR0p5`, 
  * `L1_HTT280er`, 
  * `L1_HTT280er_QuadJet_70_55_40_35_er2p5`
* **2p3e34**: same as 2p2e34 but without 
  * `L1_DoubleMu4er2p0_SQ_OS_dR_Max1p6`, 
  * `L1_DoubleMu3er2p0_SQ_OS_dR_Max1p6`, 
  * `L1_TripleMu_3SQ_2p5SQ_0_OS_Mass_Max12`



* Other references:
  * [CMSHLT-2785](https://its.cern.ch/jira/browse/CMSHLT-2785) for backup columns definitions
  * [CMSLITDPG-110](5https://its.cern.ch/jira/browse/CMSLITDPG-1105) for a summary of the 2023 prescale changes
