# aibo_ers7
Sony AIBO ERS-7

OPEN-R SDK installation instructions on Ubuntu 18.04:
1. Open terminal and install required packages.\
`sudo apt update`\
`sudo apt-get install git flex`
2. Clone the aibo_ers7 GitHub repository.\
`git clone https://github.com/sheilaschoepp/aibo_ers7.git`
3. Enter the aibo_ers7/sony directory, setup file permissions and complete the OPEN-R SDK installation.\
`cd aibo_ers7/sony`\
`chmod a+x build-aibo-toolchain-3.3.6-r3.sh`\
`sudo ./build-aibo-toolchain-3.3.6-r3.sh`

To verify the OPEN-R SDK installation, compile and run a sample program by following the instructions on page 4 of "Testing OPEN-R Samples for Sony AIBO ERS-7" document in the aibo_ers7/tutorials folder.
