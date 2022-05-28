# Cargas-AC-ESP32
Dispositivo diseñado para taller práctico de Internet de las Cosas aplicado a dómotica durante el FIT (Foro de Innovación Tecnológica). Evento organizado por Universidad Galileo en Guatemala. 
El dispositivo contiene:
- ESP32
- Acelerómetro
- Sensor de intensidad de luz
- NeoPixeles
- Buzzer
- BME280
- Control de cargas AC.

# ¿Quién obtuvo un Smart Home?

Los participantes ganadores del mejor proyecto en el taller práctico de Internet de las Cosas obtuvieron su tarjeta electrónica Smart Home.

# ¿Cómo funciona?

El Smart Home funciona por medio de un microcontrolador ESP32 el cual posee conectividad WiFi y BLE, el cual puede ser programado con difentes lenguajes de programación entre los mas utilizados se encuentra C++ y Micropython.

# ¿Qué podemos hacer?

Pesplegar información por medio de un web server o dashboard MQTT en plataformas como [adafruitIO][adafruit_io] por medio de conexión WiFi, obtiene mediciones de temperatura, humedad y presión atmosférica por medio del sensor BME280, podemos controlar cargas AC por medio de sus Relay, cuenta con LED de tipo NeoPixel como indicadores, Buzzer para aplicaciones con sonido y es capas de ser conectada con asistentes de voz como Alexa y google assistant.

[adafruit_io]: https://io.adafruit.com

# Ejemplos con MicroPython 

Para utilizar micropython con nuestro Smart Home visite el siguiente repositorio para mayor información  [FunPython Ecuador][FPE].

[FPE]: https://github.com/FunPythonEC/FIT_Guatemala_2019-SMART_HOME











# Descripción de pines 

### Pantalla OLED SSD 1306, Temperatura y Humedad – Comunicación I2C
Referencia --- | SSD 1306 | --- | SHT30 |
ESP32            | SCL IO22 | --- | SCL IO22 |
---------------- | -------- |---- | -------- |
| SSD 1306| --- | SHT30 | 
| SCL IO22 | -- | SCL IO22 |
| SDA IO23 | -- | SDA IO23 |

### Control Cargas AC 
Referencia --- | CARGA 1 | --- | CARGA 2 | --- | CARGA 3 |
ESP32            |  IO25   | --- |  IO26   | --- |  IO27   | 

### LED Neopixel - Comunicación SPI
Referencia --- | WS2812B | 
ESP32            |   SD3   |
5V | VCC 

GND | GND


### Control Cargas AC 
Referencia --- | SCT 013 | --- | Voltaje AC |
ESP32            |  IO15   | --- |     IO2    |
                 | ADC2_2  | --- |   ADC2_3   |
# Licencia

Hardware License: CERN OHL v1.0 para más información visitar el siguiente [Link][CERN_v1].

[CERN_v1]: https://ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-1.2

Software License: GPL v3

Documentation License: CC BY 4.0 International
