# trandinhchuong-stm32_linux_tool-
tools
## Installing & using ST-Link v2 to flash STM32 targets on Linux
  sudo apt-get install libusb-1.0-0-dev
  git clone https://github.com/texane/stlink stlink.git
  cd stlink
  make
# install binaries:
1.  sudo cp build/Debug/st-* /usr/local/bin
2.  sudo cp build/Release/st-* /usr/local/bin/
# install udev rules
  sudo cp etc/udev/rules.d/49-stlinkv* /etc/udev/rules.d/
# and restart udev
  sudo udevadm control --reload
## using comment
# st-flash write file.bin 0x08000000

##clock config
https://stm32f4-discovery.net/2015/01/properly-set-clock-speed-stm32f4xx-devices/

## install openocd
https://hackaday.io/page/4991-compiling-openocd-from-source-on-ubuntu-1604
## debug
https://www.bartslinger.com/cx-10-quadcopter/debugging-stm32-from-qtcreator/
https://www.youtube.com/watch?v=a7R4A0WTrds
