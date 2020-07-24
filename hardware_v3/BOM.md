## hardware v3 bill of materials

These are the parts on the board from the schematic.  All of them can
be ordered from [Digi-Key](https://www.digikey.com/) together in one
shipment.

| Quantity | Reference | Digi-Key_PN         | MPN              | Manufacturer                    | Package                     | Description                               | Notes                                            |
| -------- | --------- | ------------------- | ---------------- | ------------------------------- | --------------------------- | ----------------------------------------- | ------------------------------------------------ |
| 1        | J1        | 952-2262-ND         | M20-9990246      | Harwin Inc.                     | through-hole (2.54mm pitch) | 2x1 male header                           | Install J1 jumper to defeat EEPROM write protect |
| 1        | J2        | S5750-20-ND         | NPPN202AFCN-RC   | Sullins Connector Solutions     | through-hole (2.54mm pitch) | 20x2 female header                        | pi GPIO header                                   |
| 1        | J3        | 23-0877602616-ND    | 0877602616       | Molex                           | through-hole (2.54mm pitch) | 13x2 male header 90 degree                | Straight or 90 degree depending on application   |
| 1        | R2        | P10.0KCCT-ND        | ERJ-6ENF1002V    | Panasonic Electronic Components | 0805                        | 10K, 1/8 watt resistor                    | Pull-up for EEPROM write protect                 |
| 2        | R3 R4     | P3.90KCCT-ND        | ERJ-6ENF3901V    | Panasonic Electronic Components | 0805                        | 3.9K, 1/8 watt resistor                   | Pull-ups for ID EEPROM                           |
| 1        | R5        | P1.40KCCT-ND        | ERJ-6ENF1401V    | Panasonic Electronic Components | 0805                        | 1.4K ohm, 1/8 watt resistor               | Pull-up for STATUS3                              |
| 1        | U1        | CAT24C32WI-GT3CT-ND | CAT24C32WI-GT3   | ON Semiconductor                | 8-SOIC                      | I2C Serial EEPROM 32Kb                    | ID EEPROM                                        |
| 1        | U2        | 296-8467-1-ND       | SN74LVC161284DLR | Texas Instruments               | 48-SSOP (0.64mm lead pitch) | 19-bit bus interface with 3-state outputs | pin 1 marking oriented opposite J3               |
| 1        | C1 C2     | 399-1177-1-ND       | C0805C104Z5VACTU | KEMET                           | 0805                        | 100nF, 50V capacitor                      | Bypass                                           |

Additional board mounting and connector components:

| Quan | Description | Supplier | Notes |
| ---- | ----------- | -------- | ----- |
| 4    | M2.5 x 16mm brass standoff, with M2.5 nut | [Adafruit](https://www.adafruit.com/product/2336) | pi HAT standoff (height 11mm) |
| 4    | M2.5 x 6mm philips head screw |    |    |
| 1    | Female DB25 to female 13x2 header cable assembly | [Amazon](https://www.amazon.com/Motherboard-Parallel-Printer-bracket-socket/dp/B00PI5XF4U) | or surplus |
