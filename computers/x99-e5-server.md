# BIOS Configs

## Universal tools

| Priority | Kind  | Purpose           | Link                                     | Min. Required      |
| -------- | ----- | ----------------- | ---------------------------------------- | ------------------ |
| 1        | Check | Sensors           | <https://www.hwinfo.com>                 |                    |
| 1        | Test  | Memory stability  | <https://github.com/CoolCmd/TestMem5>    | 3-cycle, 3-hour+   |
| 2        | Test  | Overall Stability | <https://www.aida64.com>                 | Full 3 hour+       |
| 2        | Test  | Overall Stability | <https://www.ocbase.com/occt/personal>   | Full 1 hour+       |
| 3        | Test  | Stress stability  | <https://www.numberworld.org/y-cruncher> | -                  |
| 3        | Test  | CPU stability     | <https://www.mersenne.org/download>      | All mode, 24 hour+ |

## Platform-specific

| Kind  | Purpose     | Link                                                                    |
| ----- | ----------- | ----------------------------------------------------------------------- |
| Check | RAM Timings | <https://www.reddit.com/r/overclocking/comments/z82lvj/comment/iybbj1x> |
| Guide | RAM         | <https://github.com/integralfx/MemTestHelper>                           |

## Hardware lists

| Kind        | Vendor       | Model                   | Firmware          |
| ----------- | ------------ | ----------------------- | ----------------- |
| CPU         | Intel        | E5-2696v3               | -                 |
| GPU         | Sapphire     | RX 470 Nitro+           | -                 |
| Motherboard | Huananzhi    | X99-F8 (NCT5567D-B)     | v5.10 (OC-unlock) |
| CPU Cooler  | -            | 6-heatpipe china cooler | -                 |
| RAM         | SK (Hynix)   | LRDIMM-2133 ECC 32GB\*8 | -                 |
| SSD         | Samsung      | 970 Evo 500GB           | 2B2QEXE7          |
| SSD         | Samsung      | 980 Pro 2TB             | 5B2QGXA7          |
| HDD         | WD           | RED Pro 20TB \* 4       | -                 |
| HDD         | WD           | RED Plus 18TB           | -                 |
| PSU         | CoolerMaster | V1200 80+ Platinum      | -                 |
| Case        | Fractal      | Meshify 2               | -                 |
| Webcam      | -            | -                       | -                 |
| Keyboard    | -            | Cheap keyboard+mice     | -                 |
| Monitor     | IMMER        | Full HD Curved 21.5"    | -                 |
| Adapter     | LR-Link      | 6880BT 10GbE PCI-E      | -                 |
| Adapter     | Intel        | 82575 2\*1GbE PCI-E     | -                 |

## Main

- System Language — English
- System Date — \[Please set\]
- System Time — \[Please set\]

## Advanced

### Advanced » ACPI Settings

- Enabled ACPI Auto Configuration — Disabled
- Enable Hibernation — Disabled
- ACPI Sleep State — Suspend Disabled
- Lock Legacy Resources — Disabled

### Advanced » NCT5532D Super IO Configuration

- Restore AC Power Loss — Power On

### Advanced » NCT5532D Super IO Configuration » Serial Port 1 Configuration

- Serial Port — Disabled

### Advanced » Hardware Monitor

Check your temperatures from there

### Advanced » Smart Fan Function

> This is only way to control all fans via BIOS. There Case Hub between CPU 4-pin and all fans

- CPU Smart FanMode — Manual
- Set value to **50** of **250** (20%)

### Advanced » Realtek PCIe GBE Family Controller (MAC::\[unique mac address\])

Check your LAN device information from there

### Advanced » PCI Subsystem Settings

- PCI Latency Timer — 32 PCI Bus Clocks
- PCI-X Latency Timer — 64 PCI Bus Clocks
- VGA Palette Snoop — Disabled
- PERR# Generation — Disabled
- SERR# Generation — Disabled
- Above 4G Decoding — Disabled
- SR-IOV Support — Disabled
- BME DMA Mitigation — Disabled

### Advanced » PCI Subsystem Settings » PCI Express Settings

- Relaxed Ordering — Disabled
- Extended Tag — Disabled
- No Snoop — Enabled
- Maximum Payload — Auto
- Extended Sync — Disabled
- Link Training Retry — 5
- Link Training Timeout (uS) — 1000
- Restore PCIE Registers — Disabled

### Advanced » PCI Subsystem Settings » PCI Express Gen 2 Settings

- Completion Timeout — Default
- ARI Forwarding — Disabled
- AtomicOp Requester Enable — Disabled
- AtomicOp Egress Blocking — Disabled
- IDO Request Enable — Disabled
- IDO COmpletion Enable — Disabled
- LTR Mechanism Enable — Disabled
- End-to-End TLP Prwfix Blocking — Disabled
- Clock Power Management — Disabled
- Compliance SOS — Disabled
- Hardware Autonomous Width — Enabled
- Hardware Autonomous Speed — Enabled

### Advanced » Network Stack Configuration

- Network Stack — Disabled
- Lan Wake up Control — Enabled

### Advanced » CSM Configuration

- CSM Support — Disabled

Before Disabled configurations:

- GateA20 Active — Upon Request
- Boot option filter — UEFI only
- Network — Do not launch
- Storage — UEFI
- Video — UEFI
- Other PCI devices — UEFI

### Advanced » NVMe Configuration » \[NVMe device name\]

No entries here, seems bug

### Advanced » USB Configuration

- Legacy USB Support — Auto
- XHCI Hand-off — Enabled
- EHCI Hand-off — Disabled
- USB Mass Storage Driver Support — Enabled
- Port 60/64 Emulation — Disabled
- USB transfer time-out — 20 sec
- Device reset time-out — 20 sec
- Device power-up delay — Auto

## IntelRCSetup

### IntelRCSetup » Processor Configuration

- Hyper-Threading \[ALL\] — Enable
- Check CPU BIST Result — Disable
- Monitor/Mwait — Enable
- Enable Intel TXT Support — Disable
- VMX — Enable
- Enable VMX — Disable
- Lock Chipset — Enable
- MSR Lock Control — Enable
- PPIN Control — Unlock/Enable
- DEBUG INTERFACE — Disable
- Hardware Prefetcher — Enable
- Adjacent Cache Prefetch — Enable
- PCU Streamer Prefether — Enable
- DCU IP Prefetcher — Enable
- DCU Mode — 32KB 8Way without ECC
- Direct Cache Access (DCA) — Auto
- DCA Prefetch Delay — 32
- X2APIC — Disable
- AES-NI - Enable
- Down Stream PECI - Enable
- IIO LLC Ways \[19:9\] (Hex) — 0
- QLRU Config \[63:32\] (Hex) — 0
- QLRU Config \[31:0\] (Hex) — 0
- SMM Save State — Disable
- Targeted Smi — Disable

### IntelRCSetup » Processor Configuration » Per-Socket Configuration » CPU Socket \[n\] Configuration

- Cores Enabled — 0
- IOT Cfg Cbo Bitmap(Hex) — 0

### IntelRCSetup » Advanced Power Management Configuration

- Power Technology — Custom
- Config TDP — Disable
- IOTG Settings — Disable

### IntelRCSetup » Advanced Power Management Configuration » CPU P State Control

- EIST (P-states) — Enable
- Turbo Mode — Enable
- P-state coordination — HW_ALL
- SPD — Disable
- PL2_SAFETY_NET_ENABLE — Enable
- Boot performance — Max Performance

### IntelRCSetup » Advanced Power Management Configuration » CPU C State Control

- C2C3TT — 0
- Package C State limit — C0/C1 state
- CPU C3 report — Disable
- CPU C6 report — Disable

### IntelRCSetup » Advanced Power Management Configuration » CPU T State Control

- ACPI T-States — Disable

### IntelRCSetup » Advanced Power Management Configuration » CPU - Advanced PM Tuning » Energy Perf BIAS

- Energy Performance Tuning — Disable
- Energy Performance BIAS setting. — Performance
- Power/Performance Switch — Enabled
- Workload Configuration — I/O sensitive
- Averaging Time Window — 23
- P0 TotalTimeThreshold Low — 35
- P0 TotalTimeThreshold High — 58

### IntelRCSetup » Advanced Power Management Configuration » SOCKETT RAPL Config

- FAST_RAPL_NSTRIKE_PL2_DUTY_CYCLE — 64
- Turbo Pwr Limit Lock — Disable
- Long Pwr Limit Ovrd — Enable
- Long Dur Pwr Limit — 0
- Long Dur Time Window — 1
- Pkg Clmp Lim1 — Below P1
- Short Dur Pwr Limit En — Enable
- Short Dur Pwr Limit — 0
- Pkg Clmp Lim2 — Below P1

### IntelRCSetup » Advanced Power Management Configuration » DRAM RAPL Configuration

- DRAM RAPL Baseline — DRAM RAPL Mode 0
- Override BW_LIMIT_TF — 1
- DRAM RAPL Extended Range — Enable

### IntelRCSetup » Common RefCode Configuration

- MMCFG Base — 2G
- MMIOHBase — 56T
- MMIO High Size — 256G
- Isoc Mode — Auto
- MeSeg Mode — Auto
- Numa — Enable

### IntelRCSetup » QPI Configuration » QPI General Configuration

- Degrade Precedence — Topology Precedence
- Link Frequency Select — Auto
- Link L0p Enable — Auto
- Link L1 Enable — Enable
- Legacy VGA Socket — 0
- MMIO P2P Disable — Disable
- E2E Parity Enable — Disable
- COD Enable — Auto
- Early Snoop — Auto
- Home Dir Snoop with IVT- Style OSB — Auto
- QPI Debug Print Level — All

### IntelRCSetup » QPI Configuration » QPI General Configuration » QPI Status

Check your QPI data from there

### IntelRCSetup » QPI Configuration » QPI Per Socket Configuration » CPU \[n\]

- Bus Resources Allocation Ratio — 1
- IO Resources Allocation Ratio — 1
- MMIOL Resources Allocation Ratio — 1
- IIO Disable - no

### IntelRCSetup » Memory Configuration

- Enforce POR — PPR Disabled
- PPR Error Injection Test — Disabled
- Memory Frequency — 2133
- PROMOTE WARNINGS — Enabled
- Halt on Mem Training Error — Auto
- ECC Support — Auto
- Enhanced Log Parsing — Enabled
- BSSA Module Loader — Auto
- Backside RMT — Auto
- Rank Multiplication — Auto
- LRDIMM Module Delay — Auto
- MemTest — Auto
- MemTestLoops — 1
- Dram Maintenance Test — Auto
- Dram Maintenance Test Inversion — Up Direction
- Dram Maintenance Test Enable — Disabled
- Dram Maintenance Test Repetitions — 3
- Dram Maintenance Swizzle Enabling — Enabled
- CEC MD WA Mask — Auto
- Memory Type — UDIMMs and RDIMMs
- Crank Refresh Enabling — Enabled
- Rank Margin Tool — 1
- RMT Pattern Length — 10
- CMD Pattern Length — Auto
- BIT Per BIT — Auto
- Training Result Offset Config — Auto
- Attempt Fast Boot — Auto
- Attempt Fast Cold Boot — Auto
- RMT On Cold Fast Boot — Auto
- BDAT — Disabled
- Data Scrambling — Auto
- Allow SBE During Training — Auto
- CAP ERR FLOW Feature Control — Auto
- Scrambling Seed Low — 41003
- Scrambling Seed High — 54165
- Enable RDR — Auto
- MC DDL Threshold — 0
- DLL Reset Test — Disabled
- ODT Mode — 0
- Normal Operation Duration — 1024
- Number of Sparing Transaction — 4
- PSMI Support — Disabled
- C/A Parity Enable — Auto
- SMB Clock Frequency — Auto

### IntelRCSetup » Memory Configuration » Memory Thermal

- Set Throttling Mode — CLTT
- OLTT Peak BW % — 50
- Phase Shedding — Auto
- Memory Power Savings Mode — Auto
- MDLL Off — Auto
- MEMHOT Throttling Mode — Input-only
- Mem Electrical Throttling — Disabled

### IntelRCSetup » Memory Configuration » Memory Thermal » Memory Power Savings Advanced Options

- CK in SR — Auto

### IntelRCSetup » Memory Configuration » Memory Timings & Voltage Override

- DIMM profile — MANUAL
- Memory Frequency — Auto ([see memory profiles](#memory-profiles), example, **2133**)
- Memory Voltage — Auto ([see memory profiles](#memory-profiles), example, **120**)
- Command Timing — 2N
- Refresh Rate — 0
- CAS Latency — Auto ([see memory profiles](#memory-profiles), example, CL**15**-15-15-36)
- tRP — Auto ([see memory profiles](#memory-profiles), example, CL15-**15**-15-36)
- tRCD — Auto ([see memory profiles](#memory-profiles), example, CL15-15-**15**-36)
- tRAS — Auto ([see memory profiles](#memory-profiles), example, CL15-15-15-**36**)
- tWR — 18
- tRFC — 374 (LRDIMM safe values 350-400)
- tRRD — 7
- tRTP — 9
- tWTR — 9
- tFAW — 36
- tRC — 51 (tRAS + tRP)
- tCWL — 15 (should match tCL)

### IntelRCSetup » Memory Configuration » Memory Map

- Socket Interleave Below 4GB — Disable
- Channel Interleaving — Auto
- Rank Interleaving — Auto
- IOT Memory Buffer Reservation — 0
- A7 Mode — Enable

### IntelRCSetup » Memory Configuration » Memory RAS Configuration

- RAS Mode — Disable
- Lockstep x4 DIMMs — Auto
- Memory Rank Sparing — Disabled
- Correctable Error Threshold — 32767
- Leaky bucket low bit — 40
- Leaky bucket high bit — 41
- DRAM Maintenance — Auto
- Patrol Scrub — Enable
- Patrol Scrub Interval — 24
- Demand Scrub — Enable
- Device Tagging — Disabled
- Memory Power Management — Disable

### IntelRCSetup » IIO Configuration

- PCIE Train by BIOS — yes
- PCIe Hot Plug — Disable
- PCIE ACPI Hot Plug — Disable
- EV DFX Features — Disable
-
- TX EQ WA — Enable
- DMI Vc1 Control — Enable
- DMI Vcp Control — Enable
- DMI Vcm Control — Enable
- VC0 No-Snoop Configuration — Disable
- Gen3 Phase3 Loop Count — 16
- Skip Halt on DMI Degradation — Disable
- Power down unused port — yes
- SLD WA Revision — Auto
- Rx Clock WA — Disable
- PCI-E ASPM (Global) — L1 only
- PCIE Stop & Scream Support — Disable
- Snoop Response Hold off — 6

### IntelRCSetup » IIO Configuration » IIO0 Configuration

- IOU2 (IIO PCIe Port 1) — x4x4
- IOU0 (IIO PCIe Port 2) — x16
- IOU1 (IIO PCIe Port 3) — x16
- No PCIe port active ECO — PCU Squelch exit ig...
-
- IOU0 Non-Posted Prefetch — Disable
- IOU1 Non-Posted Prefetch — Disable
- IOU2 Non-Posted Prefetch — Disable

### IntelRCSetup » IIO Configuration » IIO0 Configuration » Socket 0 PcieD00F0 - Port 0/DMI

To-do, fill later

### IntelRCSetup » IIO Configuration » IIO0 Configuration » Socket 0 PcieD01F0 - Port 1A

To-do, fill later

### IntelRCSetup » IIO Configuration » IIO0 Configuration » Socket 0 PcieD01F1 - Port 1B

To-do, fill later

### IntelRCSetup » IIO Configuration » IIO0 Configuration » Socket 0 PcieD02F0 - Port 2A

To-do, fill later

### IntelRCSetup » IIO Configuration » IIO0 Configuration » Socket 0 PcieD03F0 - Port 3A

To-do, fill later

### IntelRCSetup » IIO Configuration » IOAT Configuration

- Enable IOAT — Disable
- No Snoop — Disable
- Disable TPH — Enable
- Relaxed Ordering — Disable
- Apply BOX CBDMA ECO — no

### IntelRCSetup » IIO Configuration » IIO General Configuration

- IIO IOAPIC — Enable

### IntelRCSetup » IIO Configuration » Intel VT for Directed I/O (VT-d)

- VTD Azalea VCp Optimizations — Disable
- Intel VT for Directed I/O (VT-d) — Enable
- ACS Control — Enable
- Interrupt Remapping — Enable
- Coherency Support (Non-Isoch) — Enable
- Coherency Support (Isoch) — Enable

### IntelRCSetup » PCH Configuration » PCH Devices

- Board Capability — DeepSx
- DeepSx Power Policies — Disabled
- GP27 Wake From DeepSx — Disabled
- SMBUS Device — Enabled
- PCH Server Error Reporting Mode — Disabled
- PCH Display — Enabled
- Serial IRQ Mode — Quiet
- External SSC Enable - CK420 — Disabled
- PCH CRID — Disabled

### IntelRCSetup » PCH Configuration » PCI Express Configuration

- PCI-E ASPM Support (Global) — L1 Only
- PCIE Clock Gating — Enabled
- DMI Link Extended Sync Control — Disabled
- Stop and Scream — Disabled
- Expanded SPI TPM Transaction Length — Disabled
- Subtractive Decode — Disabled

### IntelRCSetup » PCH Configuration » PCI Express Configuration » PCI Express Root Port \[n\]

- PCI Express Root Port \[n\] — Enabled
- L1 Substates — L1.1 & L.12
- - PME SCI — Disabled
- - Hot Plug — Disabled
- PCIe Speed — Auto
- - PME Interrupt — Disabled
- Extra Bus Reserved — 0
- Reserved Memory — 10
- Prefetchable Memory — 10
- Reserved I/O — 0

### IntelRCSetup » PCH Configuration » PCH SATA (or sSATA) Configuration

- SATA (or sSATA) Controller — Enabled
- Configure SATA (or sSATA) as — AHCI
- SATA (or sSATA) test mode — Disabled
-
- SATA (or sSATA) AHCI LPM — Disabled
- SATA (or sSATA) Port \[n\]
- - Port \[n\] — Enabled
- - Hot Plug — Disabled
- - Configure as SATA (or sSATA) — Disabled
- - Spin Up Device — Disabled
- - SATA (or sSATA) Device Type — Hard Disk Drive

### IntelRCSetup » PCH Configuration » PCH SATA (or sSATA) Configuration » SATA Mode options

- SATA HDD Unlock — Enabled
- SATA Led locate — Enabled

### IntelRCSetup » PCH Configuration » USB Configuration

- USB Precondition — Disabled
- xHCI Mode — Smart Auto
- Trunk Clock Gating (BTCG) — Enabled
- USB Ports Per-Port Disable Control — Disabled
- XHCI Idle L1 — Enabled
- USB XHCI s755 WA — Enabled
- USB XHCI Interrupt Remap WA — Enabled

### IntelRCSetup » PCH Configuration » Security Configuration

- GPIO Lockdown — Enabled
- RTC Lock — Enabled
- BIOS Lock — Disabled
- Host Flash Lock-Down — Enabled
- GbE Flash Lock-Down — Enabled

### IntelRCSetup » PCH Configuration » Azalia Configuration

- Azalia — Enabled
- - Azalia Docking Support Enable — Disabled
- - Azalia PME Enable — Disabled

### IntelRCSetup » PCH Configuration » Platform Thermal Configuration

- PCH Thermal Device — Disabled
- Alert Enable Lock — Disabled

### IntelRCSetup » OverClocking Feature

- OverClocking Feature — Enabled
- Filter Pll — Disabled
- Adjust Pll — Disabled
- Change PllTrim Value — 0
- Change PllTrim Prefix — \[+\]
- TJ-Max offset — 0
- SfrTrim Optin — Disabled

### IntelRCSetup » OverClocking Feature » Processor

- Core Max OC Ratio — 0
- Core Voltage Mode — Adaptive ([see cpu profiles](#cpu-profiles), example, **Adaptive**)
- Core Extra Turbo Voltage — 0
- Core Voltage Offset — 0 ([see cpu profiles](#cpu-profiles), example, **50**)
- Offset Prefix — \[-\] ([see cpu profiles](#cpu-profiles), example, **-**)
- VCCU Voltage Offset — 0
- Offset Prefix — \[+\]
- AVX2 Negative Offset — 0

### IntelRCSetup » OverClocking Feature » CLR/Ring

- CLR Max OC Ratio — 0
- CLR Min Ratio — 12
- CLR Voltage Mode — Adaptive
- CLR Extra Turbo Voltage — 0
- CLR Voltage Offset — 0
- - Offset Prefix — \[+\]

### IntelRCSetup » OverClocking Feature » Uncore

- Uncore Voltage Offset — 0 ([see memory profiles](#memory-profiles), example, **100**)
- Offset Prefix — \[+\] ([see memory profiles](#memory-profiles), example, **+**)
- Vccio Voltage Control — 1.0590V ([see memory profiles](#memory-profiles), example, **1.0590V**)

### IntelRCSetup » OverClocking Feature » SVID/FIVR

- SVID Support — Enabled
- SVID Voltage Override — 0
- CPU Vccin Voltage Level — 359
- FIVR Faults — Enabled
- FIVR Efficiency Management — Enabled

### IntelRCSetup » Miscellaneous Configuration

- Fan PWM Offset — 0
- PCIe Max Read Request Size — 4096B
- PCIe Latency Tolerance Reporting — Enable
- PCI Minimum Secondary Bus Number — 1
- PCIe Extended Tag Enable — Enable
- PCIe AtomicOp Request Support — Disable
- Breakpoint Type — None
- BIOS Guard — Disabled
- Serial Debug Message Level — Disable
- Trace Messages — Disabled
- Training Messages — Disabled
- RC Promote Warnings — Enabled
- RC Promote MRC Warnings — Enabled
- Active Video — Offboard Device
- TargetVGA — Vga From CPU 0
- RTC Wake system from S5 — Disable

### IntelRCSetup » Server ME Debug Configuration » Server ME General Configuration

- ME Initialization Complete Timeout — 2
- Custom HPET timer for SPS HECI Wai — 1

### IntelRCSetup » Server ME Debug Configuration » Server ME General Configuration » Override ICC Clock Enables

- Override ICC Clock Enables — Disabled

### IntelRCSetup » Server ME Debug Configuration » NM Configuration

- Cores Disable Override — Disabled
- - Cores To Disable — 0
- Power Measurement Override — Disabled
- - Power Measurement — Disabled
- Hardware Change Override — Disabled
- - Hardware Changed — no

### IntelRCSetup » Reserve Memory

- Reserve Memory Range — Disabled
- Start Address — 100000
- Reserve TAGEC Memory — Disabled

## Security

- Administrator Password
- User Password

### Security » Secure Boot menu

- Secure Boot — Disabled
- Secure Boot Mode — Custom

## Boot

- Setup Prompt Timeout — 1
- Bootup NumLock State — On
- Fast Boot — Disabled
- Show Full Logo — Disabled

## CPU Profiles

| Name / Param | Core Voltage (Mode, Offset, Prefix) | Comfort | Power Watt  | Relative performance |
| ------------ | ----------------------------------- | ------- | ----------- | -------------------- |
| Default      | Adaptive, 50, `-`                   | Good    | 145W (100%) | 100%                 |

## Memory profiles

See [voltage scaling](https://github.com/integralfx/MemTestHelper/blob/oc-guide/DDR4%20OC%20Guide.md#voltage-scaling) for better understanding how it works

| Name / Param      | Clock | Voltage      | Timings     | VccIo Voltage Control | Uncore Voltage Offset |
| ----------------- | ----- | ------------ | ----------- | --------------------- | --------------------- |
| JEDEC-DDR-2133 ⚠️ | 2133  | 1.200V (120) | 15-15-15-36 | 1.0590V               | \[+\] 0 (1.000V)      |
| **M-UV@1**        | 2133  | 1.200V (120) | 15-15-15-36 | 1.0590V               | \[+\] 100 (1.110V)    |

## Links

- <https://github.com/Koshak1013/HuananzhiX99_BIOS_mods>
- <https://github.com/miyconst/Mi899>
- <https://github.com/markkpa/x99-t8d-and-x99-f8d-Opencore-Hackintosh>
- <https://github.com/felipemeamaral/EFI-X99-F8-OPENCORE>
- <https://e5450.com/socket-2011-3/huananzhi-x99-f8/>
- <https://e5450.com/socket-2011-3/e5-2600-v3/xeon-e5-2696-v3/>
- <https://e5450.com/vopros-otvet/>
- <https://www.reddit.com/r/homelab/comments/1gvysj9/is_huananzhi_x99_f8_with_e5_2680_v4_with_rtx_4060/>
- <https://www.reddit.com/r/homelab/comments/1ck0p6a/x99_huananzhi_f8d_plus_server_build/>
- <https://linustechtips.com/topic/1316242-hunanazhi-x99-f8/>
- <https://linustechtips.com/topic/1480885-thread-for-those-of-you-with-chinese-x99x79x58etc-boards/>
- <https://forums.overclockers.ru/viewtopic.php?f=1&t=602922>
- <https://www.diy-laptoprepair.com/forum/fix-HUANANZHI-X99-F8-repair-guide-schematics.html>
- <https://vlab.su/viewtopic.php?f=44&t=135727>
