# ADXL345 MCU
This is a board using a STM32F103 MCU, designed to make using an [ADXL345 module](https://s.click.aliexpress.com/e/_APsfkw) for [Klipper](https://github.com/KevinOConnor/klipper)'s [Input Shaping](https://github.com/KevinOConnor/klipper/blob/master/docs/Measuring_Resonances.md) much easier, by only requiring a USB connection.
<br>You can find more information [here](https://www.youtube.com/watch?v=tDQd-jGegX0).
<br>
<br>Add these to the top of your printer.cfg. Use the correct serial address.
```
[mcu adxl]
serial: /dev/serial/by-id/xxx
```
<br> Add these somewhere in your printer.cfg. Edit according to your printer.
```
[adxl345]
cs_pin: adxl:PA4
spi_software_sclk_pin: adxl:PA5
spi_software_mosi_pin: adxl:PA7
spi_software_miso_pin: adxl:PA6

[resonance_tester]
accel_chip: adxl345
probe_points:
   175,175,20
```
<br>Recommended PCB manufacturers:
<br>[PCBWay](https://www.pcbway.com/setinvite.aspx?inviteid=374841) (Better looking PCBs)
<br>[JLCPCB](https://jlcpcb.com/) (Easier SMT Service)
<br>
<br>USB C Used:
<br>[Digi-Key](https://www.digikey.com/en/products/detail/gct/USB4085-GF-A/9859733)
<br>
<br>ADXL345 Module:
<br>[AliExpress](https://s.click.aliexpress.com/e/_APsfkw)
<br>[Amazon](https://amzn.to/3k1iGy9)
<br>
<br>Affiliate/Associate links above
