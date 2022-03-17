# Dedicated PS table of the L1Menu_Collisions2022_v0_1_7 for rate studies

**Description of PS table**
* 2.00E+34 => Menu v0
* 1.90E+34 => Menu v0 + all suggestions (bmubmu option 1) 
                        [bits 51,52,55,81,82,91,92,210,211,222,261-263,272,278,335,362,388-390]
* 1.80E+34 => Menu v0 + all suggestions (bmubmu option 2)   
                        [bits 51,52,62,63,81,82,91,92,210,211,222,261-263,272,278,335,362,388-390]
* 1.70E+34 => B physics muon block: bmumu v1 + tau3mu [bits 55 + 81,82]
* 1.60E+34 => B physics muon block: bmumu v2 + tau3mu [bits 62,63 + 81,82]
* 1.50E+34 => B physics EG + DoubleEG seeds for low-mass diphoton search [bits 210,211 + 222]
* 1.40E+34 => LLP muons [bits 51,52]
* 1.30E+34 => LLP hadronic showers [bits 91,92]
* 1.20E+34 => MET plus jets [bit 335]
* 1.10E+34 => Only DoubleEG seeds for low-mass diphoton search [bit 222]
* 1.00E+34 => Only Tau3Mu [bits 81,82]
* 9.00E+33 => Only Double tau (+jet) seeds [bits 272,278]
* 8.00E+33 => Only Double jet + tau seed [bit 362]
* 7.00E+33 => Only OvlRm seeds [bits 278,362]
* 6.00E+33 => Only LLP jets, with:
	- L1_HTT200_SingleLLPJet60 (prescale 1) [bit 390]
	- L1_HTT160_SingleLLPJet50 (prescale 10) [bit 389]
	- L1_HTT120_SingleLLPJet40 (prescale 50) [bit 388]
* 5.00E+33 => Only singleIsoTau monitoring paths [bits 261-263]
