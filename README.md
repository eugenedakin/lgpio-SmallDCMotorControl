# lgpio-SmallDCMotorControl
Uses the libgpiod library to control a small Direct Current motor with Raspberry Pi 4 or 5

The Raspberry Pi can deliver a small amount of current and voltage to power light circuits. Using the internal power of the Raspberry Pi to provide too much amperage or voltage to a motor can cause issues such as: 1) destroying a chip on the Raspberry Pi motherboard, 2) cause the power surge to reboot the Raspberry Pi, or 3) corrupt the OS or program due to low voltage. The way to prevent this from occurring is to use a transistor.

![](https://github.com/eugenedakin/lgpio-SmallDCMotorControl/blob/main/NPNMotorScreenGrab.png)

The lgpio library can be installed Raspberry Pi OS (6 July 2023) and instructions are available at http://abyz.me.uk/lg/download.html

Install instructions are:

1) sudo apt install swig python-dev python3-dev
2) sudo apt install python-setuptools python3-setuptools
3) wget http://abyz.me.uk/lg/lg.zip
4) unzip lg.zip
5) cd lg
6) make
7) sudo make install
8) create a Motor example program and copy the program and libraries to the RaspberryPi Desktop
9) give the executable permission to run with something like: 'sudo chmod +x NPNMotor'
10) run the program with something like: 'sudo ./NPNMotor'

![](https://github.com/eugenedakin/lgpio-SmallDCMotorControl/blob/main/SchematicNPNMotor.png)
