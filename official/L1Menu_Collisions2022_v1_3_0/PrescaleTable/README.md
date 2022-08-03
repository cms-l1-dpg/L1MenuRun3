# Prescale tables for the L1Menu_Collisions2022_v1_3_0

### Important REMARK
These PS tables are NOT fully aligned with the ones used online. They're still used for _development_ purposes.

<br/>

<h2 align="center">
Description of the different PS Tables
</h2>
<br/>


## L1Menu_Collisions2022_v1_3_0-13.6TeV_2748b
**Draft of the PS table** to be used during stable collisions at 13.6 TeV when the number of bunches reaches the nominal value, i.e. 2748. 
<br/>
Few notes:
- The full L1 menu is enabled at the lowest luminosity as is happening online during the ramp up. The lowest thresholds for the B-Parking seeds are also enabled (starting from *L1_DoubleEG4p5_er1p2_dR_Max0p9*). Note that few changes have been done for the PS value of ZB-Bptx seeds in order to test the table using MenuTools. (Changes to be reverted for the final version!)
    - L1_IsolatedBunch (bit 471): ps = 110 (previously it was 2239)
    - L1_FirstCollisionInOrbit (bit 480): ps = 1103 (previously it was 563)
    - L1_CDC_SingleMu_3_er1p2_TOP120_DPHI2p618_3p142 (bit 494): ps = 6 (previously it was 190);
- The following seeds have been deactivated ([CMSHLT-2295](https://its.cern.ch/jira/browse/CMSHLT-2295)):
    - L1_SingleLooseIsoEG26er1p5 (bit 176)
    - L1_SingleLooseIsoEG28er2p5 (bit 178)
    - L1_SingleLooseIsoEG28er2p1 (bit 179)
    - L1_SingleLooseIsoEG30er2p5 (bit 181)
    - L1_SingleIsoEG28er2p5 (bit 189)
    - L1_SingleIsoEG28er2p1 (bit 190)
    - L1_LooseIsoEG26er2p1_HTT100er (bit 242)    
    - For DoubleEG seeds for BParking, the last prescale scheme reported in its [CMSLITDPG-957](https://its.cern.ch/jira/browse/CMSLITDPG-957) has been adopted.
    - The seed *L1_SingleIsoEG28er1p5* has been prescaled by a factor 25 for all lumi columns, as reported in [CMSHLT-2398](https://its.cern.ch/jira/browse/CMSHLT-2398) ;
    - The lumi column 2.0E34 is now a copy of 1.7E34 with low B parking seeds deactivated (starting from *L1_DoubleEG4p5_er1p2_dR_Max0p9*).
- Tighter scenario considered in lumi column 2.2E34:
    - The main L1 seed for Tau3mu search (*L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12* (bit 82)) has been switched off, leaving only the backup seed (*L1_TripleMu_3SQ_2p5SQ_0OQ_Mass_Max12* (bit 83)) active;
    - The seeds *L1_DoubleIsoTau32er2p1* (bit 270) and *L1_DoubleIsoTau34er2p1* (bit 271) have been deactivated, while the seed *L1_DoubleIsoTau35er2p1* (bit 272) has been activated for the same lumi columns.
<br/> 
    
<h2 align="center">
Description of the different formats
</h2>
<br/>   

- The PS table in **csv format** is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
- The PS table in **xlsx format** is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).
