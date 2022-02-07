# Raspberry Pi Web Camera

Raspberry pi web camera to stream video that can be used with a web browser

Tested with Raspberry Pi Zero W and Raspberry Pi camera v1.3 at 1080p

## Pre-Requisites

- Be connected a network.
- Have the camera enabled by using raspi-config
- install the dependecies:
> sudo apt-get install python3-picamera

## Installation

Clone this directory to the pi directory, cd into the directory

> sudo cp rpi_camera.service /lib/systemd/system/rpi_camera.service
> sudo chmod 644 /lib/systemd/system/rpi_camera.service
> sudo systemctl daemon-reload
> sudo systemctl enable rpi_camera.service
> sudo reboot

Using a web browser, navigate to port 8000 of the pi's IP address.

