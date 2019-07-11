# esp-idf-ds1302
DS1302 RTC Driver for esp-idf

I ported from [here](https://github.com/Erriez/ErriezDS1302/tree/master/src).   

```
git clone https://github.com/nopnop2002/esp-idf-ds1302
cd esp-idf-ds1302
make menuconfig
make flash
```



---

# Set Clock Mode   

This mode set RTC initial value using NTP time Server.   
you have to set these config value using menuconfig.   

![config-ds1302-1](https://user-images.githubusercontent.com/6020549/59513345-a3568980-8ef5-11e9-85c8-4ed1744d73e1.jpg)

![config_ds1302-2](https://user-images.githubusercontent.com/6020549/59513344-a3568980-8ef5-11e9-9e91-79d73f91a3dc.jpg)

you have to set gpio & NTP Server using menuconfig.   

![config-ds1302-11](https://user-images.githubusercontent.com/6020549/59513485-e3b60780-8ef5-11e9-9d77-aee1cb9d40dd.jpg)

![config-ds1302-12](https://user-images.githubusercontent.com/6020549/59513496-e9135200-8ef5-11e9-9f03-2ad96fc7c1c9.jpg)

---

# Get Clock Mode   

This mode take out the time from a RTC clock.   
you have to change mode using menuconfig.   

![config-ds1302-11](https://user-images.githubusercontent.com/6020549/59513485-e3b60780-8ef5-11e9-9d77-aee1cb9d40dd.jpg)

![config-ds1302-13](https://user-images.githubusercontent.com/6020549/59514431-ca15bf80-8ef7-11e9-9b59-ff4b5510ec0f.jpg)

![ds1302-13](https://user-images.githubusercontent.com/6020549/59513594-1fe96800-8ef6-11e9-9b53-a2d2626d784f.jpg)

---

# Get the time difference of NTP and RTC   

This mode get time over NTP, and take out the time from a RTC clock.   
Calculate time difference of NTP and RTC.   
you have to change mode using menuconfig.   

![config-ds1302-11](https://user-images.githubusercontent.com/6020549/59513485-e3b60780-8ef5-11e9-9d77-aee1cb9d40dd.jpg)

![config-ds1302-14](https://user-images.githubusercontent.com/6020549/59556587-9de56600-8fff-11e9-8a02-69eacd675ad8.jpg)

![ds1302-14](https://user-images.githubusercontent.com/6020549/59556737-b2772d80-9002-11e9-921e-4a794605dd86.jpg)

---

# Time difference of 1 week later.   

![ds1302-1week](https://user-images.githubusercontent.com/6020549/59961747-e082d300-9516-11e9-87ea-dba01d00e3be.jpg)

