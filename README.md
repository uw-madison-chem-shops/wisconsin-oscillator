# Wisconsin Oscillator

Small, inexpensive, low power device for powering ion guiding devices.

The Wisconsin Oscillator has been published in the Journal of the American Society for Mass Spectrometry. Please read our article to learn more about the motivation behind the Wisconsin Oscillator and to see examples the circuit being used to guide ions through a custom spectrometer.

> [The Wisconsin Oscillator: A Low-Cost Circuit for Powering Ion Guides, Funnels, and Traps](https://doi.org/10.1021/jasms.1c00247) Kregel, S. J.; Thompson, B. J.; Nathanson, G. M.; and Bertram, T. H. _Journal of the Americian Socieity for Mass Spectrometry_ (2021)

## PCB

Printed circuit board fabrication files can be found in the gerber directory.
PCB images generated with [tracespace](https://github.com/tracespace/tracespace) follow.

<img src="./Wisconsin Oscillator-.top.svg" width="100%"/>
<img src="./Wisconsin Oscillator-.bottom.svg" width="100%"/>

## Bill of Materials

C1 and L1/L2 can be changed to control the amplitude and frequency of the oscillator, as described in the next section.
All other parts are listed below.

| reference         | manufacturer | part number                       |  vendors |
| :---------------- | :----------- | :-------------------------------- | :------- |
| C2                | various      | 2.2 pF ceramic, 1kV, 1206 package | [Mouser](https://www.mouser.com/ProductDetail/Walsin/1206N2R2C102CT?qs=ZrPdAQfJ6DMo6D%2FvZxBqfw%3D%3D) |
| C3, C4            | various      | 4.7 nF ceramic, 1kV, 1206 package | [Mouser](https://www.mouser.com/ProductDetail/Kyocera-AVX/1206AC472MAT1A?qs=%2Fha2pyFaduhzfYpjb5v9%2FX3y5jlWBFFWEQhcr6uCzhXR56xULseKBA%3D%3D) |
| C5                | various      | 100 uF electrolytic               | [Mouser](https://www.mouser.com/ProductDetail/CDE-Illinois-Capacitor/107CKE025MEM?qs=3tP%252BN51vMXeOVuB%252BkBNQFQ%3D%3D) |
| C6                | various      | 3.3 nF ceramic, 1206 package      | [Mouser](https://www.mouser.com/ProductDetail/Samsung-Electro-Mechanics/CL31C332JBFNNNE?qs=%2Fha2pyFaduhPzWFCM51KQEWJ40%252BY2tgediDfDzBWCkuVgZGDNgIATFe5%252BxLhkX0v) |
| J1, J2, J3, J4    | Molex        | 22-23-2021                        | [Mouser](https://www.mouser.com/ProductDetail/Molex/22-23-2021?qs=%2Fha2pyFaduiHQLs56YZXs3AkvtRoBprDw5MnVZuMKr8%3D) |
| R1                | various      | 6.8 kOhm, 1206 package            | [Mouser](https://www.mouser.com/ProductDetail/Panasonic/ERJ-8ENF6801V?qs=%2Fha2pyFaduh7VP2GfmkMxHOCEV8rtbSgRKUNEyrhBWx1%252BvfOW9YFPw%3D%3D) |
| R2, R3            | varous       | 1 Mohm, 1206 package              | [Mouser](https://www.mouser.com/ProductDetail/Vishay-Dale/CRCW12061M00FKEAC?qs=%2Fha2pyFaduh62bXGafpVtEasjFvzCXuSdredFavJVIq3S3FLHV7HVu%2Fl5Mz9wsE3) |
| U1, U2, U3, U4    | TI           | CD74AC04M96                       | [Mouser](https://www.mouser.com/ProductDetail/Texas-Instruments/CD74AC04M96?qs=5BZzbFV4k2sxVMcJXGEnkA%3D%3D) |
| U5                | RECOM        | R-78B6.5-1.0                      | [Mouser](https://www.mouser.com/ProductDetail/RECOM-Power/R-78B65-10?qs=YWgezujkI1Jcc6KIi%2FUXSQ%3D%3D) |

## Choice of Inductor, Capacitor

### Capacitor C1

Here is a selection of capacitor values we have tried.
All capacitors are 1 kV 1206 package.

| value         | manufacturer | part number                       |  vendors |
| :------------ | :----------- | :-------------------------------- | :------- |
| 56 pF         | Yageo        | CC1206JKNPOCBN560                 | [Mouser](https://www.mouser.com/ProductDetail/Yageo/CC1206JKNPOCBN560?qs=57cj7OiSijk2ADKKy4CU4w%3D%3D) |
| 68 pF         | Yageo        | CC1206JKNPOCBN680                 | [Mouser](https://www.mouser.com/ProductDetail/YAGEO/CC1206JKNPOCBN680?qs=%2Fha2pyFadug73UYpGd%252BxPCodrP9t1yPAmB6ei%252BRQAXUgR15E4Y3f04eqgfo8VHxn) |
| 82 pF         | Yageo        | CC1206JKNPOCBN820                 | [Mouser](https://www.mouser.com/ProductDetail/YAGEO/CC1206JKNPOCBN820?qs=%2Fha2pyFaduh7TvSxD6fC4KQyd0WEN8cCHOqGNtgg9MbcnQ3QLJdDsRoXSgCCCvv1) |
| 100 pF        | Yageo        | CC1206JKNPOCBN101                 | [Mouser](https://www.mouser.com/ProductDetail/YAGEO/CC1206JKNPOCBN101?qs=%2Fha2pyFadujRA6m79NnYQujiXiLHd9w8NvfQhCb8VhSoiFxooafVE%252BzvpZqtWvYF) |

### Inductors L1/L2

Here is a selection of inductor values we have tried.

| value         | manufacturer | part number                       |  vendors |
| :------------ | :----------- | :-------------------------------- | :------- |
| 33 uH         | Murata       | 22R333C                           | [Mouser](https://www.mouser.com/ProductDetail/Murata-Power-Solutions/22R333C?qs=AG1tZYOK7s5pE%2FTYgTs9bg%3D%3D) |
| 47 uH         | Murata       | 22R473C                           | [Mouser](https://www.mouser.com/ProductDetail/Murata-Power-Solutions/22R473C?qs=%2Fha2pyFadugoA%2Fk5i2DUbgFpVnul5qs31wjF4kEwPYY%3D) |
| 68 uH         | Murata       | 22R683C                           | [Mouser](https://www.mouser.com/ProductDetail/Murata-Power-Solutions/22R683C?qs=%2Fha2pyFaduhlAKY0M3i02bKEquptsHNV%2Fctmf2oZRWA%3D) |
| 100 uH        | Murata       | 22R104C                           | [Mouser](https://www.mouser.com/ProductDetail/Murata-Power-Solutions/22R104C?qs=%2Fha2pyFaduhkBoeUh6V30xx9He2flPOg7g7wQHv1g4k%3D) |
| 150 uH        | Murata       | 22R154C                           | [Mouser](https://www.mouser.com/ProductDetail/Murata-Power-Solutions/22R154C?qs=%2Fha2pyFaduiTZaBPCTvNTsouAFHewVG7TfxtlnQlubA%3D) |
| 220 uH        | Murata       | 22R224C                           | [Mouser](https://www.mouser.com/ProductDetail/Murata-Power-Solutions/22R224C?qs=%2Fha2pyFaduht2UPdDLlcZfB5aVrFhnwJo8oyD0ERCHs%3D) |
