## Voron 2 stls and configs backup

sudo service klipper stop
cd ~/klipper
git pull
make clean
make menuconfig
make
./scripts/flash-sdcard.sh /dev/ttyACM0 spider-fystec
sudo service klipper start
