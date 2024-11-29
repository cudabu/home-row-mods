# Kanata

---

This directory contains the kanata configuration for MacOS, as well as launchctl configuration to enable this to run as a LaunchAgent or LaunchDaemon.

To do so, make some modifications ot the launch configuration or create your own named `com.example.kanata.plist`

You'll need to replace the label string and the path to kanata in the plist file. 

```
Test
```

Then  copy the plist file to the LaunchDaeon folder:

`sudo cp ./io.cudabu.kanata.plist /Library/LaunchDaemons/`

Then load using:

```
sudo launchctl load /Library/LaunchDaemons/io.cudabu.kanata.plist
sudo loaunchctl start io.cudabu.kanata
```
