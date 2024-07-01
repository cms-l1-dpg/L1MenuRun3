# L1Menu_Collisions2024_v1_3_0

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2024_v1_3_0/L1Menu_Collisions2024_v1_3_0.html)

**Comment:** 
Fourth L1T menu for the 2024 pp data taking, with the updated UTM grammar (`0.13.0`).
This menu has been created by using the last version of TME `0.17.1`, grammar `0.13.0` and `scales_2024_05_15`.

<br/>

The following changes, from the third menu of 2024 (`L1Menu_Collisions2024_v1_2_0`), have been made:

### Added new muon monitoring seeds split per TF and endcap [CMSL1TDPG-1298](https://its.cern.ch/jira/browse/CMSLITDPG-1298)
   - Added the following seeds: 
      - `L1_SingleMu22_BMTF_POS` (bit 37)
      - `L1_SingleMu22_BMTF_NEG` (bit 38)
      - `L1_SingleMu22_OMTF_POS` (bit 39)
      - `L1_SingleMu22_OMTF_NEG` (bit 40)
      - `L1_SingleMu22_EMTF_POS` (bit 41)
      - `L1_SingleMu22_EMTF_NEG` (bit 42)

### Added new MHTHF seeds and removed MHT ones [CMSL1TDPG-1229](https://its.cern.ch/jira/browse/CMSLITDPG-1229)
   - Added the following seeds: 
      - `L1_HTMHF100` (bit 434)
      - `L1_HTMHF120` (bit 435)
      - `L1_HTMHF125` (bit 436)
      - `L1_HTMHF130` (bit 437)
      - `L1_HTMHF150` (bit 438)
   - Removed the following seeds: 
      - `L1_MHT120`
      - `L1_MHT150`
      - `L1_MHT200`

### Added new CICADA seeds [CMSL1TDPG-1295](https://its.cern.ch/jira/browse/CMSLITDPG-1295)
   - Added the following seeds: 
      - `L1_CICADA_VLoose` (bit 445)
      - `L1_CICADA_Loose`  (bit 446)
      - `L1_CICADA_Medium` (bit 447)
      - `L1_CICADA_Tight`  (bit 448)
      - `L1_CICADA_VTight` (bit 449)

### Modified the AXOL1TL seeds to include the new NN model (v4) together with updated thresholds [CMSL1TDPG-1296](https://its.cern.ch/jira/browse/CMSLITDPG-1296)
   - Modified the following seeds: 
      - `L1_AXO_VLoose`  (bit 439)
      - `L1_AXO_Loose`   (bit 440)
      - `L1_AXO_Nominal` (bit 441)
      - `L1_AXO_Tight`   (bit 442)
      - `L1_AXO_VTight`  (bit 443)

### Fixed the definition of the `MU-ETA_EMTF_NEG_er2p0` cut for the following displaced double muon seeds (not enabled, just to prevent fw/emu mismatches)
   - Issue spotted and reported [here](https://its.cern.ch/jira/browse/CMSLITDPG-1221?focusedId=6413729&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel#comment-6413729)
      - `L1_DoubleMu6_Upt6_SQ_er2p`
      - `L1_DoubleMu7_Upt7_SQ_er2p`
      - `L1_DoubleMu8_Upt8_SQ_er2p`
