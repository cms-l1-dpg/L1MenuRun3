# L1Menu_Collisions2022_v1_2_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2022_v1_2_0/L1Menu_Collisions2022_v1_2_0.html)

**Comment:** 
New version of the menu for Run3 with 5 additional seeds [CMSLITDPG-995](https://its.cern.ch/jira/browse/CMSLITDPG-995):
   - `L1_ETMHF70` (bit 418) with PS = 0
   - `L1_ETMHF80` (bit 419) with PS = 1
   - `L1_ETMHF90` (bit 420) with PS = 1
   - `L1_ETMHF70_HTT60er` (bit 427) with PS = 0
   - `L1_ETMHF80_HTT60er` (bit 428) with PS = 1

In order to accomodate the new seeds preserving the order, the following seeds have been moved:
   - 428-432 -> 429-433
<br/>

#### Few differences w.r.t. default PS table of menu v1_1_0 (implemented starting from the v1_2_0 menu):
- `L1_SingleLooseIsoEG26er1p5` (bit 176) enabled (as it was at the end of 2018)
- `L1_DoubleMu0er1p5_SQ_dR_Max1p4` (bit 59) with PS=50 (instead of 2)
- `L1_DoubleMu18er2p1_SQ` (bit 47) enabled -> [CMSHLT-2413](https://its.cern.ch/jira/browse/CMSHLT-2413). It was disabled by mistake after the seed renaming ([CMSHLT-2258](https://its.cern.ch/jira/browse/CMSHLT-2258)).
- `L1_SingleMu12er1p5` (bit 31) enabled and prescaled to 4 for all lumi scenarios from 1.7E34 and below. [CMSLITDPG-997](https://its.cern.ch/jira/browse/CMSLITDPG-997)
   
#### Few differences w.r.t. PS table used during 2018 data-taking:
- `L1_IsoEG32er2p5_Mt40` seed is now disabled (as requested in [CMSHLT-2249](https://its.cern.ch/jira/browse/CMSHLT-2249)). <br/>
  It needs to be switch on only if the seed `L1_SingleIsoEG32er2p5` will be prescaled. 
   
<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
