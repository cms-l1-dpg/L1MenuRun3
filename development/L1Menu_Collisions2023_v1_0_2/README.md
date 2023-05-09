# L1Menu_Collisions2023_v1_0_2

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/blob/master/development/L1Menu_Collisions2023_v1_0_2/L1Menu_Collisions2023_v1_0_2.html)

**Comment:** 
Reduced version of L1 menu v1_0_1 for testing purposes. It contains only seeds used in HLT paths present in the current HLT menus (both collisions and cosmics).
This menu has been created by using the last version of TME `0.15.3`, grammar `0.11` and updated scales to `scales_2023_02_16`.

<br/>

The following changes, from the last menu of 2023 (`L1Menu_Collisions2023_v1_0_1`), have been done:

### Removal of L1 seeds not currently used at the HLT
      * L1_SingleMuCosmics_BMTF
      * L1_SingleMuCosmics_OMTF
      * L1_SingleMuCosmics_EMTF
      * L1_SingleMuOpen_BMTF
      * L1_SingleMuOpen_OMTF
      * L1_SingleMuOpen_EMTF
      * L1_SingleMu0_DQ
      * L1_SingleMu0_BMTF
      * L1_SingleMu0_OMTF
      * L1_SingleMu0_EMTF
      * L1_SingleMu7_DQ
      * L1_SingleMu12_DQ_BMTF
      * L1_SingleMu12_DQ_OMTF
      * L1_SingleMu12_DQ_EMTF
      * L1_SingleMu22_OQ
      * L1_SingleMu22_DQ
      * L1_SingleMu22_BMTF
      * L1_SingleMu22_OMTF
      * L1_SingleMu22_EMTF
      * L1_SingleMu6er1p5
      * L1_SingleMu7er1p5
      * L1_SingleMu8er1p5
      * L1_SingleMu9er1p5
      * L1_SingleMu10er1p5
      * L1_SingleMu12er1p5
      * L1_SingleMu14er1p5
      * L1_SingleMu16er1p5
      * L1_SingleMu18er1p5
      * L1_DoubleMu0_OQ
      * L1_DoubleMu0_Mass_Min1
      * L1_DoubleMu_15_7_SQ
      * L1_DoubleMu_15_7_Mass_Min1
      * L1_DoubleMu0_Upt5_Upt5
      * L1_DoubleMu0er2p0_SQ_dR_Max1p4
      * L1_DoubleMu0er2p0_SQ_OS_dR_Max1p4
      * L1_DoubleMu0er2p0_SQ_dEta_Max1p6
      * L1_DoubleMu0er2p0_SQ_dEta_Max1p5
      * L1_DoubleMu0er1p5_SQ
      * L1_DoubleMu0er1p5_SQ_dR_Max1p4
      * L1_TripleMu0_OQ
      * L1_TripleMu0_SQ
      * L1_TripleMu3
      * L1_TripleMu_5_3_3_SQ
      * L1_TripleMu_5_3p5_2p5_OQ_DoubleMu_5_2p5_OQ_OS_Mass_5to17
      * L1_QuadMu0_OQ
      * L1_QuadMu0
      * L1_QuadMu0_SQ
      * L1_Mu12er2p3_Jet40er2p1_dR_Max0p4_DoubleJet40er2p1_dEta_Max1p6
      * L1_DoubleMu3_dR_Max1p6_Jet90er2p5_dR_Max0p8
      * L1_DoubleMu3_SQ_HTT240er
      * L1_DoubleMu3_SQ_HTT260er
      * L1_SingleEG28_FWD2p5
      * L1_SingleEG28er2p5
      * L1_SingleEG28er2p1
      * L1_SingleEG28er1p5
      * L1_SingleLooseIsoEG28_FWD2p5
      * L1_SingleIsoEG24er1p5
      * L1_SingleIsoEG26er1p5
      * L1_SingleIsoEG28_FWD2p5
      * L1_IsoEG32er2p5_Mt40
      * L1_DoubleEG_LooseIso20_10_er2p5
      * L1_DoubleEG_LooseIso22_10_er2p5
      * L1_TripleEG_16_12_8_er2p5
      * L1_TripleEG_16_15_8_er2p5
      * L1_TripleEG16er2p5
      * L1_LooseIsoEG30er2p1_HTT100er
      * L1_DoubleEG8er2p5_HTT340er
      * L1_SingleIsoTau32er2p1
      * L1_SingleTau70er2p1
      * L1_DoubleIsoTau32er2p1_Mass_Max90
      * L1_SingleJet35er2p5
      * L1_SingleJet120er2p5
      * L1_SingleJet35_FWD3p0
      * L1_SingleJet120_FWD3p0
      * L1_SingleJet140er2p5_ETMHF70
      * L1_SingleJet140er2p5_ETMHF80
      * L1_SingleJet140er2p5_ETMHF90
      * L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p1
      * L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p6
      * L1_DoubleJet30er2p5_Mass_Min200_dEta_Max1p5
      * L1_DoubleJet30er2p5_Mass_Min225_dEta_Max1p5
      * L1_DoubleJet30er2p5_Mass_Min250_dEta_Max1p5
      * L1_DoubleJet_80_30_Mass_Min420_Mu8
      * L1_ETT1200
      * L1_ETT1600
      * L1_ETM120
      * L1_ETMHF120_NotSecondBunchInTrain
      * L1_ETMHF110_HTT60er_NotSecondBunchInTrain
      * L1_MinimumBiasHF0_AND_BptxAND
      * L1_MinimumBiasHF0
      * L1_NotBptxOR
      * L1_BptxOR
      * L1_BptxXOR
      * L1_BptxPlus
      * L1_BptxMinus
      * L1_UnpairedBunchBptxPlus
      * L1_UnpairedBunchBptxMinus
      * L1_FirstBunchBeforeTrain
      * L1_FirstBunchInTrain
      * L1_SecondBunchInTrain
      * L1_SecondLastBunchInTrain
      * L1_LastBunchInTrain
      * L1_BPTX_NotOR_VME
      * L1_BPTX_OR_Ref3_VME
      * L1_BPTX_OR_Ref4_VME
      * L1_BPTX_RefAND_VME
      * L1_BPTX_AND_Ref1_VME
      * L1_BPTX_AND_Ref3_VME
      * L1_BPTX_AND_Ref4_VME
      * L1_BPTX_BeamGas_Ref1_VME
      * L1_BPTX_BeamGas_Ref2_VME
      * L1_BPTX_BeamGas_B1_VME
      * L1_BPTX_BeamGas_B2_VME
      * L1_TOTEM_1
      * L1_TOTEM_2
      * L1_TOTEM_3
      * L1_TOTEM_4


<br/>

**NOTE**: The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
