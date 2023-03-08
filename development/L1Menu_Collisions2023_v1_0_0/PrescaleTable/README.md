# Prescale and mask tables for the L1Menu_Collisions2023_v1_0_0
%
**Description of the different formats** 
* The PS table in **csv format** is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
* The PS table in **xlsx format** is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).
**NOTE** : This is not the final ps table: it is updated *only* for the max lumi column (2e34), i.e. the 4th column. 
* The PS table in **xml format** is also used to run the L1 emulation of the prescales. This is the format accepted by the uGT emulator code. Both online and offline, it is provided together with a set of three additional xml files:
  - UGT_BASE_RS_PRESCALES_L1MenuCollisions2023_v1_0_0.xml
  - UGT_BASE_RS_FINOR_MASK_L1MenuCollisions2023_v1_0_0.xml
  - UGT_BASE_RS_VETO_MASK_L1MenuCollisions2023_v1_0_0.xml
  - UGT_BASE_RS_ALGOBX_MASK_L1MenuCollisions2023_v1_0_0.xml   

The following recipe allows to emulate L1 prescales instead of to take into account the full list of unprescaled algorithms by default.
```
cmsrel CMSSW_13_0_0_pre4/src
cd CMSSW_13_0_0_pre4/src
cmsenv
git cms-init
git cms-addpkg L1Trigger/L1TGlobal
mkdir -p L1Trigger/L1TGlobal/data/Luminosity/startup
cd L1Trigger/L1TGlobal/data/Luminosity/startup
wget https://raw.githubusercontent.com/cms-l1-dpg/L1MenuRun3/master/development/L1Menu_Collisions2023_v1_0_0/L1Menu_Collisions2023_v1_0_0.xml
wget https://raw.githubusercontent.com/cms-l1-dpg/L1MenuRun3/master/development/L1Menu_Collisions2023_v1_0_0/PrescaleTable/UGT_BASE_RS_FINOR_MASK_L1MenuCollisions2023_v1_0_0.xml
wget https://raw.githubusercontent.com/cms-l1-dpg/L1MenuRun3/master/development/L1Menu_Collisions2023_v1_0_0/PrescaleTable/UGT_BASE_RS_PRESCALES_L1MenuCollisions2023_v1_0_0.xml
cd -
git cms-addpkg L1Trigger/Configuration
emacs -nw L1Trigger/Configuration/python/customiseUtils.py ### L79: change the menu name to L1Menu_Collisions2023_v1_0_0.xml
git cms-checkdeps -A -a
scram b -j 8

[...lines to be added as L1 menu customisations in the python config file to run the L1 emulation...]
process.load('L1Trigger.L1TGlobal.simGtStage2Digis_cfi')
process.load('L1Trigger.L1TGlobal.hackConditions_cff')                                                                                                       
process.L1TGlobalPrescalesVetosFract.PrescaleXMLFile = cms.string('UGT_BASE_RS_PRESCALES_L1MenuCollisions2023_v1_0_0.xml')      
process.L1TGlobalPrescalesVetosFract.FinOrMaskXMLFile = cms.string('UGT_BASE_RS_FINOR_MASK_L1MenuCollisions2023_v1_0_0.xml')  
process.simGtStage2Digis.AlgorithmTriggersUnmasked = cms.bool(False)
process.simGtStage2Digis.AlgorithmTriggersUnprescaled = cms.bool(False)
process.simGtStage2Digis.PrescaleSet = cms.uint32(3)
```

The main usage of this recipe is the L1 emulation in the context of the preparation of L1Skimmed files for HLT studies (see the [L1PhysicsSkim](https://github.com/sanuvarghese/L1PhysicsSkim) repository for details and instructions). 

**NOTE:** The default PrescaleSet is set to 3. This column corresponds to the current set of prescales for the default configuration (2.00E34). See below the correspondence between the column identifier and the corresponding instantaneous luminosity scenario under consideration:
* 0: Emergency (all PS=0)
* 1: 2.20E+34
* 2: 2.10E+34
* 3: 2.00E+34
* 4: 1.90E+34
* 5: 1.80E+34
* 6: 1.70E+34
* 7: 1.60E+34
* 8: 1.50E+34
* 9: 1.40E+34
* 10: 1.30E+34
* 11: 1.20E+34
* 12: 1.10E+34
* 13: 1.00E+34
* 14: 9.00E+33
* 15: 8.00E+33
* 16: 7.00E+33
* 17: 6.00E+33

At the current stage, the main configuration for the **column 2.00E34** considers as baseline:
* core 2022 L1 Menu
* plus Option 1 new Bsmumu seeds
* plus new Tau3Mu seed
* plus DoubleEG11 seed for B Parking
* plus L1_HTT280 (DiHiggs Parking)
 
You can also use **column 1.70E34** with some other L1 seeds under discussion enabled:
* Seeds to design other options for Bsmumu:
  * Bit 78: L1_DoubleMu5_SQ_OS_dR_Max1p6
  * Bit 68: L1_DoubleMu3er2p0_SQ_OS_dR_Max1p6
  * Bit 64: L1_DoubleMu0er1p5_SQ_OS_dEta_Max1p2
* Central dijet seeds with invariant mass cuts: 
  * Bit 349-350-351: L1_DoubleJet30er2p5_Mass_Min200/225/250_dEta_Max1p5
* Seeds for W3pi:
  * Bit 273-278: L1_DoubleIsoTau28/30/32er2p1_Mass_Max80/90
