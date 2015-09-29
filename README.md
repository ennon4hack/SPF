SPF (SpeedPhish Framework) is a python tool designed to allow for quick recon and deployment of simple social engineering phishing exercises.

# Requirements:
* dnspython
* twisted
* PhantomJS

# Usage:
```
usage: spf.py [-h] [-f <list.txt>] [-C <config.txt>] [--all] [--test] [-e]
              [-g] [-s] [--simulate] [-w] [-W] [-d <domain>]
              [-c <company's name>] [--ip <IP address>] [-v] [-y]

optional arguments:
  -h, --help           show this help message and exit
  -d <domain>          domain name to phish
  -c <company's name>  name of company to phish
  --ip <IP address>    IP of webserver defaults to [192.168.1.124]
  -v, --verbosity      increase output verbosity

input files:
  -f <list.txt>        file containing list of email addresses
  -C <config.txt>      config file

enable flags:
  --all                enable ALL flags... same as (-e -g -s -w)
  --test               enable all flags EXCEPT sending of emails... same as
                       (-e -g --simulate -w -y -v -v)
  -e                   enable external tool utilization
  -g                   enable automated gathering of email targets
  -s                   enable automated sending of phishing emails to targets
  --simulate           simulate the sending of phishing emails to targets
  -w                   enable generation of phishing web sites
  -W                   leave web server running after termination of spf.py

misc:
  -y                   automatically answer yes to all questions
```
Execution:
```
cd spf
python spf.py --test -d example.com
```
or to just test the websites:
```
cd spf
python web.py default.cfg
```

# Misc
DerbyCon 2015 Video

[![DerbyCon 2015 Video](https://img.youtube.com/v1/uyUyD1hwL9k/0.jpg)](https://www.youtube.com/watch?v=uyUyD1hwL9k)

BsidesLV 2015 Video

[![BSidesLV 2015 Video](http://img.youtube.com/vi/TtgJ3DaMtAo/0.jpg)](http://www.youtube.com/watch?v=TtgJ3DaMtAo)

BsidesKnox 2015 Video

[![BsidesKnox 2015 Viedo](http://img.youtube.com/vi/85QQwOduH6A/0.jpg)](http://www.youtube.com/watch?v=85QQwOduH6A)

Video of sample usage

[![Video of simple usage](http://img.youtube.com/vi/wMPlO41lo80/0.jpg)](http://www.youtube.com/watch?v=wMPlO41lo80)


