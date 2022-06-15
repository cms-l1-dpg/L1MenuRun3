# Dedicated PS table of the L1Menu_Collisions2022_v1_1_0 for rate studies with new Run3 seeds

**Description of PS table**

* 2E+34 => Menu v0 with: 
     - L1_SingleLooseIsoEG26er1p5 (bit 176) enabled
     - L1_DoubleMu0er1p5_SQ_dR_Max1p4 (bit 59) with PS=50 (instead of 2)
     
* 1.90E+34 => 2E+34 + All new Run3 seeds (with Bmumu opt1)
    Seeds enabled:
     DoubleMu0 Upt seeds
     - L1_DoubleMu0_Upt6_IP_Min1_Upt4 (bit 49)
     - L1_DoubleMu0_Upt15_Upt7 (bit 50)
    Bmumu (opt1)
     - L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p6 (bit 55)
     - L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p5 (bit 56)
     - L1_DoubleMu0er2p0_SQ_dEta_Max1p6 (bit 53) with PS=190 -> control seed
     - L1_DoubleMu0er2p0_SQ_dEta_Max1p5 (bit 54) with PS=190 -> control seed
     Tau3mu
     - L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12 (bit 82) 
     - L1_TripleMu_3SQ_2p5SQ_0OQ_Mass_Max12 (bit 83)
     - L1_TripleMu_2SQ_1p5SQ_0OQ (bit 74) with PS=100 -> control seed
     Muon shower
     - L1_SingleMuShower_Nominal (bit 92)
     - L1_SingleMuShower_Tight (bit 93)
     Bparking 
     - L1_DoubleEG11_er1p2_dR_Max0p6 (bit 214)
     - L1_DoubleEG10p5_er1p2_dR_Max0p6 (bit 213)
     - L1_DoubleEG10_er1p2_dR_Max0p6 (bit 212)
     Higgs to Diphoton final state at Very low Mass
     - L1_DoubleEG_LooseIso16_LooseIso12_er1p5 (bit 225)
     - L1_DoubleEG_LooseIso18_LooseIso12_er1p5 (bit 226)
     - L1_DoubleEG_LooseIso20_LooseIso12_er1p5 (bit 227)
     - L1_DoubleEG_LooseIso22_LooseIso12_er1p5 (bit 228)
     - L1_DoubleEG_LooseIso25_LooseIso12_er1p5 (bit 229)
     SingleIsoTau monitoring seeds
     - L1_SingleIsoTau32 (bit 262) with PS=800
     - L1_SingleTau70 (bit 263) with PS=50
     Double-tau+jet seed
     - L1_DoubleIsoTau26er2p1_Jet55_RmOvlp_dR0p5 (bit 283)
     - L1_DoubleIsoTau26er2p1_Jet70_RmOvlp_dR0p5 (bit 284)
     - L1_Mu18er2p1_Tau26er2p1_Jet55 (bit 281) -> control seed
     - L1_Mu18er2p1_Tau26er2p1_Jet70 (bit 282) -> control seed
     - L1_DoubleIsoTau35er2p1 (bit 272) 
     ETMHF+recoiling Jet seeds
     - L1_ETMHF90_SingleJet60er2p5_dPhi_Min2p1 (bit 335)
     - L1_ETMHF90_SingleJet60er2p5_dPhi_Min2p6 (bit 336)
     - L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p1 (bit 337)
     - L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p6 (bit 338)
     Double Jet + One Tau seed
     - L1_DoubleJet35_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5 (bit 362)
     LLP searches
     - L1_DoubleLLPJet40 (bit 383)
     - L1_HTT120_SingleLLPJet40 (bit 384) with PS=100
     - L1_HTT160_SingleLLPJet50 (bit 385) with PS=50
     - L1_HTT200_SingleLLPJet60 (bit 386)
     - L1_HTT240_SingleLLPJet70 (bit 387)
     
      Seeds disabled:
    - L1_DoubleIsoTau32er2p1 (bit 270)
    - L1_DoubleIsoTau32er2p1 (bit 271)
     
     
* 1.80E+34 => B physics muon block: bmumu v1 + tau3mu 
    Seeds enabled:
    Bmumu (opt1)
     - L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p6 (bit 55)
     - L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p5 (bit 56)
     - L1_DoubleMu0er2p0_SQ_dEta_Max1p6 (bit 53) with PS=190 -> control seed
     - L1_DoubleMu0er2p0_SQ_dEta_Max1p5 (bit 54) with PS=190 -> control seed
     Tau3mu
     - L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12 (bit 82) 
     - L1_TripleMu_3SQ_2p5SQ_0OQ_Mass_Max12 (bit 83)
     - L1_TripleMu_2SQ_1p5SQ_0OQ (bit 74) with PS=100 -> control seed
     
* 1.70E+34 => Bparking + DoubleEG seeds for low-mass diphoton search
    Seeds enabled:
     - L1_DoubleEG11_er1p2_dR_Max0p6 (bit 214)
     - L1_DoubleEG10p5_er1p2_dR_Max0p6 (bit 213)
     - L1_DoubleEG10_er1p2_dR_Max0p6 (bit 212)
     - L1_DoubleEG_LooseIso16_LooseIso12_er1p5 (bit 225)
     - L1_DoubleEG_LooseIso18_LooseIso12_er1p5 (bit 226)
     - L1_DoubleEG_LooseIso20_LooseIso12_er1p5 (bit 227)
     - L1_DoubleEG_LooseIso22_LooseIso12_er1p5 (bit 228)
     - L1_DoubleEG_LooseIso25_LooseIso12_er1p5 (bit 229)
    
* 1.60E+34 => LLP muons
    Seeds enabled:
     - L1_DoubleMu0_Upt6_IP_Min1_Upt4 (bit 49)
     - L1_DoubleMu0_Upt15_Upt7 (bit 50)
    
* 1.50E+34 => LLP hadronic showers
    Seeds enabled:
     - L1_SingleMuShower_Nominal (bit 92)
     - L1_SingleMuShower_Tight (bit 93)
    
* 1.40E+34 => ETMHF+recoiling Jet seeds
    Seeds enabled:
     - L1_ETMHF90_SingleJet60er2p5_dPhi_Min2p1 (bit 335)
     - L1_ETMHF90_SingleJet60er2p5_dPhi_Min2p6 (bit 336)
     - L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p1 (bit 337)
     - L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p6 (bit 338)

* 1.30E+34 => Only DoubleEG seeds for low-mass diphoton search
    Seeds enabled:
     - L1_DoubleEG_LooseIso16_LooseIso12_er1p5 (bit 225)
     - L1_DoubleEG_LooseIso18_LooseIso12_er1p5 (bit 226)
     - L1_DoubleEG_LooseIso20_LooseIso12_er1p5 (bit 227)
     - L1_DoubleEG_LooseIso22_LooseIso12_er1p5 (bit 228)
     - L1_DoubleEG_LooseIso25_LooseIso12_er1p5 (bit 229)

* 1.20E+34 => Only Tau3mu
    Seeds enabled:
     - L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max12 (bit 82) 
     - L1_TripleMu_3SQ_2p5SQ_0OQ_Mass_Max12 (bit 83)
     - L1_TripleMu_2SQ_1p5SQ_0OQ (bit 74) with PS=100 -> control seed
    
* 1.10E+34 => Only Double tau (+jet) seeds
    Seeds enabled:
     - L1_DoubleIsoTau26er2p1_Jet55_RmOvlp_dR0p5 (bit 283)
     - L1_DoubleIsoTau26er2p1_Jet70_RmOvlp_dR0p5 (bit 284)
     - L1_Mu18er2p1_Tau26er2p1_Jet55 (bit 281) -> control seed
     - L1_Mu18er2p1_Tau26er2p1_Jet70 (bit 282) -> control seed
     - L1_DoubleIsoTau35er2p1 (bit 272) 
    Seeds disabled:
    - L1_DoubleIsoTau32er2p1 (bit 270)
    - L1_DoubleIsoTau32er2p1 (bit 271)
    
* 1.00E+34 => Only Double jet + tau seed
    Seeds enabled:
     - L1_DoubleJet35_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5 (bit 362)

* 9.00E+33 => Only OvlRm seeds
    Seeds enabled:
     - L1_DoubleIsoTau26er2p1_Jet55_RmOvlp_dR0p5 (bit 283)
     - L1_DoubleIsoTau26er2p1_Jet70_RmOvlp_dR0p5 (bit 284)
     - L1_DoubleJet35_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5 (bit 362)
     - L1_DoubleIsoTau35er2p1 (bit 272) 
    Seeds disabled:
    - L1_DoubleIsoTau32er2p1 (bit 270)
    - L1_DoubleIsoTau32er2p1 (bit 271)

* 8.00E+33 => Only LLP jets
    Seeds enabled:
     - L1_DoubleLLPJet40 (bit 383)
     - L1_HTT120_SingleLLPJet40 (bit 384) with PS=100
     - L1_HTT160_SingleLLPJet50 (bit 385) with PS=50
     - L1_HTT200_SingleLLPJet60 (bit 386)
     - L1_HTT240_SingleLLPJet70 (bit 387)
    
* 7.00E+33 => Only singleIsoTau monitoring paths
    Seeds enabled:
     - L1_SingleIsoTau32 (bit 262) with PS=800
     - L1_SingleTau70 (bit 263) with PS=50
