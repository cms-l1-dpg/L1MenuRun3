# Prescale and mask tables for the L1Menu_Collisions2022_v0_1_6

**Description of the different formats** 
* The PS table in **csv format** is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
* The PS table in **xlsx format** is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).
* The PS table in **xml format** is also used to run the L1 emulation of the prescales. This is the format accepted by the uGT emulator code. Both online and offline, it is provided together with a set of three additional xml files:
  - UGT_BASE_RS_PRESCALES_L1MenuCollisions2022_v6.xml
  - UGT_BASE_RS_FINOR_MASK_L1MenuCollisions2022_v6.xml
  - UGT_BASE_RS_VETO_MASK_L1MenuCollisions2022_v6.xml
  - UGT_BASE_RS_ALGOBX_MASK_L1MenuCollisions2022_v6.xml   

The following recipe allows to emulate L1 prescales instead of to take into account the full list of unprescaled algorithms by default.
```
cmsrel CMSSW_12_3_X_2022-03-01-1100
cd CMSSW_12_3_X_2022-03-01-1100/src/
cmsenv
git cms-init
git cms-addpkg L1Trigger/L1TGlobal
mkdir -p L1Trigger/L1TGlobal/data/Luminosity/startup
cd L1Trigger/L1TGlobal/data/Luminosity/startup
wget https://raw.githubusercontent.com/cms-l1-dpg/L1MenuRun3/master/preliminary/L1Menu_Collisions2022_v0_1_6/L1Menu_Collisions2022_v0_1_6.xml
wget https://raw.githubusercontent.com/cms-l1-dpg/L1MenuRun3/master/preliminary/L1Menu_Collisions2022_v0_1_6/PrescaleTable/UGT_BASE_RS_FINOR_MASK_L1MenuCollisions2022_v6.xml
wget https://raw.githubusercontent.com/cms-l1-dpg/L1MenuRun3/master/preliminary/L1Menu_Collisions2022_v0_1_6/PrescaleTable/UGT_BASE_RS_PRESCALES_L1MenuCollisions2022_v6.xml
cd -
git cms-addpkg L1Trigger/Configuration
emacs -nw L1Trigger/Configuration/python/customiseUtils.py ###change the menu name to L1Menu_Collisions2022_v0_1_6.xml
git cms-checkdeps -A -a
scram b -j 8

process.load('L1Trigger.L1TGlobal.simGtStage2Digis_cfi')
process.load('L1Trigger.L1TGlobal.hackConditions_cff')                                                                                                       
process.L1TGlobalPrescalesVetosFract.PrescaleXMLFile = cms.string('UGT_BASE_RS_PRESCALES_L1MenuCollisions2022_v6.xml')      
process.L1TGlobalPrescalesVetosFract.FinOrMaskXMLFile = cms.string('UGT_BASE_RS_FINOR_MASK_L1MenuCollisions2022_v6.xml')  
process.simGtStage2Digis.AlgorithmTriggersUnmasked = cms.bool(False)
process.simGtStage2Digis.AlgorithmTriggersUnprescaled = cms.bool(False)
process.simGtStage2Digis.PrescaleSet = cms.uint32(3)
```
**NOTE:** The default PrescaleSet is set to 3. This column corresponds to the set of prescales for an instantaneous luminosity 2E+34. See below the correspondence between the column identifier and the corresponding instantaneous luminosity scenario under consideration:
* 0: Emergency (all PS=0)
* 1: Unprescaled (all PS=1)
* 2: 2.2E+34
* 3: 2E+34
* 4: 1.7E+34
* 5: 1.5E+34
* 6: 1.3E+34
* 7: 1.1E+34
* 8: 9E+33
* 9: 6E+33
