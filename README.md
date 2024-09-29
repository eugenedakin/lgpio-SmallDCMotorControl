# lgpio-SmallDCMotorControl
Uses the libgpiod library to control a small Direct Current motor with Raspberry Pi 4 or 5

The Raspberry Pi can deliver a small amount of current and voltage to power light circuits. Using the internal power of the Raspberry Pi to provide too much amperage or voltage to a motor can cause issues such as: 1) destroying a chip on the Raspberry Pi motherboard, 2) cause the power surge to reboot the Raspberry Pi, or 3) corrupt the OS or program due to low voltage. The way to prevent this from occurring is to use a transistor.

![](https://github.com/eugenedakin/lgpio-SmallDCMotorControl/blob/main/NPNMotorScreenGrab.png)

The lgpio library can be installed Raspberry Pi OS (6 July 2023) and instructions are available at http://abyz.me.uk/lg/download.html

Install instructions are:

1) install Raspberry Pi OS (64-bit)
2) Open a terminal and type the following commands:
3) sudo apt install swig python3-dev
4) sudo apt install python3-setuptools
5) wget https://github.com/joan2937/lg/archive/master.zip
6) unzip master.zip
7) cd lg-master
8) make
9) sudo make install
10) create a Motor example program and copy the program and libraries to the RaspberryPi Desktop
11) give the executable permission to run with something like: 'sudo chmod +x NPNMotor'
12) run the program with something like: 'sudo ./NPNMotor'

![](https://github.com/eugenedakin/lgpio-SmallDCMotorControl/blob/main/SchematicNPNMotor.png)
