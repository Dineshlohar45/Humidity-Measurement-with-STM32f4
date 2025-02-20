# Humidity-Measurement-with-STM32f4
Humidity Measurement using STM32 AND HUMIDITY SENSOR 
Explanation
Initialization
System Clock Configuration: Configures the system clock using HSI (High-Speed Internal) oscillator.
GPIO Initialization: No specific GPIO pins are initialized for this project.
TIM2 Initialization: Initializes TIM2 for timestamping and other timing-related purposes.
Task Creation
vTask_Humidity: A FreeRTOS task that reads humidity every second using the read_humidity function and prints the value to the console. It uses the vTaskDelayUntil function to ensure it runs periodAically.
Humidity Sensor Simulation
humidity_sensor.h and humidity_sensor.c: These files define and implement a dummy function read_humidity that simulates reading from a humidity sensor. In a real application, this function would interface with actual hardware to get the humidity value.
Both projects demonstrate basic FreeRTOS functionality on an STM32 microcontroller, with one focusing on toggling an LED and the other on reading and printing humidity values.
