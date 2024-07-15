
# DIR865L_A1 has a Hardcoded Password

## DIR865L_A1 
version:V1.0.0 B24

## Description:
D-LINK DIR-865L_FIRMWARE_1.00B24 has a hardcoded password for the Alphanetworks account, which allows remote attackers to obtain root access via a telnet session.

## Source:
you may download it from : https://support.dlink.com/resource/products/DIR-865L/REVA/
![](https://github.com/IOTSakura/IOT/blob/main/D-Link/img/1.png)

## Analyse：
In file telnetd.sh has telnetd -l /usr/sbin/login -u Alphanetworks:$image_sign -i br0 &
![](https://github.com/IOTSakura/IOT/blob/main/D-Link/img/2.png) 

Then in /etc/config/image_sign has hardcoded passord：
![](https://github.com/IOTSakura/IOT/blob/main/D-Link/img/3.png)

login:
![](https://github.com/IOTSakura/IOT/blob/main/D-Link/img/4.png)
