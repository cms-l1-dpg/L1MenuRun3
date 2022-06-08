# Dedicated PS table of the L1Menu_Collisions2022_v1_1_0 for rate studies

**Description of PS table**

* 2E+34 => Menu v0 with: 
     - L1_SingleLooseIsoEG26er1p5 (bit 176) enabled
     - L1_DoubleMu0er1p5_SQ_dR_Max1p4 (bit 59) with PS=50 (instead of 2)

* 1.90E+34 => Higher thresholds for different groups of seeds
    Seeds disabled:
    MUONS
    - L1_SingleMu22 (bit 21)
    - L1_SingleMu22_BMTF (bit 22)
    - L1_SingleMu22_OMTF (bit 23)
    - L1_SingleMu22_EMTF (bit 24)
    EG seeds (former "opt4")
     - L1_SingleLooseIsoEG26er1p5 (bit 176)
     - L1_SingleLooseIsoEG28er2p5 (bit 178)
     - L1_SingleLooseIsoEG28er2p1 (bit 179) 
     - L1_SingleLooseIsoEG30er2p5 (bit 181)
     - L1_SingleIsoEG28er2p5 (bit 189)
     - L1_SingleIsoEG28er2p1 (bit 190)
     - L1_SingleIsoEG28er1p5 (bit 191)
     - L1_SingleIsoEG30er2p5 (bit 192)
     - L1_DoubleEG_LooseIso22_12_er2p5 (bit 223)
     - L1_LooseIsoEG26er2p1_HTT100er (bit 242)
     TAU
    - L1_DoubleIsoTau32er2p1 (bit 270) 
    JETMET
    - L1_SingleJet180 (bit 313) 
    - L1_SingleJet180er2p5 (bit 322) 
    - L1_DoubleJet150er2p5 (bit 343) 
    - L1_DoubleJet30er2p5_Mass_Min300_dEta_Max1p5 (bit 351) 
    - L1_DoubleJet_110_35_DoubleJet35_Mass_Min620 (bit 357) 
    - L1_TripleJet_95_75_65_DoubleJet_75_65_er2p5 (bit 372) 
    - L1_HTT320er_QuadJet_70_55_40_40_er2p4 (bit 389) 
    - L1_HTT360er (bit 404) 
    
* 1.80E+34 => 1.90E+34 + All new Run3 seeds (with Bmumu opt1)
    Seeds enabled:
     DoubleMu0 Upt seeds
     - L1_DoubleMu0_Upt6_IP_Min1_Upt4 (bit 49)
     - L1_DoubleMu0_Upt15_Upt7 (bit 50)
    Bmumu (opt1)
     - L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p6 (bit 55)
     - L1_DoubleMu0er2p0_SQ_dEta_Max1p5 (bit 56)
     - L1_DoubleMu0er2p0_SQ_dEta_Max1p6 (bit 53) with PS=190 -> control seed
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
     - L1_Mu18er2p1_Tau26er2p1_Jet55 (bit 281) -> control seed
     ETMHF+recoiling Jet seeds
     - L1_ETMHF90_SingleJet60er2p5_dPhi_Min2p1 (bit 335)
     - L1_ETMHF90_SingleJet60er2p5_dPhi_Min2p6 (bit 336)
     - L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p1 (bit 337)
     - L1_ETMHF90_SingleJet80er2p5_dPhi_Min2p6 (bit 338)
     Double Jet + One Tau seed
     - L1_DoubleJet35_Mass_Min450_IsoTau45er2p1_RmOvlp_dR0p5 (bit 362)
     LLP searches
     - L1_HTT120_SingleLLPJet40 (bit 384) with PS=100
     - L1_HTT160_SingleLLPJet50 (bit 385) with PS=50
     - L1_HTT200_SingleLLPJet60 (bit 386)
    
* 1.70E+34 => 1.90E+34 + Bmumu seed active (opt1)
    Seeds enabled for Bmumu:
     - L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p6 (bit 55)
     - L1_DoubleMu0er2p0_SQ_dEta_Max1p5 (bit 56)
     - L1_DoubleMu0er2p0_SQ_dEta_Max1p6 (bit 53) with PS=190

* 1.60E+34 => 1.90E+34 + New EG seeds for Run3 (Bparking, Higgs to Diphoton final state at Very low Mass)
    Seeds enabled:
     - L1_DoubleEG11_er1p2_dR_Max0p6 (bit 214)
     - L1_DoubleEG10p5_er1p2_dR_Max0p6 (bit 213)
     - L1_DoubleEG10_er1p2_dR_Max0p6 (bit 212)
     - L1_DoubleEG_LooseIso16_LooseIso12_er1p5 (bit 225)
     - L1_DoubleEG_LooseIso18_LooseIso12_er1p5 (bit 226)
     - L1_DoubleEG_LooseIso20_LooseIso12_er1p5 (bit 227)
     - L1_DoubleEG_LooseIso22_LooseIso12_er1p5 (bit 228)
     - L1_DoubleEG_LooseIso25_LooseIso12_er1p5 (bit 229)
