# What is this repository?
This repository is the submission for NordSec 2025 and contains the ns-3 source code used to generate test data.

To get started, install ns-3 by following the official installation guide:
https://www.nsnam.org/docs/release/3.44/installation/html/index.html.

For a quicker setup, you can also refer to the Quick Start guide:
https://www.nsnam.org/docs/release/3.44/installation/html/quick-start.html.

Once ns-3 is installed and built, locate the scratch directory inside ``ns-3.44`` (which itself is inside ``ns-allinone-3.44``).
Copy or move the ``localization_3log1.cc`` file into this scratch directory. Currently there is new version of ns-3, however please download the ns-3.44 since this version is what we used to generate test data.

This C++ file is responsible for generating synthetic test data. You can control the randomness of the generated datasets by adjusting the ``seed`` and run ``variables`` inside the main function. Changing these values alters the initial positions of UEs, BSs, and FBSs, allowing you to produce multiple distinct test datasets.

# Running a ns-3 code
Once ``localization_3log1.cc`` is placed in the scratch folder, follow these steps to run it:
1) Open the terminal.
2) Navigate to the ``ns-allinone-3.44`` (ns-3 project directory) using the cd command.
3) If you are in the ``ns-allinone-3.44`` directory, enter: ``cd ns-3.44``.
4) If you are in the ``ns-3.44``, Run the C++ file by executing: ``./ns3 run scratch/localization_3log1.cc``.

After running this command, a new output file (``localization no-building environment=Urban city-size=Large frequency=1.4e+09 grid=500X500 n(UE)=200 n(eNB+FBS)=5 lbs=46 fbs=48 seed=1 run=1.txt``) will appear in the ``ns-3.44`` directory.

## Note: This README section does not explain the purpose or function of each step. It is intended solely as a quick reference for running the ns-3 C++ code to generate test data.. 
