# Official Menus

Collection of L1 menus released during MWGRs or for data taking.

**NOTE**: 
- The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.

- The following L1 seeds based on NoBptxOR requirement are instead used for Physics purposes and thus they have to be enabled for the online data taking. The corresponding prescale values have been agreed for the start of the Run 3 data taking, and updated during the data-taking (see details in [CMSLITDPG-1001](https://its.cern.ch/jira/browse/CMSLITDPG-1001)):
```
- L1_SingleMuOpen_NotBptxOR (PS=250)
- L1_SingleMuOpen_er1p4_NotBptxOR_3BX (PS=1)
- L1_SingleMuOpen_er1p1_NotBptxOR_3BX (PS=1)
- L1_SingleJet20er2p5_NotBptxOR (PS=100)
- L1_SingleJet20er2p5_NotBptxOR_3BX (PS=0)
- L1_SingleJet43er2p5_NotBptxOR_3BX (PS=1)
- L1_SingleJet46er2p5_NotBptxOR_3BX (PS=1)
```
