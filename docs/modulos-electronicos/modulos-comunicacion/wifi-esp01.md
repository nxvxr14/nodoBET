---
sidebar_position: 1
---

# WIFI ESP01

<img src="https://http2.mlstatic.com/D_NQ_NP_978371-MLU75805003117_042024-O.webp" alt="ESP01 WiFi Module" style={{maxHeight: '200px'}} />

## Descripción

El módulo ESP01 es una pequeña placa de desarrollo basada en el chipset ESP8266. Este módulo permite conectar microcontroladores a una red WiFi y establecer conexiones TCP/IP sencillas mediante comandos AT. Es ampliamente utilizado en proyectos de IoT (Internet de las Cosas) debido a su bajo costo, tamaño reducido y facilidad de implementación.

## ¿Que incluye?

- 1x Módulo WiFi ESP01
- No incluye adaptador USB ni cables de conexión

## Ubicación

| Código     | E5B3-000 |
| ---------- | -------- |
| Estantería | 5        |
| Bandeja    | 3        |
| Posición   | 000      |

## Cantidad Disponible

15 unidades (actualizado: Marzo 2025)

## Características Técnicas

- Procesador: Tensilica L106 32-bit RISC
- Voltaje de operación: 3.3V (NO tolera 5V)
- Consumo de corriente: 70mA (promedio)
- Protocolos soportados: 802.11 b/g/n
- Potencia de transmisión: +19.5dBm en modo 802.11b
- Memoria flash: 1MB
- Pines GPIO disponibles: 2
- Comunicación serial UART
- Velocidad CPU: 80MHz/160MHz

## Pinout

<img src="https://programarfacil.com/wp-content/uploads/2017/01/pines-esp01.png" alt="ESP01 Pin Diagram" style={{maxHeight: '200px'}} />

```
    GND   1 |·    ·| 8   TX
    GPIO2  2 |     | 7   CH_PD
    GPIO0  3 |     | 6   RST
    RX     4 |     | 5   VCC
```

### Función de cada pin

- **GND**: Conexión a tierra.
- **GPIO2**: Pin de entrada/salida de propósito general. Usado comúnmente para LED o sensores.
- **GPIO0**: Pin de entrada/salida de propósito general. También determina el modo de arranque (alto: modo normal, bajo: modo programación).
- **RX**: Pin receptor UART para comunicación serial.
- **VCC**: Alimentación (3.3V exclusivamente).
- **RST**: Pin de reset. Un pulso bajo reinicia el módulo.
- **CH_PD**: Chip Enable. Debe estar en alto (3.3V) para que el módulo funcione.
- **TX**: Pin transmisor UART para comunicación serial.

## Códigos de Ejemplo

- [Ejemplos básicos de ESP8266](https://github.com/esp8266/Arduino)
- [Blink LED con ESP01](https://github.com/esp8266/Arduino/blob/master/libraries/ESP8266WiFi/examples/WiFiClientBasic/WiFiClientBasic.ino)
- [Servidor Web Simple](https://github.com/esp8266/Arduino/blob/master/libraries/ESP8266WebServer/examples/HelloServer/HelloServer.ino)

## DataSheet Fabricante

[Datasheet ESP8266](https://www.espressif.com/sites/default/files/documentation/0a-esp8266ex_datasheet_en.pdf)
