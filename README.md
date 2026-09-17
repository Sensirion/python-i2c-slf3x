# Python I2C Driver for Sensirion SLF3X

This repository contains the Python driver to communicate with a Sensirion sensor of the SLF3X family over I2C.

<img src="https://raw.githubusercontent.com/Sensirion/python-i2c-slf3x/master/images/sensor_SLF3C_1300F.png"
    width="300px" alt="SLF3X picture">


Click [here](https://sensirion.com/products/catalog/liquid-flow-sensors?series=SLF3x) to learn more about the Sensirion SLF3X sensor family.


Not all sensors of this driver family support all measurements.
In case a measurement is not supported by all sensors, the products that
support it are listed in the API description.



## Supported sensor types

| Sensor name   | I²C Addresses  |
| ------------- | -------------- |
|[SLF3C-1300F](https://sensirion.com/products/catalog/SLF3C-1300F/)| **0x08**|
|[SLF3S-1300D](https://sensirion.com/products/catalog/SLF3S-1300D/)| **0x08**|
|[SLF3S-1300F](https://sensirion.com/products/catalog/SLF3S-1300F/)| **0x08**|
|[SLF3S-0600D](https://sensirion.com/products/catalog/SLF3S-0600D/)| **0x08**|
|[SLF3S-0600F](https://sensirion.com/products/catalog/SLF3S-0600F/)| **0x08**|
|[SLF3S-4000B](https://sensirion.com/products/catalog/SLF3S-4000B/)| **0x08**|

The following instructions and examples use a *SLF3C-1300F*.



## Connect the sensor

You can connect your sensor over a [SEK-SensorBridge](https://developer.sensirion.com/product-support/sek-sensorbridge/).
For special setups you find the sensor pinout in the section below.

<details><summary>Sensor pinout</summary>
<p>
<img src="https://raw.githubusercontent.com/Sensirion/python-i2c-slf3x/master/images/SLF3x_Pinout.png"
     width="300px" alt="sensor wiring picture">

| *Pin* | *Cable Color* | *Name* | *Description*  | *Comments* |
|-------|---------------|:------:|----------------|------------|
| 1 |  | NC | Do not connect |
| 2 | green | SDA | I2C: Serial data input / output |
| 3 | red | VDD | Supply Voltage | 3.2V to 3.8V
| 4 | black | GND | Ground |
| 5 | yellow | SCL | I2C: Serial clock input |
| 6 |  | NC | Do not connect |


</p>
</details>


## Documentation & Quickstart

See the [documentation page](https://sensirion.github.io/python-i2c-slf3x) for an API description and a
[quickstart](https://sensirion.github.io/python-i2c-slf3x/quickstart.html) example.


## Contributing

In case you want to contribute to this project, please read the [contribution guidelines]((https://sensirion.github.io/python-i2c-slf3x/contributing.html)).

## License

See [LICENSE](LICENSE).