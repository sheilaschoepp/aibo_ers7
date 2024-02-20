# aibo_ers7

## OPEN-R SDK installation instructions on Ubuntu 18.04

1. Open terminal and install required packages.  
`sudo apt update`  
`sudo apt-get install git flex`
2. Clone the aibo_ers7 GitHub repository.  
`git clone https://github.com/sheilaschoepp/aibo_ers7.git`
3. Enter the aibo_ers7/sony directory, setup file permissions and complete the OPEN-R SDK installation.  
`cd aibo_ers7/sony`  
`chmod a+x build-aibo-toolchain-3.3.6-r3.sh`  
`sudo ./build-aibo-toolchain-3.3.6-r3.sh`  

To verify the OPEN-R SDK installation, compile and run a sample program by following the instructions on page 4 of "Testing_OPEN-R_Samples_for_Sony_AIBO_ERS-7.pdf" in the aibo_ers7/tutorials folder.


## Source(s)

All documentation was downloaded in April 2020. Links annotated with an asterisk (*) are no longer accessible.



### programs/walking

1. [Generation of dynamic gaits in real Aibo using distributed neural networks.pdf](http://www.ouroboros.org/evo_gaits.html)
2. [nets.tar.gz](http://www.ouroboros.org/nets.tar.gz)
3. [openr_neural_controller.tar.gz](http://www.ouroboros.org/openr_neural_controller.tar.gz)

#### Walking Program Installation Instructions

1. Download and unpack openr_neural_controller.tar.gz and nets.tar.gz.  <path_to_folder> will refer to the directory where you have unpacked these files.
2. Insert a Sony memory stick into a memory card reader that is plugged into your machine.
3. In terminal, go to the memory stick's directory.  On my ubuntu 18.04 machine, this is in /media/<username>/<memory_card_id>.
4. Prepare the media stick with the OPEN-R SDK.  Use the wconsole memory protection option.  
`cp -rf /usr/local/OPEN_R_SDK/OPEN_R/MS_ERS7/WCONSOLE/memprot/* .`
5. Move the contents of openr_neural_controller/OPENR to the OPEN-R folder on your memory stick.  
`cd OPEN-R (you should be in the MS/OPEN-R directory)`  
`cp -rf <path_to_folder>/openr_neural_controller/OPENR/* .`
6. Move the contents of nets to the /MW/DATA/P folder.  
`cd MW/DATA/P (you should be in the MS/OPEN-R/MW/DATA/P folder)`  
`cp -rf <path_to_folder>/nets/* .`
7. Eject the memory stick and insert into the AIBO.



### sony/documentation

1. [ERS-7_User's_Guide_(Basic).pdf](https://www.sony-aibo.com/wp-content/uploads/2013/01/Sony-ERS-7-Manual.pdf) *
2. [ERS-7_User's_Guide_(PC-Network).pdf](http://www.aiai.ed.ac.uk/project/aibo/documents/ERS-7M2/AIBO-Network.pdf)
3. [ERS-7M2_User's_Guide_(AIBO_Entertainment_Player).pdf](http://www.aiai.ed.ac.uk/project/aibo/documents/ERS-7M2/AIBO-Entertainment-Player.pdf)
4. [AIBO_Brochure.pdf](http://www.aiai.ed.ac.uk/project/aibo/documents/ERS-7M2/AIBO-Brochure.pdf)
5. [AIBO_ERS-7_(MIND)_Brochure_II.pdf](https://www.sony-aibo.com/wp-content/uploads/2013/01/Sony-ERS-7-Manual.pdf) *
6. [ERS-7M2_Quick_Guide.pdf](http://www.aiai.ed.ac.uk/project/aibo/documents/ERS-7M2/AIBO-Quick-Guide.pdf)
7. [ERS-7M2_Quick_Guide.pdf](http://www.aiai.ed.ac.uk/project/aibo/documents/ERS-7M2/AIBO-Quick-Guide.pdf)
8. [AIBO_Mind_2_Wireless_LAN_Set_Up_Guide.pdf](http://www.aiai.ed.ac.uk/project/aibo/documents/ERS-7M2/AIBO-WLAN.pdf)
9. ERS-7M3_User's_Guide_(Basic).pdf from disk.
10. ERS-7M3_User's_Guide_(PC-Network).pdf from disk.
11. ERS-7M3_User's_Guide_(AIBO_Entertainment_Player_Ver._2.0).pdf from disk.

### sony/software

1. [Install OPEN-R on Linux.pdf](http://www.dogsbodynet.com/openr/install_openr_linux.html)


### tutorials

1. [AIBO_Programming.pdf](http://www.ouroboros.org/notes.pdf)
2. [AIBO_Programming_Tutorial.pdf](https://www.cc.gatech.edu/~tucker/courses/amrs/aibo/AIBOProgrammingTutorial.pdf) *
3. [AIBO_Programming_Using_OPEN-R_SDK.pdf](http://homes.dsi.unimi.it/~tirelli/robotics/material/tutorial/tutorial_OPENR_ENSTA-1.0.pdf) *
4. [AIBO_Quickstart_Manual.pdf](http://www.ouroboros.org/AIBO-quickstart.pdf)
5. [OPEN-R_Essentials.pdf](http://www.ouroboros.org/open-r_v1.0.pdf)
5. [Testing_OPEN-R_Samples_for_Sony_AIBO_ERS-7.pdf](https://paginas.fe.up.pt/~lpreis/robo2004/documents/samples.pdf)
