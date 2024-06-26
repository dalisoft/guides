# Xiaomi Mi Curved 34"

Settings of pictures, audio and more

## Tools

- <http://www.lagom.nl/lcd-test>
- <https://www.eizo.be/monitor-test>
- <https://webkit.org/blog-files/color-gamut/comparison.html>

## Useful tools

- <https://www.epaperpress.com/monitorcal>
- <https://www.w4zt.com/screen>
- <https://www.photofriday.com/info/calibrate>
- <https://www.drycreekphoto.com/Learn/Calibration/monitor_black.htm>
- <https://webkit.org/blog-files/color-gamut>

## Profiles

- <https://drive.usercontent.google.com/download?id=1fA6XK3SpekGPCI2ceORlqJRkAK0mLts0>

## Recommendations

- Use DisplayPort interface to connecting to your device
- Please use `3440x1440@120` mode for best expierence with less flickering issue
- Please use `RGB 8-bit Full` mode from **Nvidia Control Panel** or alternative control

## macOS Recommended Profiles

Download [ICC Profile](#profiles) and put into `~/Library/ColorSync/Profiles`
to get correct profiles. It's recommended for **Author-recommended settings**

or choose by order of recommendation

1. Use "Mi Curved Monitor" if **available**
2. sRGB IEC61966-2.1
3. Rec. ITU-R BT.709-5

or you don't find out any good variant, choose **Colour LCD** profile

## Windows Recommended Profiles

Download [ICC Profile](#profiles) and use that.
to get correct profiles. It's recommended for **Author-recommended settings**

### NVidia Control Panel

#### 3D Settings → Manage 3D Settings

| Name                  | Value             | Kind   | Description                 |
| --------------------- | ----------------- | ------ | --------------------------- |
| Power Management Mode | Adaptive          | Global | Helps with performance/idle |
| Monitor Technology    | G-SYNC compatible | Global | Helps reduce screen tearing |
| Low latency Mode      | Ultra             | Global | Helps with V-SYNC           |
| Triple buffering      | Off               | Global | Offloads GPU +1 frame       |
| Vertical Sync         | On                | Global | Helps with smoothness       |

#### Display → Change resolutions

Choose **NVIDIA color settings** and also select `120hz` mode to match within bandwidth

| Name                 | Value            |
| -------------------- | ---------------- |
| Desktop color depth  | Highest (32-bit) |
| Output color depth   | 8 bpc            |
| Output color format  | RGB              |
| Output dynamic range | Full             |

---

## Bri/Con

| Option             | 200 nits | 120 nits | 100 nits |
| ------------------ | -------- | -------- | -------- |
| Brightness         | 70       | -        | -        |
| Dynamic Brightness | Off      | Off      | Off      |
| Black Level        | 50       | 50       | 50       |
| Contrast           | 65       | 65       | 65      |
| DCR                | Off      | Off      | Off      |

---

### Picture

- Color Temprature — **Warm**
- Hue - **50**
- Saturation - **45**
- Gamma - **2.2**
- Aspect Ratio - **\[Default\]**

---

### PQ Settings

- Sharpness — **50**
- Response Time - **Off**
- Noise Reduction - **Off**
- Motion Response Time - **\[Default\]**

---

### Smart Mode

Choose **Standard**

---

### Window Settings

Author of this guide using **Single window** but you can use whatever you want

---

## Settings

- Language — English **select for yourself**
- Audio Source — **your current Input**
- Volume — **100**
- FreeSync Premium — **On**
