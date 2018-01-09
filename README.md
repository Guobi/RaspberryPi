### Login into my Raspberry Pi
```
ssh pi@192.168.1.81
pi123567
```

### Scheduling tasks with crontab
#### Link
https://www.raspberrypi.org/documentation/linux/usage/cron.md  
https://crontab.guru/  
https://crontab.guru/every-1-minute  
#### View your currently saved scheduled tasks with:
```
crontab -l
```
#### Edit crontab
```
crontab -e
```
#### Example
```
* * * * * date>>/home/pi/Log/cron.log
ping -c 3 www.zaobao.com
```
#### Monitor cron
```
cat /var/log/syslog | grep CRON
grep CRON /var/log/syslog
tail -f /var/log/syslog | grep CRON
```

### Make .sh script executable
```
chmod +x PingZaobao.sh
```

### Establish a cloud connection
https://www.realvnc.com/en/connect/docs/raspberry-pi.html#raspberry-pi-connect-cloud
