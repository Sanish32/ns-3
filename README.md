# What is this repository?
This repository contains the ns-3 source code used for generating test data.

To get started, install ns-3 by following the official installation guide:
https://www.nsnam.org/docs/release/3.44/installation/html/index.html

For a quicker setup, you can also refer to the Quick Start guide:
https://www.nsnam.org/docs/release/3.44/installation/html/quick-start.html

Once ns-3 is installed and built, locate the scratch directory inside ``ns-3.44`` (which itself is inside ``ns-allinone-3.44``).
Copy or move the ``localization_3log1.cc`` file into this scratch directory. Currently there is new version of ns-3, however please download the ns-3.44 since this version is what we used to generate test data.

This C++ file is responsible for generating synthetic test data. You can control the randomness of the generated datasets by adjusting the ``seed`` and run ``variables`` inside the main function. Changing these values alters the initial positions of UEs, BSs, and FBSs, allowing you to produce multiple distinct test datasets.


# Running a ns-3 code
Now, once you have ``localization_3log1.cc`` in scratch folder, go to the location of scratch folder in the terminal. To do this, follow the following steps:
1) Open the terminal.
2) Locate the ns-3 project. Command ``cd`` will be useful.
3) If you are able to go in ``ns-allinone-3.44``, now type ``cd ns-3.44``.
4) Now, run the C++ file (``localization_3log1.cc``) by typing ``./ns3 run scratch/localization_3log1.cc``. Once you run the command, you will see new file in the ``ns-3.44`` folder.

## Note: This readme file does not explain what each step means and what is its point. It only provides the necessary steps to run the ns-3 C++ code to generate test data for simplicity
. 
