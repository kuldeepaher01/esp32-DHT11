
# ESP32-DHT11

This is an ESP-IDF driver for the DHT11 temperature and humidity sensor. It is based on the work of [kaizoku-oh](https://github.com/kaizoku-oh/esp32-DHT11) and has been updated to work with newer versions of ESP-IDF.

## Installation

There are multiple ways to install this library:

1.  Using PlatformIO:
    
    -   You can install the library using PlatformIO by following the instructions provided in this [link](https://platformio.org/lib/show/5817/ESP32-DHT11).
2.  Manual Installation:
    
    -   Clone this repository into your PlatformIO project's `components` folder or the `[esp]/esp-idf/components` folder.

## Usage

To use the ESP32-DHT11 library in your project, follow these steps:

1.  Import the `dht11.h` header file into your program.
    
2.  Initialize the DHT11 sensor by calling the `DHT11_init(gpio_num)` function, where `gpio_num` is the GPIO pin number to which the DHT11 sensor is connected.
    
3.  Call the `DHT11_read()` function whenever you need to read from the DHT11 sensor. This function returns a struct containing the temperature and humidity readings, as well as a status code for error checking.
    
    **Note:** The `DHT11_read()` function is a blocking function, meaning it will wait until the sensor data is available before returning.
    

You can find more information and usage examples in the `examples` folder of this repository.

**WARNING:** Keep in mind that the `DHT11_read()` function is a blocking function, so it may introduce delays in your program execution.

Feel free to explore the examples and modify the library according to your specific requirements.
