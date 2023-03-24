# L1Menu_Collisions2023_v1_0_1

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_0_1/L1Menu_Collisions2023_v1_0_1.html)

**Comment:** 
New version of 2023 L1 menu, created in updated version of TME `0.15` and grammar `0.11`.

<br/>

The following seeds have been modified with an updated (more compact) logic expression: 
   - `L1_DoubleMu0_Upt5_Upt5`	(bit 51)
   - `L1_DoubleMu0_Upt6_IP_Min1_Upt4` (bit 52)
   - `L1_DoubleMu0_Upt15_Upt7` (bit 53)


<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
