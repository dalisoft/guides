# Wi-Fi Guides » Windows 10 Internet

See [here](https://www.drivereasy.com/knowledge/solved-windows-10-slow-internet-2/) for more information and tips & tricks.
From above guide, use only section 1, 4, 6 for better internet performance

1. Disable Large Send Offload / V2 for Ethernet and for Wi-Fi adapters if available (from Adapters Options)
2. Disable bandwidth reserve via `gpedit.msc`, see [guide](https://www.itechtics.com/limit-reservable-bandwidth/#limit-reservable-bandwidth-from-group-policy)
3. Disable Disable Peer to Peer Update / Delivery Optimization if you don't have any other running Windows 10/11 devices
4. Run commands:

```ps
netsh winsock reset
netsh int tcp set global autotuninglevel=normal
```

Now, please reboot your computer and enjoy good internet performance
