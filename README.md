# APDS9253

Simple Arduino sketch to test Broadcom's APDS9253 rgbiR light sensor. The I2C sensor has a wide dynamic range, has four dedicated channels for R, G, B, and IR, has a mode where only the ambient light (green) and IR channels are active to save power, and has an interrupt for light threshold or light variation detection. The interrupt would have been more useful if it included a data ready function as well as separate interrupt bits for crossing the high and low thresholds. But this is a pretty useful sensor that makes for a poor man's 4-channel spectrometer (FWHM ~ 100 nm) as well an ambient light sensor.

![APDS9253](https://user-images.githubusercontent.com/6698410/128101546-b2eb92d6-e1f3-4c89-8ffc-c4788b52b8da.jpg)

I used the STM32L432 ([Ladybug](https://www.tindie.com/products/tleracorp/ladybug-stm32l432-development-board/)) development board to test but the sketch shoud be easy to adapt for almost any MCU.

The breakout board [design](https://oshpark.com/shared_projects/T91eXOoo) is available on the OSH Park shared space.
