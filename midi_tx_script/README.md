Send MIDI message via Serial Port.

In Raspberry Pi, TTL232 USB Dongle and other SBCs

connect SBC's Serial TX to Flipper zero RX / GND to GND.

Then

```
pip install mido pyserial
```

then 

```
python midi_tx.py -i demo_song.mid -p /dev/your_device --tempo 90
```

options:
```
  -h, --help            show this help message and exit
  -p PORT, --port PORT  Serial port name
  -i INPUT, --input INPUT
                        MIDI file path
  -b BAUD, --baud BAUD  Baud rate (default: 31250)
  -t TEMPO, --tempo TEMPO
                        Override tempo (in BPM)
```
