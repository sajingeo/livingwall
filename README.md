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

sudo systemctl start wall.service
sudo systemctl stop wall.service
sudo systemctl enable wall.service
```

# Things to do
Disable audio (bcm28x)


## Credits:
bare conductive 
Jgarff for the lib

