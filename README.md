# Multitech-conduit-SDcard-logger

The bashscript has been written to log LoRa packets information (tmst, RSSI, Time and other) on to the SD card found inside Multitech conduit. 

Please follow the steps as below:-

Log in to the multitech conduit either using ethernet or USB port

Copy the contents of the Datalogger.txt

Create a bashscript file by writing the following command in the terminal 
  nano /usr/sbin/dataLogger.sh

Paste the contents in to the newly created bashscript file and save it using ctrl+x

Now write the following command in the terminal and press enter

  export EDITOR=NANO
  
Then write
  crontab -e 
and press enter 

@reboot /usr/sbin/dataLogger.sh

Save and close it by pressing ctrl+x

Now issue reboot command by writing 
  reboot
in the terminal and press enter. 

From now onwards every packets information will be stored inside the SD card. 
