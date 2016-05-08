# Fridump
Fridump (v 0.1) is an open source memory dumping tool, primarily aimed to penetration testers and developers. Fridump is using the Frida framework to dump accessible memory addresses from any platform supported. It can be used from a Windows, Linux or Mac OS X system to dump the memory of an iOS, Android or Windows application.

Usage
---
The following are the main flags that can be used with fridump:

      positional arguments:
      process            the process that you will be injecting to

      optional arguments:
      -h, --help         show this help message and exit
      -o dir, --out dir  provide full output directory path. (def: 'dump')
      -u, --usb          device connected over usb
      -v, --verbose      verbose
      -r, --read-only    dump read-only parts of memory. More data, more errors
      -s, --strings      run strings on all dump files. Saved in output dir.
      --max-size bytes   maximum size of dump file in bytes (def: 20971520)

Pre-requisites
---
To use fridump you need to have frida installed on your python environment and frida-server on the device you are trying to dump the memory from.
The easiest way to install frida on your python is using pip:

    pip install frida
    
More information on how to install Frida can be found [here](http://www.frida.re/docs/installation/)

For iOS, installation instructions can be found [here](http://www.frida.re/docs/ios/).

For Android, installation instructions can be found [here](http://www.frida.re/docs/android/).

Note: On Android devices, make sure that the frida-server binary is running as server!

Disclaimer
---
* This is version 0.1 of the software, so I expect some bugs to be present
* I am not a developer, so my coding skills might not be the best
* This tool has been tested on a Windows 7 and a Mac OS X laptop, dumping memory of an iOS 8.2 app, Cyanogenmod 4.4.4 app and Windows 7 app.
 
Therefore, if this tool is not working for you, I apologise and I will try to fix it. Any suggestions and comments are welcome!