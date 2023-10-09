---
description: Architecture of CDCC
---

# CDCC Pins

Some of the pins in CDCC controller.

<table data-full-width="true"><thead><tr><th width="227">Communication</th><th width="139">Number</th><th>Pins</th></tr></thead><tbody><tr><td>LIN</td><td>5</td><td>A16, A37, A38, B12, B32</td></tr><tr><td>CAN High</td><td>8</td><td>A25, A33, A43, A48, B03, B10, B13, B16</td></tr><tr><td>CAN Low</td><td>8</td><td>A24, A32, A44, A49, B04, B11, B14, B15</td></tr><tr><td>Flex-ray</td><td>4</td><td>A21, A22 (out) , A39, A40 (in)</td></tr><tr><td>Ethernet</td><td>4</td><td>B30, B31, C01, C02</td></tr><tr><td>Analog</td><td>4</td><td>A11, A12, A27, A45</td></tr><tr><td>PWM/PFM (in)</td><td>4</td><td>A19, B01, B17, B18</td></tr><tr><td>Digital out/Multi bit out</td><td>4</td><td>A26, A50, B29, A07 (in too)</td></tr><tr><td>Digital In | PWM/PFM in Digital out| Multi bit out</td><td>1</td><td>A20</td></tr><tr><td>Resistance out</td><td>7</td><td>A10, A30, B05, B06, B09, B25, B26</td></tr><tr><td>Ground</td><td>6</td><td>A18, A31, A41, A46, A47, B23</td></tr><tr><td>Sent out/ digital Out</td><td>2</td><td>A05, A42</td></tr><tr><td>Power 5V</td><td>3</td><td>A23, A28, A29,</td></tr><tr><td>KL87 (12 V power pin)</td><td>1</td><td>A36</td></tr><tr><td>KL30 power supply</td><td>1</td><td>A17</td></tr><tr><td>IGN\KL 15</td><td>1</td><td>A54</td></tr><tr><td>Unused</td><td>2</td><td>A03, A04</td></tr></tbody></table>



Requirement

* 8 CAN channels
* 5 LIN channels
* 2 Flexray
* 2 Ethernet

