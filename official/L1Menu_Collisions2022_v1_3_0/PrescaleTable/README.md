# Prescale tables for the L1Menu_Collisions2022_v1_3_0

<h2 align="center">
Description of the different PS Tables
</h2>
<br/>


## L1Menu_Collisions2022_v1_3_0-13.6TeV
**Draft of the PS table** to be used during stable collisions at 13.6 TeV. 
<br/>
Few notes:
- The full L1 menu is enabled at the lowest luminosity as is happening online during the ramp up. The lowest thresholds for the B-Parking seeds are also enabled (starting from `L1_DoubleEG4p5_er1p2_dR_Max0p9`). Note that few changes have been done for the PS value of ZB-Bptx seeds in order to test the table using MenuTools. (Changes to be reverted for the final version!)
    - `L1_IsolatedBunch` (bit 471): ps = 1 (previously it was 2239)
    - `L1_FirstCollisionInOrbit` (bit 480): ps = 563 (previously it was 563)
    - `L1_CDC_SingleMu_3_er1p2_TOP120_DPHI2p618_3p142` (bit 494): ps = 3 (previously it was 190);
- The following seeds have been deactivated ([CMSHLT-2295](https://its.cern.ch/jira/browse/CMSHLT-2295)):
    - `L1_SingleLooseIsoEG26er1p5` (bit 176)
    - `L1_SingleLooseIsoEG28er2p5` (bit 178)
    - `L1_SingleLooseIsoEG28er2p1` (bit 179)
    - `L1_SingleLooseIsoEG30er2p5` (bit 181)
    - `L1_SingleIsoEG28er2p5` (bit 189)
    - `L1_SingleIsoEG28er2p1` (bit 190)
    - `L1_LooseIsoEG26er2p1_HTT100er` (bit 242)    
    - For DoubleEG seeds for BParking, the last prescale scheme reported in its [CMSLITDPG-957](https://its.cern.ch/jira/browse/CMSLITDPG-957) has been adopted. In the tightest scenario (lumi column 2.2e34) only the highest pt threshold seed `L1_DoubleEG11_er1p2_dR_Max0p6` (bit 213) is kept on.
    - The seed `L1_SingleIsoEG28er1p5` (bit 191) has been prescaled by a factor 25 for all lumi columns, as reported in [CMSHLT-2398](https://its.cern.ch/jira/browse/CMSHLT-2398) ;
    - The lumi column 2.0E34 is now a copy of 1.7E34 with low B parking seeds deactivated (starting from `L1_DoubleEG4p5_er1p2_dR_Max0p9`).

### Updated backup columns situation [CMSLITDPG-1019](https://its.cern.ch/jira/browse/CMSLITDPG-1019):
- Seed switched off in lumi column 2.1E34 (w.r.t. 2.0E34):
    - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min620`
    - `L1_DoubleJet_115_40_DoubleJet40_Mass_Min620`
    - `L1_ETMHF90`
    - `L1_ETMHF90_HTT60er`
- Seed switched off in lumi column 2.2E34 (w.r.t. 2.1E34):
    - `L1_DoubleMu0er2p0_SQ_dEta_Max1p6`
    - `L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p6`
    - `L1_DoubleIsoTau26er2p1_Jet55_RmOvlp_dR0p5`
<br/> 

### Modifications (21st Oct 2022):
- seeds deactivated in all columns:
    - `L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12` (bit 82): deactivated due to an observed increase in its rate after the TS1 &rarr; [CMSLITDPG-960](https://its.cern.ch/jira/browse/CMSLITDPG-960). Its backup seed is still active.
    - `L1_SingleIsoTau32er2p1` (bit 262): deactivated because not used by any HLT path.
- seeds deactivated (in all columns) to ensure safe deployment of new HCAL calibrations [CMSLITDPG-1021](https://its.cern.ch/jira/browse/CMSLITDPG-1021):
    - `L1_ETMHF80` &rarr; `L1_ETMHF90` 
    - `L1_ETMHF80_HTT60er` &rarr; `L1_ETMHF90_HTT60er`
    - `L1_ETMHF80_SingleJet55er2p5_dPhi_Min2p1` &rarr; `L1_ETMHF90_SingleJet55er2p5_dPhi_Min2p1`
    - `L1_ETMHF80_SingleJet55er2p5_dPhi_Min2p6` &rarr; `L1_ETMHF90_SingleJet55er2p5_dPhi_Min2p1`
    - `L1_DoubleIsoTau32er2p1` &rarr; `L1_DoubleIsoTau34er2p1`
    - `L1_HTT200_SingleLLPJet60` &rarr; `L1_HTT240_SingleLLPJet70`
    - `L1_DoubleIsoTau26er2p1_Jet55_RmOvlp_dR0p5` &rarr; `L1_DoubleIsoTau26er2p1_Jet70_RmOvlp_dR0p5` (_only_ in the highest emergency column 2.2E34)
- change in ps value for NotBPTX seeds JIRA [CMSLITDPG-1044](https://its.cern.ch/jira/browse/CMSLITDPG-1044):
    - `L1_SingleMuOpen_NotBptxOR` from 20 to 250; 
    - `L1_SingleJet20er2p5_NotBptxOR` from 20 to 100; 
    
### Last modifications (8st Nov 2022):
- seeds deactivated (in all columns) after new HCAL corrections [CMSLITDPG-1021](https://its.cern.ch/jira/browse/CMSLITDPG-1021):  
    - `L1_DoubleMu3_SQ_ETMHF30_HTT60er`
	- `L1_DoubleMu3_SQ_ETMHF30_Jet60er2p5_OR_DoubleJet40er2p5`
	- `L1_Mu3er1p5_Jet100er2p5_ETMHF30`
- LLP displaced jet seeds activated [CMSHLT-2525](https://its.cern.ch/jira/browse/CMSHLT-2525):   
    - `L1_HTT200_SingleLLPJet60`
    - `L1_DoubleLLPJet40`
- Change in seeds for ZeroBias:   
    - `L1_ZeroBias_copy`: ps value: 40438 &rarr; 13781 _only_ in column "2p0E34+ZeroBias+HLTPhysics" [CMSHLT-2551](https://its.cern.ch/jira/browse/CMSHLT-2551)
    - `L1_FirstCollisionInTrain`: ps value: 14057 &rarr; 59051 [CMSHLT-2517](https://its.cern.ch/jira/browse/CMSHLT-2517)
- For prefiring study with masking:
    - enable `L1_FirstBunchBeforeTrain`
    - bunch masking is working since run `361467` (masking of the last empty bx before train has been deployed since run 360850, but trigger counts were still observed because this seed was prescaled to 0).
<br/> 

 
## L1Menu_Collisions2022_v1_3_0-13.6TeV (in development) - study on backup columns
The PS table in development has presently the following definition of the backup columns
- **2.1e34** (same as 2.2e34 of official PS column) - seeds disabled w.r.t. 2.0E34:
    - `L1_DoubleJet_110_35_DoubleJet35_Mass_Min620`
    - `L1_DoubleJet_115_40_DoubleJet40_Mass_Min620`
    - `L1_ETMHF90`
    - `L1_ETMHF90_HTT60er`
    - `L1_DoubleMu0er2p0_SQ_dEta_Max1p6`
    - `L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p6`
    - `L1_DoubleIsoTau26er2p1_Jet55_RmOvlp_dR0p5`
- **2.2e34** - seeds disabled w.r.t. 2.1E34:
    - `L1_DoubleEG11_er1p2_dR_Max0p6`
<br/>   

<h2 align="center">
Description of the different formats
</h2>
<br/>   

- The PS table in **csv format** is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
- The PS table in **xlsx format** is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).
