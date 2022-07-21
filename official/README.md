# Official Menus

Collection of L1 menus released during MWGRs or for data taking.

**NOTE**: 
- The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.

- The following L1 seeds based on NoBptxOR requirement are instead used for Physics purposes (details in JIRA: https://its.cern.ch/jira/browse/CMSLITDPG-1001) and thus they have to be enabled for the online data taking.
```
LIST of NoBptxOR based seeds needed for physics, with the ps value used during 2018 data taking:
- L1_SingleMuOpen_NotBptxOR (ps=4000)
- L1_SingleMuOpen_er1p4_NotBptxOR_3BX (ps=1)
- L1_SingleMuOpen_er1p1_NotBptxOR_3BX (ps=1)
- L1_SingleJet20er2p5_NotBptxOR (ps=4000)
- L1_SingleJet20er2p5_NotBptxOR_3BX (ps=0)
- L1_SingleJet43er2p5_NotBptxOR_3BX (ps=1)
- L1_SingleJet46er2p5_NotBptxOR_3BX (ps=1)
```
