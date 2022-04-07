# Dedicated PS table of the L1Menu_Collisions2022_v1_0_0 for rate studies

**Description of PS table**
* 2E+34 => Menu v0
* 1.90E+34 => Menu v0 + all suggestions (bmubmu option 1) 
                        [bits 49,50,53,55,74,82,91,92,212-214,225,262,263,272,278,335,362,388-390]
* 1.80E+34 => Menu v0 + all suggestions (bmubmu option 2)   
                        [bits 49,50,62,63,74,82,91,92,212-214,225,262,263,272,278,335,362,388-390]
* 1.70E+34 => B physics muon block: bmumu v1 + tau3mu [bits 53,55 + 74,82]
* 1.60E+34 => B physics muon block: bmumu v2 + tau3mu [bits 62,63 + 74,82]
* 1.50E+34 => B physics EG + DoubleEG seeds for low-mass diphoton search [bits 212-214 + 225]
* 1.40E+34 => LLP muons [bits 49,50]
* 1.30E+34 => LLP hadronic showers [bits 91,92]
* 1.20E+34 => MET plus jets [bit 335]
* 1.10E+34 => Only bmumu v1 [bits 53,55]
* 1E+34 => Only Tau3Mu [bits 74,82]
* 9E+33 => Only Double tau (+jet) seeds [bits 272,278]
* 8E+33 => Only Double jet+tau seed + "L1_DoubleIsoTau35er2p1" [bit 362 + 272]
* 7E+33 => Only RmOvlp seeds (with "L1_DoubleIsoTau35er2p1") [bits 272,278,362]
* 6E+33 => Only LLP jets, with:
	- L1_HTT200_SingleLLPJet60 (prescale 1) [bit 390]
	- L1_HTT160_SingleLLPJet50 (prescale 10) [bit 389]
	- L1_HTT120_SingleLLPJet40 (prescale 50) [bit 388]
* 5E+33 => Only singleTau monitoring paths, with:
    - L1_SingleIsoTau32er2p1 (prescale 800) [bits 262]
    - L1_SingleTau70er2p1 (prescale 50) [bits 263]
* 4E+33 => Menu v0 + "L1_DoubleIsoTau35er2p1" seed [bit 272]


**NOTE**
* When the seed "L1_DoubleIsoTau35er2p1" (bit 272) is active, the two equivalent seeds with lower pt thresholds "L1_DoubleIsoTau32er2p1", "L1_DoubleIsoTau34er2p1" have PS = 0.
* The new BPH seeds added for systematics evaluation (bit 53,54,74) are ON when their corresponding main seeds are active. The PS values used for these seeds are tuned so that their rate is about 100 Hz. In particular, the following PS values are used:
    - L1_DoubleMu0er2p0_SQ_dEta_Max1p6 (bit 53): PS = 190
    - L1_DoubleMu0er2p0_SQ_dEta_Max1p5 (bit 54): PS = 190
    - L1_TripleMu_2SQ_1p5SQ_0OQ (bit 74): PS = 100
* The seeds L1_SingleMu22_BMTF/OMTF/EMTF (bits 20-22) have been activated in all scenarios, with PS=1 (before they had PS=0).
