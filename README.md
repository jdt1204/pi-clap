# PI-Clap Updated

Clap detection and singnaling program for Raspberry Pi running on Python3.

## Hardware Requirements

- Raspberry Pi
- Microphone - I used a simple USB microphone

## Installation

The following assumes that you're already on a Raspberry Pi (I updated and tested on a Pi3), and that you already have RaspbianOS installed on the Pi

### Install OS-Level Packages

- portaudio19-dev
- python-all-dev (**Note**: This comes with Raspbian, but I put it here just in case)

### Clone Repo

Run `git clone https://github.com/jdt1204/pi-clap` to bring the project onto your PI.

### Install Python Packages

Navigate to the project directory (`cd path/to/pi-clap`) and run the following: 

```bash
sudo pip3 install -r requirements.txt
```

## Hardware Setup

Connect the output line to BCM #24 Pin on RPi.

## Run pi-clap

While in your project directory, run `sudo python main.py`.

( Try 2 claps to activate the output line for 1 sec. Note: Use 4 claps to exit from the system )

## References

 1. https://learn.adafruit.com/usb-audio-cards-with-a-raspberry-pi/instructions
 1. http://computers.tutsplus.com/articles/using-a-usb-audio-device-with-a-raspberry-pi--mac-55876
 1. http://forum.kodi.tv/showthread.php?tid=172072
 1. http://www.raspberrypi.org/documentation/installation/installing-images/
