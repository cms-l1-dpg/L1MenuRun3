# PS Table for Rate Study

## Table structure 

### 2e34: Baseline (with `L1_SingleMu22_BMTF`,`L1_SingleMu22_OMTF`,`L1_SingleMu22_EMTF` (bit 25-27) activated)

### 1.9e34: Baseline w/o Bmumu opt 1 and w/ Bmumu opt 3 (tau3mu active)
   - Deactivated the following seeds (w.r.t. baseline): 
      - `L1_DoubleMu0er1p4_SQ_OS_dEta_Max1p2` (bit 67) 
      - `L1_DoubleMu5_SQ_OS_dR_Max1p6` (bit 78) 
   - Activated the following seed (w.r.t. baseline): 
      - `L1_DoubleMu3er2p0_SQ_OS_dR_Max1p6` (bit 68) 

### 1.8e34: Same as 1.9e34 but w/o new seeds for tau3mu:
   - Deactivated the following seeds w.r.t. 1.9e34: 
      - `L1_TripleMu_3SQ_2p5SQ_0` (bit 84) 
      - `L1_TripleMu_3SQ_2p5SQ_0_Mass_Max12` (bit 85) 
      - `L1_TripleMu_3SQ_2p5SQ_0_OS_Mass_Max12` (bit 91) 
      - `L1_TripleMu_4SQ_2p5SQ_0_OS_Mass_Max12` (bit 92) 

### 1.7e34: Same as baseline, but with different ps value for the following seed:
   - `L1_DoubleEG11_er1p2_dR_Max0p6` (bit 214): ps=1 &rarr; ps=2 
