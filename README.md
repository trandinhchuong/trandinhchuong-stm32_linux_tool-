# trandinhchuong-stm32_linux_tool-
tools
## Installing & using ST-Link v2 to flash STM32 targets on Linux
  sudo apt-get install libusb-1.0-0-dev
  git clone https://github.com/texane/stlink stlink.git
  cd stlink
  make
# install binaries:
  sudo cp build/Debug/st-* /usr/local/bin
# install udev rules
  sudo cp etc/udev/rules.d/49-stlinkv* /etc/udev/rules.d/
# and restart udev
  sudo udevadm control --reload

