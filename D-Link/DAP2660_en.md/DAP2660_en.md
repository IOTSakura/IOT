# DAP2660
Firmware Information：DAP-2660_firmware_v2.00r140.bin
Download link：[DAP-2660_REVA_FIRMWARE_v2.00R140.zip](https://support.dlink.com/resource/products/DAP-2660/REVA/DAP-2660_REVA_FIRMWARE_v2.00R140.zip)
# Vulnerability Description：
There is a command injection vulnerability in DAP 2660 of Dlink, which can perform command execution through exeshll function in atp program.
![](vx_images/298693472235106_1.png)
This variable is used when requesting the st_stats_wl.xgi page on the web.
![](vx_images/584987377734955_1.png)
The command injection is done by concatenating the values of the exeshell parameter.
![](vx_images/104692879337850_1.png)
Result：
![](vx_images/288876787136535_1.png)