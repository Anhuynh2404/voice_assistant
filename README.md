# Hands-on-Tutorial-Voice-Assistant-on-Raspberry-Pi
A hands-on tutorial to build a voice assistant with Google Gemini on Raspberry Pi

Following the YouTube video below to learn more about this project:    
https://youtu.be/uV6hJQcuW4w

Before using this Python script, please add your Google Gemini API key to it first. 

Here is a schematic of the Raspberry Pi and LEDs    
<img src="https://github.com/techmakerai/Hands-on-Tutorial-Voice-Assistant-on-Raspberry-Pi/blob/main/schematic1.png" width="720"/>
 
## Hardware (\*):
1. Raspberry Pi
2. microSD card
3. Audio amplifier
4. Mini speaker
5. USB Microphone
6. (optional) LEDs and resistors
7. (optional) Breadboard 
8. uni SD Card Reader 
9. Power Supply for Raspberry Pi 3
10. Audio cable for speaker
11. Pi 4 case with cooling fan and heatsink

## Update and Upgrade the Raspberry Pi OS 

```console
sudo apt update
sudo apt upgrade
```


## Install a Firewall for the Raspberry Pi   

```console
sudo apt install ufw
sudo ufw allow ssh
sudo ufw enable
```

## Install Python and Pip
```console 
sudo apt install python3 python3-pip python3-venv
```

## Create Python Virtual Environment in the home directory 
```console 
python3 -m venv .venv
```

## Install Packages for Processing Audio Data
```console  
sudo apt install portaudio19-dev python3-pyaudio flac espeak 
```
## Create a Project Folder 
```console  
mkdir projects
cd projects
mkdir va
cd va 
```

## Activate Python Virtual Environment 
```console 
source ~/.venv/bin/activate
```  

## Install Python Packages 
You will need to install the following packages: 

```console
pip install speechrecognition sounddevice pyaudio
pip install -q -U google-generativeai
pip install gtts pygame gpiozero lgpio
```

## Run the Python Code
```console 
python gva7_led.py
``` 
Press "Ctrl + C" on your keyboard to exit from a running Python program. 

## Power off Raspberry Pi 
```console 
sudo poweroff
``` 

\* As a participant in the Amazon Associate Program, we earn from qualifying purchases.  
