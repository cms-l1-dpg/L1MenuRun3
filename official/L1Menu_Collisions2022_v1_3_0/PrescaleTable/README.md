# Prescale tables for the L1Menu_Collisions2022_v1_3_0

<h2 align="center">
Description of the different PS Tables
</h2>
<br/>


## L1Menu_Collisions2022_v1_3_0-13.6TeV
**Draft of the PS table** to be used during stable collisions at 13.6 TeV. 
<br/>
Few notes:
- The full L1 menu is enabled at the lowest luminosity as is happening online during the ramp up. The lowest thresholds for the B-Parking seeds are also enabled (starting from *L1_DoubleEG4p5_er1p2_dR_Max0p9*). Note that few changes have been done for the PS value of ZB-Bptx seeds in order to test the table using MenuTools. (Changes to be reverted for the final version!)
    - L1_IsolatedBunch (bit 471): ps = 1 (previously it was 2239)
    - L1_FirstCollisionInOrbit (bit 480): ps = 563 (previously it was 563)
    - L1_CDC_SingleMu_3_er1p2_TOP120_DPHI2p618_3p142 (bit 494): ps = 3 (previously it was 190);
- The following seeds have been deactivated ([CMSHLT-2295](https://its.cern.ch/jira/browse/CMSHLT-2295)):
    - L1_SingleLooseIsoEG26er1p5 (bit 176)
    - L1_SingleLooseIsoEG28er2p5 (bit 178)
    - L1_SingleLooseIsoEG28er2p1 (bit 179)
    - L1_SingleLooseIsoEG30er2p5 (bit 181)
    - L1_SingleIsoEG28er2p5 (bit 189)
    - L1_SingleIsoEG28er2p1 (bit 190)
    - L1_LooseIsoEG26er2p1_HTT100er (bit 242)    
    - For DoubleEG seeds for BParking, the last prescale scheme reported in its [CMSLITDPG-957](https://its.cern.ch/jira/browse/CMSLITDPG-957) has been adopted. In the tightest scenario (lumi column 2.2e34) only the highest pt threshold seed *L1_DoubleEG11_er1p2_dR_Max0p6* (bit 213) is kept on.
    - The seed *L1_SingleIsoEG28er1p5* (bit 191) has been prescaled by a factor 25 for all lumi columns, as reported in [CMSHLT-2398](https://its.cern.ch/jira/browse/CMSHLT-2398) ;
    - The lumi column 2.0E34 is now a copy of 1.7E34 with low B parking seeds deactivated (starting from *L1_DoubleEG4p5_er1p2_dR_Max0p9*).

Last modifications in view of the 2400 colliding bunches scenario:
- Seed switched off in lumi column 2.1E34 and 2.2E34:
    - New L1 seeds for Bmumu search (*L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p6* (bit 55) and *L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p5* (bit 56)) 
    - New L1 seeds for Tau3mu search (*L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12* (bit 82) and *L1_TripleMu_3SQ_2p5SQ_0OQ_Mass_Max12* (bit 83)) 
<br/> 

## L1Menu_Collisions2022_v1_3_0-13.6TeV (in development)
Additional lumi column 2.3e34, which is a copy of column 2.2E34, but with the following seeds disabled:
- *L1_DoubleIsoTau32* (bit 270) and *L1_DoubleIsoTau34* (bit 271) -> next enabled seed: *L1_DoubleIsoTau35* (bit 272)
- *L1_LooseIsoEG28er2p1_Jet34er2p5_dR_Min0p3* (bit 239) -> next enabled seed: *L1_LooseIsoE308er2p1_Jet34er2p5_dR_Min0p3* (bit 240)
<br/>   

<h2 align="center">
Description of the different formats
</h2>
<br/>   

- The PS table in **csv format** is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
- The PS table in **xlsx format** is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).
