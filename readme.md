# Dell Optiplex 9020 Micro Hackintosh

## Audio

Realtek ALC3234 / ALC255

Kext(s): 
- [AppleAlc](https://github.com/acidanthera/AppleALC)
- [Lilu](https://github.com/acidanthera/Lilu)

Layout ID: 15

Config.plist for audio device:
```
...
<key>Devices</key>
<dict>
  <key>Properties</key>
  <dict>
    <key>PciRoot(0x0)/Pci(0x1b,0x0)</key>
    <dict>
      <key>AAPL,slot-name</key>
      <string>Internal</string>
      <key>device_type</key>
      <string>Audio device</string>
      <key>hda-gfx</key>
      <string>onboard-2</string>
      <key>layout-id</key>
      <integer>15</integer>
      <key>model</key>
      <string>8 Series/C220 Series Chipset High Definition Audio Controller</string>
    </dict>
  </dict>
<dict>
...
```

## Network

Intel I217LM PCI Express Gigabit

Kext(s):
- [IntelMausiEthernet](https://github.com/Mieze/IntelMausiEthernet)
