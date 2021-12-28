# Raspi Configuration

- `boot-cmdline.txt`: Used `/boot/cmdline.txt` file. Added `usb-storage.quirks` not to use _USB Attached SCSI (UAS)_ but legacy _usb-storage_. With UAS the used SSD had only bad very bad performance. Details [here](https://www.raspberrypi.org/forums/viewtopic.php?f=28&t=245931).

- Exact value for Intensio external SSD: `usb-storage.quirks=152d:0579:u`
