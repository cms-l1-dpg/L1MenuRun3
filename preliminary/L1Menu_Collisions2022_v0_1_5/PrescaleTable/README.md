# Prescale and masks tables for the L1Menu_Collisions2022_v0_1_5

**Description of the different formats** 
* The PS table in csv format is used in the context of the rate estimation. It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools). 
* The PS table in xlsx format is used to allow easily changes; it represents the baseline to run TSG Tools in the context of the data-taking to produce an xml PS table used online. The xml file is included in L1+HLT keys using L1CE (L1 Configuration Editor). It is provided by default when a new menu is released and it is produced using [pstools](https://github.com/cms-l1-dpg/L1MenuTools/tree/master/pstools).
* The PS table in xml file is also used to run the L1 emulation of the prescales. This is the format accepted by the uGT emulator code. 
* The mask table in xml file is used together with the xml PS table to run the L1 emulation of the prescales.  

The following recipe allows to emulate L1 prescales instead of to take into account the full list of unprescaled algorithms by default.
```
process.load('L1Trigger.L1TGlobal.PrescalesVetos_cff')
process.load('L1Trigger.L1TGlobal.simGtStage2Digis_cfi')
process.load('L1Trigger.L1TGlobal.hackConditions_cff')                                                                                                       
process.L1TGlobalPrescalesVetos.PrescaleXMLFile = cms.string('l1prescales_L1MenuCollisions2022_v5.xml')      
process.L1TGlobalPrescalesVetos.FinOrMaskXMLFile = cms.string('mask_L1MenuCollisions2022_v5.xml')  
process.simGtStage2Digis.AlgorithmTriggersUnmasked = cms.bool(False)
process.simGtStage2Digis.AlgorithmTriggersUnprescaled = cms.bool(False)
process.simGtStage2Digis.PrescaleSet = cms.uint32(1)
```