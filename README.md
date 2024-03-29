# OsirisCube
## Instructions
To use the program on a linux operating system, the following dependencies must be installed:
* `python3` an interpreter/compiler for python code, use package manager (`apt` for ubuntu) to install
* `pip` a package manager for python library modules, required for API interfacing. Use distro package manager to install (`apt` for ubuntu)
* `python-binance`, `selenium` use `pip install --user <name>`

Note: to verify the installation of the modules and find their implementation, use `pip show -f <name>`

## Content
Interprets TradingView's online javascript technical analysis summary and logs recommendations ver time

## Agenda 
- [x] start github (27/1/19)
- [x] add live price (28/1/19)
- [ ] log prices with recommendations
- [ ] work out trading fees
- [ ] add live testing
- [ ] add buy and sell order handling

## Files
### OsirisCube.py
Uses Selenium to download JS information from TradingView website. Also is used
as an interface with the user. Execute using `python3 OsirisCube.py`.
### readLog
Bash script for viewing escape sequenced log files, used with `./readLog logs/XRP.txt`
### keys.py
Contains various API keys as attributes and is provided as a skeleton since API keys should never be shared
### formatting.py
Contains a bunch of escape sequences for colors and stores welcome messages so
that they are abstracted from main code in `OsirisCube.py`
### tvSpeedometer.html
Uses embedded speedometers from TradingView's website for the user to manually
verify that OsirisCube is reading the same data that is available here.

## Screenshots
![image](https://user-images.githubusercontent.com/38335668/51811676-2c33a680-2302-11e9-89be-3a3c8a1cebb7.png)
![image](https://user-images.githubusercontent.com/38335668/51811638-f8588100-2301-11e9-9761-f7fa5226a6b5.png)
