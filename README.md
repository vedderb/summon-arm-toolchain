Based on https://github.com/esden/summon-arm-toolchain

I have made the following changes:
* Updated GCC to version 7.3 
* Updated binutils to 2.30
* Updated newlib to version 2.4
* Include libopencm3 support as default
* Tested on FreeRTOS with libopencm3

Usage on debian-based linux distributions (e.g. Ubuntu):

1. Install dependencies

sudo apt-get install build-essential git flex bison libgmp3-dev libmpfr-dev libncurses5-dev libmpc-dev autoconf texinfo libtool libftdi-dev libusb-1.0-0-dev zlib1g zlib1g-dev gcc


2. Run the script

./summon-arm-toolchain

3. (Optional) add to path

sudo su

echo 'export PATH=/home/YOUR_USER/sat/bin:$PATH' > /etc/profile.d/arm_tools.sh

exit

4. Done!

Also, see:

http://vedder.se/2012/07/get-started-with-stm32f4-on-ubuntu-linux/

for a complete tutorial

Compile twice to get through the gcc failure (?!). Requires about 7 GB disk space.
