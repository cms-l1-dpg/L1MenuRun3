# L1Menu_Collisions2022_v1_3_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2022_v1_3_0/L1Menu_Collisions2022_v1_3_0.html)

**Comment:** 
New version of the menu for Run3 with 7 additional seeds with low MET thresholds [CMSLITDPG-995](https://its.cern.ch/jira/browse/CMSLITDPG-995):
   - `L1_Mu3er1p5_Jet100er2p5_ETMHF30` (bit 127) 
   - `L1_DoubleMu3_SQ_ETMHF30_HTT60er` (bit 141) 
   - `L1_DoubleMu3_SQ_ETMHF40_HTT60er` (bit 142) 
   - `L1_DoubleMu3_SQ_ETMHF30_Jet60er2p5_OR_DoubleJet40er2p5` (bit 144) 
   - `L1_DoubleMu3_SQ_ETMHF40_Jet60er2p5_OR_DoubleJet40er2p5` (bit 145) 
   - `L1_ETMHF80_SingleJet55er2p5_dPhi_Min2p1`  (bit 334) 
   - `L1_ETMHF80_SingleJet55er2p5_dPhi_Min2p6`  (bit 335) 

In order to accomodate the new seeds preserving the order, the following seeds have been moved:
   - 142,143 -> 138,139
   - 145 -> 143
   - 329-334 -> 328-333
   - 335-338 -> 336-339
   
**NOTE**: The ps value for the already present seed `L1_DoubleMu3_SQ_ETMHF50_HTT60er` was changed from 0 to 1.
<br/>
<br/>

#### Few differences w.r.t. L1Menu_Collisions2022_v1_2_0-13.6TeV_2748b PS table (implemented starting from v1_3_0 menu): 
- `L1_SingleIsoEG28er1p5` (bit 91) prescaled to 25 in all lumi scenarios ([CMSLITDPG-996](https://its.cern.ch/jira/browse/CMSLITDPG-996))
- Copied 2.0E+34 column in 2.2E+34, and 2.0E+34 is a copy of 1.7E34 lumi column, with B Parking seeds (DoubleEG, bits: 200 - 212) disabled
- Increased the ps value for L1_SingleMu7 seed ([JIRA](https://its.cern.ch/jira/browse/CMSLITDPG-992?focusedCommentId=4469684&page=com.atlassian.jira.plugin.system.issuetabpanels%3Acomment-tabpanel#comment-4469684)).

#### Few differences w.r.t. default PS table of menu v1_1_0 (implemented starting from the v1_2_0 menu):
- `L1_SingleLooseIsoEG26er1p5` (bit 176) enabled (as it was at the end of 2018)
- `L1_DoubleMu0er1p5_SQ_dR_Max1p4` (bit 59) with PS=50 (instead of 2)
- `L1_DoubleMu18er2p1_SQ` (bit 47) enabled -> [CMSHLT-2413](https://its.cern.ch/jira/browse/CMSHLT-2413). It was disabled by mistake after the seed renaming ([CMSHLT-2258](https://its.cern.ch/jira/browse/CMSHLT-2258)).
- `L1_SingleMu12er1p5` (bit 31) enabled and prescaled to 4 for all lumi scenarios from 1.7E34 and below ([CMSLITDPG-997](https://its.cern.ch/jira/browse/CMSLITDPG-997))

#### Few differences w.r.t. PS table used during 2018 data-taking:
- `L1_IsoEG32er2p5_Mt40` seed is now disabled (as discussed in [CMSHLT-2249](https://its.cern.ch/jira/browse/CMSHLT-2249)). <br/>
  Note that it is kept in the menu as backup and it has to be switch on in case `L1_SingleIsoEG32er2p5` will be disabled. 
   
<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.


**Additional Remarks:**

- Reference JIRA ticket: [CMSLITDPG-980](https://its.cern.ch/jira/browse/CMSLITDPG-980)
- Synthesized and tested in uGT test crate
- Tag in condDB uploaded: [L1Menu_Collisions2022_v1_3_0-d1_xml](https://cms-conddb.cern.ch/cmsDbBrowser/list/Prod/tags/L1Menu_Collisions2022_v1_3_0-d1_xml)
- The L1Menu_Collisions2022_v1_3_0 was deployed online on 10th August, 2022 during run [357150](https://cmsoms.cern.ch/cms/runs/report?cms_run=357150&cms_run_sequence=GLOBAL-RUN).

