# L1MenuRun3
This repository contains the L1 menu versions centrally developed and validated by the L1 Trigger DPG.
There are two directories:
* **Development**: it contains all versions of the L1 menu used for development purposed and offline rate studies
* **Official**: it contains all versions of the L1 menu deployed at P5 for the data-taking (with all relevant details about the deployment)

All details about each version of the L1 menu can be found [here](https://twiki.cern.ch/twiki/bin/view/CMS/SWGuideL1TriggerMenu#Official_L1_Menus).


### Instructions to create a new menu using the [Trigger Menu Editor](https://globaltrigger.web.cern.ch/upgrade/tme)
* **Install the TME**:
```
python3 -m venv tme
. tme/bin/activate
pip install --upgrade pip
pip install git+https://github.com/cms-l1-globaltrigger/tm-editor.git@0.16.0
```

After that, create a user shell script `tme.sh`
```
#!/bin/bash
. ~/tme/bin/activate
tm-editor $@
exit $?
```
and launch it (`source tme.sh`) to open an interactive window and work with the TME.

* **Open the TME and edit your reference menu**:
For a clear example about the setting and first usage of the TME, the bonus Ex. 3 of the [Trigger Exercise the DAS at Fermilab](https://twiki.cern.ch/twiki/bin/view/CMS/SWGuideCMSDataAnalysisSchoolLPC2023TriggerExercise#Bonus_Exercise_3_Modify_the_L1_m) can be followed, adapting it for the reference menu that you use as starting point.

### Instructions to use the tm-reporter tool to create the html version of the menu from the xml file and the corresponding twiki
* **Install the tm-reporter for the first time**:
```
python3 -m venv tm-reporter
. tm-reporter/bin/activate
pip install --upgrade pip
pip install git+https://github.com/cms-l1-globaltrigger/tm-reporter.git@2.12.0
```
* **Run the tm-reporter**:
The general command is:
```
tm-reporter [-m {html,twiki}] [-o L1Menu_Collisions2024_* ] L1Menu_Collisions2024_*.xml
```
Example working command to test that the tm-reporter is working fine with a xml file copied in your working directory:
```
tm-reporter -m html L1Menu_Collisions2024_v1_0_1.xml
```
