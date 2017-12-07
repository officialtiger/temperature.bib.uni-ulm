# Temperature measurement at the library of the University of Ulm
4 Sensors reading out data including temperature and humidity

## Environment
The project is carried out in the Communication and Information Centre (kiz) of the University of Ulm. This is an internal project of the kiz, which should help to solve the temperature problems of the library.

## Project description:
The aim of the project is to build a measuring station that can measure and output temperature and humidity.

The data is measured with sensors and transferred to a gateway using the LoraWan protocol. The gateway sends the data in IP packets to the backend of TTN Ulm.
The data is then retrieved there using Node Red and stored in an InfluxDB. 
Grafana is used as representation, which receives and displays the sensor data from the InfluxDB.

## Hardware components:
- Adafruit Feather M0
- BME280 (temperature, humidity, pressure)
- Power supply with Adaptor
- Case
- Optional:
  - air quality sensor
  - battery (fail-safe in case of power supply failure)

## Presentation - Prezi [German]
https://prezi.com/view/cG6FL62uhYvEj2B41j7k/

