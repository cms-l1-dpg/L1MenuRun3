# L1Menu_Collisions2022_v0_1_2

[![online preview](https://img.shields.io/badge/Online%20preview-click%20here-blue)](https://htmlpreview.github.io/?https://github.com/cms-l1-dpg/L1MenuRun3/master/development/L1Menu_Collisions2022_v0_1_2/L1Menu_Collisions2022_v0_1_2.html)

**Comment:** Menu for November 2021 Trigger Review for Run3. [Scale set reference, for grammar version 0.9]

An extensive description of the menu content and the differences w.r.t. the previous one is in the [twiki](https://twiki.cern.ch/twiki/bin/view/CMS/L1Menu_Collisions2022_v0_1_2).

- Seeds for Bmumu [https://its.cern.ch/jira/browse/CMSLITDPG-951] :
    - L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p6
    - L1_DoubleMu0er2p0_SQ_OS_dEta_Max1p5
    - L1_DoubleMuOpen_er1p4_OS_dEta_Max1p6
    - L1_DoubleMu3er2p0_SQ_OS_dR_Max1p4

- Seeds for Tau to 3mu search [https://its.cern.ch/jira/browse/CMSLITDPG-960]:
    - L1_TripleMu_2_1p5_0OQ_Mass_Max_15
    - L1_TripleMu_2SQ_1p5SQ_0OQ_Mass_Max_15

- Seeds for hadronic shower triggers [https://its.cern.ch/jira/browse/CMSLITDPG-953]:
    - L1_MuShower_OneNominal
    - L1_MuShower_OneTight

- new L1 Double EG seeds [https://its.cern.ch/jira/browse/CMSLITDPG-956]:
    - L1_DoubleEG_LooseIso16_LooseIso12_er1p5
    - L1_DoubleEG_LooseIso18_LooseIso12_er1p5
    - L1_DoubleEG_LooseIso20_LooseIso12_er1p5
    - L1_DoubleEG_LooseIso22_LooseIso12_er1p5
    - L1_DoubleEG_LooseIso25_LooseIso12_er1p5

- new L1 seeds for LLP searches wit Displaced Dimuon [https://its.cern.ch/jira/browse/CMSLITDPG-959]:
    - L1_DoubleMu0_upt15_upt7
    - L1_DoubleMu0_upt6ip123_upt4

- new L1 Double EG seeds for B-parking [https://its.cern.ch/jira/browse/CMSLITDPG-957]:
    - L1_DoubleEG10p5er1p22_dR_0p6
    - L1_DoubleEG10er1p22_dR_0p6
    - L1_DoubleEG9p5er1p22_dR_0p6
    - L1_DoubleEG9er1p22_dR_0p7
    - L1_DoubleEG8p5er1p22_dR_0p7
    - L1_DoubleEG8er1p22_dR_0p7
    - L1_DoubleEG7p5er1p22_dR_0p7
    - L1_DoubleEG7er1p22_dR_0p8
    - L1_DoubleEG6p5er1p22_dR_0p8
    - L1_DoubleEG6er1p22_dR_0p8
    - L1_DoubleEG5p5er1p22_dR_0p8
    - L1_DoubleEG5er1p22_dR_0p9

- new L1 ETMHF+recoiling Jet [https://its.cern.ch/jira/browse/CMSLITDPG-947]:
    - L1_ETMHF90_SingleJet60er2p5_ETMHF90_DPHI_MIN2p094
    - L1_ETMHF90_SingleJet60er2p5_ETMHF90_DPHI_MIN2p618
    - L1_ETMHF90_SingleJet80er2p5_ETMHF90_DPHI_MIN2p094
    - L1_ETMHF90_SingleJet80er2p5_ETMHF90_DPHI_MIN2p618

**NOTE:** The default behavior of the script sets the prescales of seeds using NotBptx or Bptx to zero. This is due to problems emulating NotBptx in ZeroBias. If you wish to include the prescale information for these seeds, use the --includeBptx option.
