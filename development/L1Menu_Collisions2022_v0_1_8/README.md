# L1Menu_Collisions2022_v0_1_8

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/caruta/L1MenuRun3/blob/patch-1/preliminary/L1Menu_Collisions2022_v0_1_8/L1Menu_Collisions2022_v0_1_8.html)

**Comment:** 
New version of the menu for Run3. 
Adding three new seeds for B-Parking and renaming/shifting in position of some already present seeds (list of modification in https://docs.google.com/spreadsheets/d/1WKz3Nl0gIOeoM03cUgKJwZ5rOQ4LS_lyGjZM_5AFCj4/edit#gid=1571902755 ).

- new L1 Double EG seeds for B-parking [https://its.cern.ch/jira/browse/CMSLITDPG-957]:
    - L1_DoubleEG4_er1p2_dR_Max0p9 (bit n.200)
    - L1_DoubleEG4p5_er1p2_dR_Max0p9 (bit n.201)
    - L1_DoubleEG11_er1p2_dR_Max0p6 (bit n.214)

- Seeds to be deleted (copies with wrong name): 34, 35, 36, 93, 94, 114, 115, 116, 117, 281, 299, 368, 369, 370, 371, 391, 392, 493, 495, 496, 497, 498, 499, 502, 507, 508, 509, 510, 511.

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.

**Additional Remarks:**

- Tag in condDB uploaded: [L1Menu_Collisions2022_v0_1_8_xml](https://cms-conddb.cern.ch/cmsDbBrowser/search/Prod/L1Menu_Collisions2022_v0_1_8_xml)
- GT request done [https://cms-talk.web.cern.ch/t/mc-run3-gt-update-of-the-l1-menu-tag-v0-1-8-in-run-3-mc-gts/8579]
