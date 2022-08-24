## Voron 2 stls and configs backup

1. sudo service klipper stop
2. cd ~/klipper && git pull
3. make clean
4. make menuconfig
5. make
6. ./scripts/flash-sdcard.sh /dev/ttyACM0 fysetc-spider
7. sudo service klipper start

## umbilical is a remix of: https://www.thingiverse.com/thing:5400946
