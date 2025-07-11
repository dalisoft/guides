# BIOS Configs for Hackintosh

> [!WARNING]
> This settings will not be updated anymore. Since 2022 i am own Macbook Pro M1 Max 16"

## Hardware lists

| Kind        | Vendor        | Model                               | Firmware |
| ----------- | ------------- | ----------------------------------- | -------- |
| CPU         | Intel         | i9-9900K                            | -        |
| GPU         | Sapphire      | RX 470 Nitro+                       | -        |
| Motherboard | Gigabyte      | Intel Z390 AORUS Pro Wi-Fi          | F12k     |
| CPU Cooler  | Cooler Master | MasterLiquid ML240 RGB              | -        |
| RAM         | Crucial       | Ballistix DDR4-3000CL15 16GB\*4 Kit | -        |
| SSD         | Samsung       | 970 Evo 500GB                       | 2B2QEXE7 |
| SSD         | Samsung       | 970 Evo+ 500GB                      | 2B2QEXM7 |
| HDD         | Toshiba       | 4TB 7200RPM HDD                     | -        |
| PSU         | CoolerMaster  | V1200 80+ Platinum                  | -        |
| Case        | Gamdias       | Athena M2 ELite Mesh                | -        |
| Webcam      | Logitech      | C930c Full HD                       | -        |
| Keyboard    | Logitech      | MK470 Slim                          | -        |
| Monitor     | LG            | UK850-W 4K                          | -        |
| Adapter     | Fenvi         | T-919 Wi-Fi/BT Adapter              | -        |

## Tweaker configurations

### Tweaker » CPU Configuration

- Enhanced Multi-Core Performance — Disabled
- IGP Ratio — Auto

### Tweaker » CPU Configuration » Advanced CPU Settings

- CPU Over Temperature Protection — 95C
- FCLK Frequency for Early Power On — 1Ghz
- Hyper-Threading Technology — Enabled
- No. Of CPU Cores Enabled — Auto
- VT-d — Enabled
- Intel(R) Speed Shift Technology — Disabled
- CPU Thermal Monitor — Disabled
- Ring to Core offset (Down Bin) — Disabled
- CPU EIST Function — Disabled
- Each To Halt (RTH) — Disabled
- Energy Efficient Turbo — Disabled
- Voltage Optimization — Disabled
- Hardware Prefetcher — Auto
- Adjacent Cache Line Prefetch — Auto
- Intel(R) Turbo Boost Technology — Disabled
- CPU Flex Ratio Override — Disabled
- CPU Flex Ratio Settings — \[default value\]
- Frequency Clipping TVB — Disabled
- Voltage reduction initiated TVB — Disabled
- Active Turbo Ratios — Disabled
- C-States Control — Disabled
- Turbo Power Limits — Disabled
- Turbo Per Core Limit Control — Disabled

### Tweaker » CPU Voltage

- CPU Core — Auto ([see cpu profiles](#cpu-profiles), example, **48**)
- Dynamic Vcore(DVID) — Auto
- SVID offset — Disabled
- BCLK Adaptive Voltage — Auto
- CPU Graphics Voltage (VAXG) — Auto

### Tweaker » Memory Voltage

- DRAM Voltage (CH A/B) — Auto ([see memory profiles](#memory-profiles), example, **1.350V**)
- CPU VCCIO — Auto ([see memory profiles](#memory-profiles), example, **1.100V**)
- CPU System Agent Voltage — Auto ([see memory profiles](#memory-profiles), example, **1.150V**)
- VCC Sustained — Auto
- VCCPLL — Auto
- VCCPLL OC — Auto
- PCH Core — Auto

### Tweaker » Advanced Voltage Settings » CPU/VRM Settings

- CPU Internal AC/DC Load Line — Auto ([see cpu profiles](#cpu-profiles), example, **Auto**)
- CPU Vcore Loadline Calibration — Auto ([see cpu profiles](#cpu-profiles), example, **High**)

### Tweaker » Advanced Memory Settings

- Memory Multiplier Tweaker — Auto
- Channel Interleaving — Auto
- Rank Interleaving — Auto
- Realtime Memory Timing — Auto
- Memory Enhancement Settings — Auto

### Tweaker » Advanced Memory Settings » Memory Channels Timing

- CAS Latency — Auto ([see memory profiles](#memory-profiles), example, CL**15**-16-16-35)
- tRCD — Auto ([see memory profiles](#memory-profiles), example, CL15-**16**-16-35)
- tRP — Auto ([see memory profiles](#memory-profiles), example, CL15-16-**16**-35)
- tRAS — Auto ([see memory profiles](#memory-profiles), example, CL15-16-16-**35**)
- All other settings leave as — Auto

## Settings

### Settings » Platform Power

- Platform Power Management — Disabled
- PEG ASPM — Disabled
- PCH ASPM — **Disabled**
- DMI ASPM — Disabled
- AC BACK — Always Off
- ErP — Disabled
- Soft-Off by PWR-BTTN — Delay 4 sec.
- Resume by Alarm — Disabled
- Power Loading — Disabled
- CEC 2019 Ready — Disabled
- RC6(Render Standby) — Enabled

### Settings » IO Ports

- Initial Display Output — PCIe 1 Slot
- Internal Graphics — **Enabled**
- DVMT Pre-Allocated — 64M
- DVMT Total Gfx mem — 128MB
- Aperture Size — 256MB
- Wi-Fi — Disabled
- Audio Controller — Enabled
- Above 4G Decoding — Enabled
- Re-Size BAR Support — Auto
- PCH LAN Controller — Enabled
- Wake on LAN Enable — Disabled
- IOAPIC 24-119 Entries — Enabled

### Settings » IO Ports » USB Configuration

- Legacy USB Support — Auto
- XHCI Hand-off — Enabled
- USB Mass Storage Driver Support — Enabled
- Port 60/64 Emulation — Disabled

### Settings » IO Ports » Network Stack Configuration

- Network Stack — Disabled

### Settings » IO Ports » SATA and RST Configuration

- SATA Controllers — Enabled
- SATA Mode Selection — AHCI
- Aggressive LPM Support — Disabled
- SATA\[n\] Port — Enabled
- SATA\[n\] Hot Plug — Disabled

### Settings » IO Ports » Intel(R) Ethernet Connection

- NIC Configuration » Link Speed — Auto Negotiation
- NIC Configuration » Wake On LAN — Disabled

### Settings » Smart Fan 5/6

- CPU FAN — Configure manual or SILENT
- CPU OPT — Configure manual or SILENT
- Temperature Warning Control — CPU, 90C
- CPU Fan Fail Warning — Enabled

| Fan         | Temperature     | Sensor  | Speed            |
| ----------- | --------------- | ------- | ---------------- |
| CPU AIO     | -               | CPU     | Full Speed       |
| CPU-OPT AIO | 50-60-70-80-90C | CPU     | 20-40-60-80-100% |
| Rear Case   | 40-42-44-46-48C | VRM_MOS | 20-40-60-80-100% |
| Bottom      | 20-30-40-50     | HDD     | 0-30-60-90%      |
| GPU FAN     | 40-50-60-70-80C | GPU     | 20-40-60-80-100% |

### Settings » Miscellaneous

- LEDs in System Power On State — On
- LEDs in Sleep, Hibernation and Soft Off States — Off
- Intel Platform Trust Technology (PTT) — Disabled
- Software Guard Extensions (SGX) — Disabled
- Max Link Speed — Auto
- 3DMark01 Enhancement — Disabled

### Settings » Miscellaneous » Trusted Computing

- Security Device Support — **Disable**
- SHA-1 PCR Bank — Enabled
- SHA256 PCR Bank — Enabled
- Pending operation — None
- Platform Hierarchy — Enabled
- Storage Hierarchy — Enabled
- Endorsement Hierarchy — Enabled
- TPM2.0 UEFI Spec Version — TGG_2
- Physical Presence Spec Version — 1.3

## System Info

- System Language — English
- System Date — \[Please set\]
- System Time — \[Please set\]

## Boot

- Bootup NumLock State — On
- CFC Lock — Disabled
- Security Option — System
- Full Screen LOGO Show — Enabled
- Boot Option — \[change as you want\]
- Fast Boot — Disabled
- Mouse Speed — 1X
- Windows 8/10 Features — Other OS
- CSM Support — Disabled
- Preferred Operating Mode — Auto

### Boot » Secure Boot

- System Mode — Setup
- Secure Boot Enable — Disabled, Not Active
- Secure Boot Mode — Custom

## CPU Profiles

- Clocks - Core, AVX, Uncore. example, 48 is 4.8Ghz
- DC - AC/DC Calibration
- LLC - Load Line Calibration

| Name       | Clocks   | Voltage | DC   | LLC    | Comfort | Power Watt  | Overclock |
| ---------- | -------- | ------- | ---- | ------ | ------- | ----------- | --------- |
| **OC@1**   | 48/46/45 | 1.235V  | Auto | High   | Good    | 160W (100%) | 27%       |
| Power      | 48/46/44 | 1.200V  | Auto | High   | Good    | 145W (90%)  | 26%       |
| Underpower | 44/40/40 | 1.100V  | Auto | Medium | Best    | 100W (62%)  | 11%       |

## Memory profiles

See [voltage scaling](https://github.com/integralfx/MemTestHelper/blob/oc-guide/DDR4%20OC%20Guide.md#voltage-scaling) for better understanding how it works

- VCCSA - System Agent Voltage
- RWCL - Performance of Read, Write, Copy and Latency

| Name     | Clock | Voltage | Timings     | CR  | CPU VCCIO | CPU VCCSA | RWCL                |
| -------- | ----- | ------- | ----------- | --- | --------- | --------- | ------------------- |
| XMP-1    | 3000  | 1.340V  | 15-16-16-35 | 2   | 1.100V    | 1.150V    | -                   |
| **OC@1** | 3466  | 1.350V  | 16-18-18-42 | 2   | 1.150V    | 1.200V    | 42GB/45GB/42GB/60ns |
| OC@2     | 3733  | 1.430V  | 17-18-18-42 | 2   | 1.200V    | 1.250V    | -                   |

## FAQ

### Cold boot reboot few times

This may be caused by **CFG Lock** disabling and/or installing Hackintosh (OpenCore/Clover)

Try [this](https://forums.tomshardware.com/threads/z390-aorus-pro-cpu-and-dram-led.3673431/post-22123817) trick and it should help

### BIOS config resets

Try replace motherboard battery for time

### CPU fans works always

Please check **your Smart Fan** or **Load-line level**. One of these values cause this behavior

### PCI-E Wi-Fi/BT Card does not work

Please disable **PCH ASPM** at **Settings » Platform Power** for working any external PCI-E Wi-Fi/BT Card
