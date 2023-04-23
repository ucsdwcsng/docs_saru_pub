# How to flash to EVB1000 using a Nucleo board and WSL2.

## 1. check busid of nucleo board

```
$ usbipd.exe wsl list
BUSID  VID:PID    DEVICE                                                        STATE
1-3    0483:374b  ST-Link Debug, USB Mass Storage, STMicroelectronics STL...  Not attached
1-7    8087:0a2b  Intel(R) Wireless Bluetooth(R)                           Not attached
2-1    0eef:c01d  USB Input Device                                              Not attached
2-3    5986:054c  USB HD Webcam                                                 Not attached
```

## 2. connect USB to WSL2

in this case, 1-3 is ST-Link debugger.

```
usbipd.exe wsl attach --busid 1-3
```

## 3. check stlink on WSL2.


```

