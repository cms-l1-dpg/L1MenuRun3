# Prescale and mask tables for the L1Menu_Collisions2022_v0_1_5

**Description of the different formats** 
* The PS table in **csv format** is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
* The PS table in **xlsx format** is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).
* The PS table in **xml format** is also used to run the L1 emulation of the prescales. This is the format accepted by the uGT emulator code. Both online and offline, it is provided together with a set of three additional xml files:
  - UGT_BASE_RS_PRESCALES_L1MenuCollisions2022_v5.xml
  - UGT_BASE_RS_FINOR_MASK_L1MenuCollisions2022_v5.xml
  - UGT_BASE_RS_VETO_MASK_L1MenuCollisions2022_v5.xml
  - UGT_BASE_RS_ALGOBX_MASK_L1MenuCollisions2022_v5.xml   

The following recipe allows to emulate L1 prescales instead of to take into account the full list of unprescaled algorithms by default.
```
cmsrel CMSSW_12_3_0_pre5
cd CMSSW_12_3_0_pre5/src
cmsenv
git cms-init 
git-cms-addpkg EventFilter/L1TRawToDigi
git-cms-addpkg L1Trigger/L1TCaloLayer1
git-cms-addpkg L1Trigger/L1TCalorimeter
git-cms-addpkg L1Trigger/L1TNtuples
git-cms-addpkg SimCalorimetry/HcalTrigPrimAlgos
git-cms-addpkg L1Trigger/L1TGlobal
git cms-merge-topic 36919
git cms-merge-topic 37046
mkdir -p L1Trigger/L1TGlobal/data/Luminosity/startup
cp  YOURXML.xml   L1Trigger/L1TGlobal/data/Luminosity/startup/.
git cms-checkdeps -A -a
scram b -j 8

process.load('L1Trigger.L1TGlobal.PrescalesVetosFract_cff')
process.load('L1Trigger.L1TGlobal.simGtStage2Digis_cfi')
process.load('L1Trigger.L1TGlobal.hackConditions_cff')                                                                                                       
process.L1TGlobalPrescalesVetosFract.PrescaleXMLFile = cms.string('UGT_BASE_RS_PRESCALES_L1MenuCollisions2022_v5.xml')      
process.L1TGlobalPrescalesVetosFract.FinOrMaskXMLFile = cms.string('UGT_BASE_RS_FINOR_MASK_L1MenuCollisions2022_v5.xml')  
process.simGtStage2Digis.AlgorithmTriggersUnmasked = cms.bool(False)
process.simGtStage2Digis.AlgorithmTriggersUnprescaled = cms.bool(False)
process.simGtStage2Digis.PrescaleSet = cms.uint32(2)
```
**NOTE:** The default PrescaleSet is set to 2. This column corresponds to the set of prescales for an instantaneous luminosity 2E+34. See below the correspondence between the column identifier and the corresponding instantaneous luminosity scenario under consideration:
* 0: Emergency
* 1: 2.2E+34
* 2: 2E+34
* 3: 1.7E+34
* 4: 1.5E+34
* 5: 1.3E+34
* 6: 1.1E+34
* 7: 9E+33
* 8: 6E+33
