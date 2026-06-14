# Nextion Interface

This folder describes the graphical interface developed for the supervision module using a Nextion display.

The interface allows the user to:
- monitor climate variables;
- monitor soil moisture and irrigation state;
- monitor lighting and PPFD values;
- monitor energy data;
- change setpoints;
- send manual commands to the local control module;
- visualize alarms and system status.

## Main Pages

- Climate page
- Irrigation page
- Lighting page
- Energy page
- Setpoints page
- CO2 page prepared for future integration
- pH page prepared for future integration

## Communication

The Nextion display communicates with MCU2 through UART. MCU2 processes the commands received from the display and sends the corresponding instructions to MCU1 through LoRa.

Examples of commands:
- FAN_ON
- FAN_OFF
- BOMBA_ON
- BOMBA_OFF
- LED_ON
- LED_OFF
- MODO_AUTO
- SET_TEMP
- SET_SOIL
- SET_ILUM
- GUARDAR_SETPOINTS
