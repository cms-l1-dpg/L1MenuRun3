# Prescale tables for L1Menu_Collisions2023_v1_0_1
%
**Description of the csv PS table** 

At the current stage, the main configuration for the **column 2.00E34** considers as baseline:
* core 2022 L1 Menu
* plus Option 3 new Bsmumu seeds
* plus new Tau3Mu seed
* plus DoubleEG11 seed for B Parking
* plus `L1_HTT280er` (DiHiggs Parking)
* plus W3pi seed `L1_DoubleIsoTau32_Mass_Max80`
* plus central dijet seed with inv. mass cut `L1_DoubleJet30er2p5_Mass_Min250_dEta_Max1p5`


**NOTE** : The following definitions for the backup columns (2p1e34, 2p2e34, 2p3e34) has been adopted:
* 2p1e34: same as 2p0e34, but without `L1_DoubleIsoTau32_Mass_Max80` and `L1_DoubleJet30er2p5_Mass_Min250_dEta_Max1p5`.
* 2p2e34: same as 2p1e34 but changed ps of Diele Bparking seed `L1_DoubleEG11_er1p2_dR_Max0p6` from 1 to 2.
* 2p3e34: same as 2p2e34
