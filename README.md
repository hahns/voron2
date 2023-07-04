## Voron 2 stls and configs backup

1. sudo service klipper stop
2. cd ~/klipper && git pull
3. make clean
4. make menuconfig
5. make
6. ./scripts/flash-sdcard.sh /dev/ttyACM0 fysetc-spider
7. sudo service klipper start

resonance testing without klipper numpy being built with pip:

1. TEST_RESONANCES AXIS=X OUTPUT=raw_data
2. TEST_RESONANCES AXIS=Y OUTPUT=raw_data

3. ~/klipper/scripts/calibrate_shaper.py /tmp/raw_data_x_ZZZ.csv -o /tmp/raw_data_x.png
4. ~/klipper/scripts/calibrate_shaper.py /tmp/raw_data_y_ZZZ.csv -o /tmp/raw_data_y.png

fix corrupt repo (emtpy git objects)

1. find .git/objects/ -type f -empty | xargs rm
2. git fetch -p
3. git fsck --full

## umbilical is a remix of: https://www.thingiverse.com/thing:5400946
=======
# umbilical is a remix of: https://www.thingiverse.com/thing:5400946
# voron0
