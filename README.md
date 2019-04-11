# wally
EEG acquisition using g.tec's API using MATALAB's App Designer. I know, not the
best choice structure-wize (single file and all), but makes gui design painless.

## requirements
 - MATLAB R2017b (later versions might also work)
 - g.tec's g.NEEDaccess and its MATLAB API
 - Windows 10 (due to API restrictions)
 - suported from the API eeg acquisition hardware 

## usage
 - run `Wally` from MATLAB after connecting the hardware
 - adjust parameters (remember to set a proper montage template, see
   `montage.txt`)
 - set an appropriate **Name** and **Folder** for filename and folder (rest of the *info* are
   saveds as metadata) 
 - press **Start EEG** to initialize the connection and view the data stream
 - when ready, press **Record Data**
 - once the "Record Data" is pressed again, the recorded strem will be saved
   with a filename and inside a folder corresponding the date and time of the acquisition
