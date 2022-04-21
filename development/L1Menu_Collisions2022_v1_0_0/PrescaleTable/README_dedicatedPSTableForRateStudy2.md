# Dedicated PS table of the L1Menu_Collisions2022_v1_0_0 for rate studies2

**Description of PS table**

* 2E+34 => Menu v0

* 1.90E+34 => MUONS 
    Seeds disabled:
    - SingleMu22 (bit 19) 
    - SingleMu22_BMTF (bit 20) 
    - SingleMu22_OMTF (bit 21) 
    - SingleMu22_EMTF (bit 22)
    
* 1.80E+34 => EG (opt1): SingleEGX->SingleEGX+2
    Seeds disabled:
    - L1_SingleEG36er2p5 (bit 168) 
    - L1_SingleLooseIsoEG28er2p5 (bit 178)
    - L1_SingleLooseIsoEG28er2p1 (bit 179) 
    - L1_SingleIsoEG28er2p5 (bit 189) 
    - L1_SingleIsoEG28er2p1 (bit 188) 
    - L1_SingleIsoEG28er1p5 (bit 187) 
    - L1_LooseIsoEG28er2p1_Jet34er2p5_dR_Min0p3 (bit 239) 
    - L1_LooseIsoEG26er2p1_HTT100er (bit 242) 
    - L1_LooseIsoEG22er2p1_IsoTau26er2p1_dR_Min0p3 (bit 257) 
    
* 1.70E+34 => EG (opt2): SingleEGX->SingleEGX+4
    Seeds disabled: same as 1.80E+34, with the addition of: 
    - L1_SingleEG38er2p5 (bit 169) 
    - L1_SingleIsoEG30er2p5 (bit 192) 
    - L1_SingleIsoEG30er2p1 (bit 193)
    - L1_LooseIsoEG28er2p1_HTT100er (bit 243) 

* 1.60E+34 => TAU
    Seeds disabled:
    - L1_DoubleIsoTau32er2p1 (bit 270) 
    - L1_DoubleIsoTau34er2p1 (bit 271) 

* 1.50E+34 => JETMET
    Seeds disabled:
    - L1_HTT360er (bit 404) 
    - L1_SingleJet180 (bit 313) 
    - L1_SingleJet180er2p5 (bit 322) 
    - L1_DoubleJet150er2p5 (bit 343) 
    - L1_DoubleJet30er2p5_Mass_Min300_dEta_Max1p5 (bit 351) 
    - L1_DoubleJet_110_35_DoubleJet35_Mass_Min620 (bit 357) 
    - L1_TripleJet_95_75_65_DoubleJet_75_65_er2p5 (bit 372) 
    - L1_HTT320er_QuadJet_70_55_40_40_er2p5 (bit 385) 
    
* 1.40E+34 => ALL: 1.90E+34 + 1.80E+34 + 1.60E+34 + 1.50E+34

* 1.30E+34 => ALL: 1.90E+34 + 1.80E+34 + 1.70E+34 + 1.50E+34

