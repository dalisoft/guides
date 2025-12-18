# LG 27UK850-W

Settings of pictures, audio and more

## Universal tools

| Priority | Kind     | Purpose          | Link                                                                |
| -------- | -------- | ---------------- | ------------------------------------------------------------------- |
| 1        | Test     | Pixels, Colors   | <http://www.lagom.nl/lcd-test>                                      |
| 1        | Test     | Pixels, Colors   | <https://www.eizo.be/monitor-test>                                  |
| 2        | Test     | Color gamut      | <https://webkit.org/blog-files/color-gamut/comparison.html>         |
| 2        | Test     | Color gamut      | <https://webkit.org/blog-files/color-gamut>                         |
| 2        | Test     | Contrast         | <https://www.photofriday.com/info/calibrate>                        |
| 2        | Test     | Black color      | <https://www.drycreekphoto.com/Learn/Calibration/monitor_black.htm> |
| 4        | Guide    | Calibration      | <https://www.epaperpress.com/monitorcal>                            |
| 4        | Test     | Guide            | <https://www.w4zt.com/screen>                                       |
| -        | Resource | Monitor profiles | <https://tftcentral.co.uk/articles/icc_profiles>                    |

## Monitor-specific

| Kind   | Purpose                  | Link                                                                                      |
| ------ | ------------------------ | ----------------------------------------------------------------------------------------- |
| Review | Calibration, correctness | <https://www.rtings.com/monitor/reviews/lg/27uk650-w>                                     |
| Review | Capabilities             | <https://www.tomshardware.com/reviews/lg-27uk850-gaming-monitor,5708-2.html>              |
| Review | Capabilities             | <https://settingslab.com/lg-27uk650-calibration-settings>                                 |
| File   | **Monitor profile**      | <https://www.rtings.com/images/reviews/monitor/lg/27uk650/27uk650-rtings-icc-profile.icm> |

## Recommendations

- Use USB-C / Type-C interface to connecting to your device
- On a macOS, please use `2560x1440@2` scale mode for best expierence for 27"

## macOS Recommended Profiles

Download [ICC/Monitor Profile](#monitor-specific) and put into `~/Library/ColorSync/Profiles`
to get correct profiles. It's recommended for **Author-recommended settings**

or choose by order of recommendation

1. Use "LG HDR 4K" if **available**
2. sRGB IEC61966-2.1
3. Display P3
4. Rec. ITU-R BT.2020-1 (monitor profile)
5. Rec. ITU-R BT.709-5

or you don't find out any good variant, choose **Colour LCD** profile

---

## Picture

- Picture Mode — Custom

### Picture → Picture Adjust

| Option      | 200 nits | 120 nits | 100 nits |
| ----------- | -------- | -------- | -------- |
| Brightness  | 36       | 24       | 17       |
| Contrast    | 67       | 67       | 67       |
| Sharpness   | 50       | 50       | 50       |
| Super Res+  | Off      | Off      | Off      |
| Black Level | High     | High     | High     |
| DFC         | Off      | Off      | Off      |

### Picture → Game Adjust

- Response Time — Faster (for gaming) and/or Off (for coding)
- FreeSync - Extended
- Black Stabilizer - **50** (or choose your ideal value)

### Picture → Color Adjust

This settings get from <https://rtings.com>

| Option     | 200 nits        | 125 nits        | 100 nits        |
| ---------- | --------------- | --------------- | --------------- |
| Gamma      | Mode 4          | Mode 4          | Mode 4          |
| Color Temp | Custom          | Custom          | Custom          |
| Red        | 46              | 46              | 46              |
| Green      | 50              | 50              | 50              |
| Blue       | 48              | 48              | 48              |
| Six Color  | **\[Default\]** | **\[Default\]** | **\[Default\]** |

---

## Sound

- Volume — 10 (later you can control)
- MaxxAudio — On

---

## General

- Language — English **select for yourself**
- SMART ENERGY SAVING — Off
- Power LED — Off
- Automatic Standby — Off
- DisplayPort Version — **v1.2** or v1.4
- HDMI UHD Deep Color — On
- Buzzer — Off
- OSD Lock — Off
- OSD Size — Small
- Deep Sleep Mode — Off
