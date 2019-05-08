# MiBand3
Library to work with Xiaomi MiBand 3

Base lib provided by Leo Soares
Additional debug & fixes was made by Volodymyr Shymanskyy


# [DEMO](https://www.youtube.com/watch?v=9TL2qmBpVms)


# Run

### Install dependencies

`pip install -r requirements.txt`

Turn on your Bluetooth

Unpair you MiBand2 from current mobile apps

Find out your MiBand3 MAC address

```sudo hcitool lescan```

Run this to auth device

```python main.py MAC_ADDRESS --init```

If you having problems(BLE can glitch sometimes)

```sudo hciconfig hci0 reset```


If you got the followin error

```fatal error: glib.h: No such file or directory```

then try this 

```sudo apt-get install libglib2.0-dev```

If you got the following error

```ImportError: No module named 'crc16'```

then try this 

```python -m pip install crc16```
