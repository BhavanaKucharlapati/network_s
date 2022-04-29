# Collect data of packets before and after a DoS attack
## REQUIREMENTS
* VMware Workstation 16 Player
* Ubuntu 64-bit (Version 21.10)
## Simulated Router id range
* Team Number *4*
* Considered from 150 router id to 200 router id
## Open Vmware and start Ubuntu OS
* Open Terminal in Ubuntu Os

## Installation of Mininet
* Give following command line by line:
* $ sudo apt-get update
* $ sudo apt-get upgrade
* $ sudo apt-get dist-upgrade
#### Install required git software
* sudo apt-get install git
#### Install mininet 2.0 from source code
* $ git clone https://github.com/mininet/mininet
#### The Mininet project provides an install script. Run the script. 
* ~/mininet/util/install.sh -a


## INSTALL PACKAGES
You'll also need to run the following commands to install some required packages.  

 sudo apt install python3-pandas
 
 ## INSTALL WIRESHARK
 sudo apt install wireshark
 
## RUN THE CODE  
* Save the code to following path /mininet/custom  
* Run by using this command sudo mn –custom <python file name.py>  --topo= network
* We have considered file name as *beforeddos.py* and class name as *project*
 * We have considered file name as *afterddos.py* and class name as *project*

 ## CAPTURING DATA ON WIRESHARK
 * Open wireshark using sudo wireshark from terminal
 * Click on Capture, select interfaces you want to monitor the traffic 
 * Start capturing the packets by giving pingall in mininet console
 * Once pingall is completed, export the file to csv
 
 ## DDOS ATTACK
 * To launch ddos attack we have selected the ten nodes with highest degree and turned them off for about 25 minutes
 * In our ddos attack we have used following the nodes 160,155,164,193,181,192,179,156,184,182
 
## AUTHOR'S INFORMATION

* Bhavana Kucharlapati, bkucharl@ttu.edu, Section-001, +16692816244
*  Kavya Konisa, kkonisa@ttu.edu, Section-001, +18064129889
*   Venkata Revanth Kollipara, vekollip@ttu.edu, Section-001, +16198555656
*    Viswanth Boyina, vboyina@ttu.edu, Section-001, +18065007185
*    Srija Pullakhandam, spullakh@ttu.edu, Section-001, +18064013679
