# Smart Environmental Monitoring System

Project mainly made for my college but wanted to learn something there

The idea was created by chatgpt (for a while there will be copied text from chatgpt, but I will fix this when my arm will be in shape)

Description:
Develop a smart environmental monitoring system using an STM32 microcontroller that can measure various environmental parameters such as temperature, humidity, and air quality. The system will have multiple sensors connected via I2C and SPI interfaces. It will also feature a display to provide real-time data visualization and a UART interface for remote monitoring/control.

Components:

STM32 microcontroller (STM32F446RE)
Temperature sensor (e.g., DS18B20) connected via SPI
Humidity sensor (e.g., DHT22) connected via UART
Air quality sensor (e.g., MQ-135) connected via ADC
OLED display connected via I2C
UART module for communication with a PC or other devices
PWM module for controlling external actuators (e.g., fans, heaters)
Functionality:

- ADC: Use ADC channels of the STM32 to read analog values from the air quality sensor (MQ-135).
- Timers and Interrupts: Utilize timers and interrupts to schedule periodic sampling of sensor data, ensuring timely updates without CPU intervention.
- I2C: Communicate with the OLED display using the I2C protocol to display real-time sensor data and system status.
- SPI: Interface with the temperature sensor (DS18B20) using the SPI protocol to measure temperature.
- UART: Establish UART communication with the humidity sensor (DHT22) to retrieve humidity data.
- PWM: Control external actuators such as fans or heaters based on environmental parameters measured by the sensors.
- Display: Utilize the OLED display to present real-time data such as temperature, humidity, air quality index, and system status.
- User Interface: Implement user interaction through buttons or a keypad connected to GPIO pins for settings adjustment or mode switching.
