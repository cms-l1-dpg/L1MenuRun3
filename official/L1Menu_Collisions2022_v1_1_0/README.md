# L1Menu_Collisions2022_v1_1_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/cms-l1-dpg/L1MenuRun3/master/development/L1Menu_Collisions2022_v1_1_0/L1Menu_Collisions2022_v1_1_0.html)

**Comment:** New version of the menu for Run3 with the following additional seeds:

- 3 new monitoring seeds for muon triggers [https://its.cern.ch/jira/browse/CMSLITDPG-990]
	- L1_SingleMu22_OQ (bit 19)
	- L1_SingleMu22_DQ (bit 20)
	- L1_DoubleMu0_Upt5_Upt5 (bit 48)
- 1 new prefiring monitoring seed [ https://its.cern.ch/jira/browse/CMSLITDPG-991]
	- L1_MinimumBiasHF0 (bit 462)

In order to accomodate the new seeds preserving the order, the following seeds have been moved:

- 19-23 -> 21-25
- 25-33 -> 26-34
- 36-48 -> 35-47

For grouping the LLP seeds together, the following changes took place:
- 339 -> 383
- 384-387 -> 388-391
- 388-391 -> 384-387

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.

**Additional Remarks:**

- Refernce JIRA ticket: [https://its.cern.ch/jira/browse/CMSLITDPG-980]
- Synthesized and tested in uGT test crate
- Tag in condDB uploaded: [L1Menu_Collisions2022_v1_1_0_xml](https://cms-conddb.cern.ch/cmsDbBrowser/search/Prod/L1Menu_Collisions2022_v1_1_0_xml)
- GT request done [https://cms-talk.web.cern.ch/t/run-3-gt-update-of-the-l1-menu-tag-v1-1-0-in-run-3-mc-gts-and-run-3-data-relvals-gts/11279]
- The L1Menu_Collisions2022_v1_1_0 was deployed online on 2nd June, 2022 during run 352795 and fill 7689.

