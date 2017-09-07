# PI-Clap Updated

Clap detection and singnaling program for Raspberry Pi running on Python3.

## Hardware Requirements

- Raspberry Pi
- Microphone - I used a simple USB microphone

## Installation

The following assumes that you're on Raspbian OS. 

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

 * Audio Driver [1],[2],[3].

###Setting up

1. [Download Raspbian OS](http://www.raspberrypi.org/downloads/).
2. [Install Raspbian OS in RPi](http://www.raspberrypi.org/documentation/installation/installing-images/).
3. Install all dependecies
4. Connect the output line to BCM #24 Pin on RPi.
5. Run 'sudo python main.py' command in terminal.

( Try 2 claps to activate the output line for 1 sec. Note: Use 4 claps to exit from the system )

###References

 1. https://learn.adafruit.com/usb-audio-cards-with-a-raspberry-pi/instructions
 2. http://computers.tutsplus.com/articles/using-a-usb-audio-device-with-a-raspberry-pi--mac-55876
 3. http://forum.kodi.tv/showthread.php?tid=172072
 4. http://www.raspberrypi.org/documentation/installation/installing-images/
