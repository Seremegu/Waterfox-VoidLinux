# Waterfox for Void Linux
This is a template for installing Waterfox on Void Linux.

The template is originally created by [mobinmob](https://codeberg.org/mobinmob/abyss-packages), but I updated the version. I will update it when there's a new Waterfox version when I can.


## Installation steps
Install xtools: `sudo xbps-install xtools`

Clone the void-packages repository: `git clone --depth 5 https://github.com/void-linux/void-packages`

Clone this repository: `git clone https://github.com/Seremegu/Waterfox-VoidLinux`

Copy the 'waterfox' folder to void-packages/srcpkgs: `cp -r Waterfox-VoidLinux/waterfox void-packages/srcpkgs`

Go to void-packages: `cd void-packages`

Build the package by executing this command: `./xbps-src pkg -j$(nproc) waterfox`

Install the package: `xi waterfox`
