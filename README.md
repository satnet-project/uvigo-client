

### SATNet client for the University of Vigo.


This repository contains the source code for  the SATNet client created 
for the University of Vigo.

This is the code for a GS with a TNC to demodulate/modulate the frames 
which are being received/sent from/to the satellite.

### Installation

Steps to install the UVigo client for the SATNet network:

1. To install the dependencies run, from the Scripts folder:

`setup.sh`

You will need root privileges.

#### Dependencies

Before starting the script should be activate the corresponding virtualenv to satisfy the required dependencies.

    source .venv/bin/activate

#### Normal operation

To run this script you have the following options:

1. If you want to enter data connection from the user interface.

    `python client_amp.py`

2. To start a serial connection directly from the command line will have to enter 
the parameters as follows:

    `python client_amp.py -g -u username -p userpassword -t slot -c serial -s serialport -b baudrate`
    
3. For a UDP connection you must set an ip and a port: 

    `python client_amp.py -g -u username -p userpassword -t slot -c udp -i ip -u ipport`
