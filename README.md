# Kimsufi Checker [![Build Status](https://travis-ci.org/t1hom7as/kimsufi_checker.svg?branch=master)](https://travis-ci.org/t1hom7as/kimsufi_checker) ![Python Version](https://img.shields.io/badge/python-3.6%2C%203.7-blue.svg)
A simple package to check for kimsufi server availablity.

Requires python 3.6 or above.

Currently only available for servers located in France.

## Installation

* Clone this repo
* Install the required dependancies
* Build the package
* Install the package
* Run the package


``` 
$ pip install -r requirements.txt
$ make build-python-source
$ pip install dist/kimsufi-checker-1.0.0.tar.gz
$ kimsufi-checker <args>
```

## Available arguments
```
kimsufi-checker <arg>
- ks1
- ks2
- ks3
- ks4
- ks5
- ks6
- ks7
- ks8
- ks9
- ks10
- ks11
- ks12
```
## Run example

```
$ kimsufi-checker ks2 && sms 'Kimsufi ks2 available!!!'

$ while true; do kimsufi-checker ks2 && ( sms 'Kimsufi ks2 available!!! https://www.kimsufi.com/uk/order/kimsufi.xml?reference=1801sk13'; notify-send -i /usr/share/icons/Tango/scalable/status/dialog-warning.svg 'Kimsufi KS-2 server available!!!' '<a href="https://www.kimsufi.com/uk/order/kimsufi.xml?reference=1801sk13">Buy Kimsufi KS-2 server</a>' ); sleep 8; done
```
