# HUSKYLENSUploader
## Windows

* Install .Net Framework https://www.microsoft.com/zh-CN/download/details.aspx?id=56116
* Run K-Flash.exe on administrator.
* Select the firmware and serial port.
* Click to flash.

## Mac and Linux
We recommand to upload the firmware on windows using HUSKYLENSUploader as it has a GUI.
If you want to upload it on Mac and Linux please following these instruction:

* Install the USB Serial driver depending on your OS: https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers

* Install pip3 if you do not have in your OS

Install `pip3` on MAC

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
brew install python3
```

install `pip3`  on Linux

```
sudo apt install python3-pip
```

* Run the following code to install pyserial:

```
sudo pip3 install pyserial
```

* Go to the `HUSKYLENSUploader` folder

```
cd HUSKYLENSUploader
```

* Run the following code to update the firmware:

```
sudo python3 kflash.py -b 2000000 HUSKYLENSWithModelV0.4.6Stable.kfpkg
```


* Disconnect and reconnect the USB to reboot the HUSKYLENS to make it a refresh start up.

