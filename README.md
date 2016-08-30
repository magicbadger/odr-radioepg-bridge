ODR Bridge EPG
==============

Creates a DAB EPG bitstream directly from the ODR multiplex configuration file, using RadioDNS to lookup SI and PI documents.

# Dependencies

* (python-hybridspi)[https://github.com/magicbadger/python-hybridspi]
* (odr-radiodns-bridge)[https://github.com/nickpiggott/odr-radiodns-bridge]
* (python-mot)
* (python-mot-epg)
* (python-msc)

# Usage

```
usage: generate-epg [-h] [-o OUTPUT] [-X] [-d DAYS] f

Encodes an EPG bitstream for services in a multiplex configuration file

positional arguments:
  f           multiplex configuration file

optional arguments:
  -h, --help  show this help message and exit
  -o OUTPUT   output bitstream file
  -X          turn debug on
  -d DAYS     number of days ahead to encode schedule files
```

Where the default number of `days` is 2, and the default output file is `output.dat`.
