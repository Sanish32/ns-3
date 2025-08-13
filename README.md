# What is this repository?
This repository contains the ns-3 codes for generating test data. The installation guide can be found in https://www.nsnam.org/docs/release/3.44/installation/html/index.html. Please follow the necessary steps to download, build and test ns-3 simulator (https://www.nsnam.org/docs/release/3.44/installation/html/quick-start.html). 

There is a scratch folder inside the ns-3.44 folder (this folder is inside ns-allinone-3.44) and now, copy/move the ``localization_3log1.cc``. This C++ file is used for generating our synthetic test data. Adjusting ``seed`` and ``run`` variables (inside main function) allows to introduce randomness in our multiple test data, since adjusting those variables change the initial locations of UEs, BSs and FBS.

# Running a ns-3 code
Now, once you have ``localization_3log1.cc`` in scratch folder, go to the location of scratch folder in the terminal. To do this, follow the following steps:
1) Open the terminal.
2) Locate the ns-3 project. Command ``cd`` will be useful.
3) If you are able to go in ``ns-allinone-3.44``, now type ``cd ns-3.44``.
4) Now, run the C++ file (``localization_3log1.cc``) by typing ``./ns3 run scratch/localization_3log1.cc``. Once you run the command, you will see new file in the ``ns-3.44`` folder.

## Note: This readme file does not explain what each step means and what is its point. It only provides the necessary steps to run the ns-3 C++ code to generate test data for simplicity
. 
