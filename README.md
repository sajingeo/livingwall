# livingwall
The living wall

# What it is
A interactive wall using bare conductive and neo pixels.

![alt text](https://github.com/sajingeo/livingwall/raw/master/IMG_2840.JPG "a pic")

# Dependency
```
sudo apt-get install picap
sudo apt-get install build-essential python-dev git scons swig

---- complete setup -----

git clone https://github.com/jgarff/rpi_ws281x.git
cd rpi_ws281x
scons
cd python
sudo python setup.py install

---- enable on boot ----
sudo cp  wall.service /lib/systemd/system/wall.service

sudo systemctl daemon-reload
sudo systemctl enable wall.service

 * sudo systemctl start wall.service
 * sudo systemctl stop wall.service

```

# Things to do
Disable audio (bcm28x)


## Credits:
bare conductive 
Jgarff for the lib 

### Note:
Raspberry pi has different pin numbering internally. The jxx number printed on the bare conductive pi-cap board are the phicial pin numbers on the pi.

Picap also calibrates on boot for the surface it mounted on, after connecting the pads make sure you reboot the pi.

