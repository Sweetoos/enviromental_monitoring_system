# Smart Environmental Monitoring System

Project mainly made for my college but wanted to learn something there
## components

- STM32F446RE
- ESP32
- BME280 
- RGB LED
- Potentiometer
- A couple of resistors and wires


## interfaces

- **UART** - computer printout
- **I2C** - BME280 read
- **SPI** - communication between boards (STM32 master, ESP32 slave)
- **TIM** - delay
- **ADC** - setting PWM with potentiometer 
- **PWM** - led brightness

value read by sensor will determine in what colour led will light

stm32 will handle those interfaces, esp32 will write a plot to a site

uart will just write a value to a computer
