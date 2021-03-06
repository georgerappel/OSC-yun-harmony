OSC-yun-harmony
===============

A full implementation of OSC messages sent from Arduino Yun to Pure Data or any OSC server using local UDP.

How to use:
---

1) Download pyOSC from: https://trac.v2.nl/wiki/pyOSC.

2) Create /OSCtoPD folder on yun:
```c
mkdir OSCtoPD
```
3) Copy lib to yun:
```c
scp -r /User/.../Downloads/pyOSC-0.3.5b-5294 root@arduino.local:/OSCtoPD
```
4) Install pyOSC on yun:
```c
python setup.py install
```
5) Copy python script to yun:
```c
scp /Users/.../Desktop/oscsend.py root@arduino.local:/OSCtoPD
```
6) Change exec mode on script:
```c
chmod +x oscsend.py
```
7) Copy yunOSC folder to arduino/libraries path.

8) Open pure data patch.

9) Open Arduino IDE.

10) Choose File->Examples->yunOSC->send_example.

11) Update sketch with your ip

12) Upload and listen to your analog reads.
