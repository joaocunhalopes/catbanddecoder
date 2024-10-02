# CatBandDecoder

CatBandDecoder is a C# Windows Application that reads the frequency of Amateur Radio Tansceivers or Receivers.
Based on that frequency, the current amateur band is determined.
Once the band is determined, band information is send to an USB device that outputs band information using two different protocols:

- Yaesu BCD Band Data
- ICOM Band Voltage

This app is intended at the Amateur Radio Operators community.

## Supported CAT Protocols

The application supports the following CAT (Computer Aided Transceiver) protocols:

- CI-V, Communications Interface 5
- KSI, Kenwood Serial Protocol
- CAT, Yeasu CAT Computer Aided Transceiver)

CI-V is used by ICOM and Xiegu Transceivers. KSI is used by Kenwood Transceivers. CAT is used by Yeasu Transceivers.
If there's enough interest, support for Elecraft K3 protocol can be added.

## Supported Amateur Bands

Frequency limits for each band are configurable. Default is:

| Amateur Band     | Frequency (Lower) | Frequency (Upper) |
|------------------|-------------------|-------------------|
| 160 meters       | 1.800 MHz         | 2.000 MHz         |
| 80 meters        | 3.500 MHz         | 4.000 MHz         |
| 60 meters        | 5.3305 MHz        | 5.4065 MHz        |
| 40 meters        | 7.000 MHz         | 7.300 MHz         |
| 30 meters        | 10.100 MHz        | 10.150 MHz        |
| 20 meters        | 14.000 MHz        | 14.350 MHz        |
| 17 meters        | 18.068 MHz        | 18.168 MHz        |
| 15 meters        | 21.000 MHz        | 21.450 MHz        |
| 12 meters        | 24.890 MHz        | 24.990 MHz        |
| 10 meters        | 28.000 MHz        | 29.700 MHz        |
| 6 meters         | 50.000 MHz        | 54.000 MHz        |
| 2 meters         | 144.000 MHz       | 148.000 MHz       |
| 70 centimeters   | 420.000 MHz       | 450.000 MHz       |

## Supported Yaesu BCD Outputs

| Amateur Band     | Band A | Band B | Band C | Band D |
|------------------|--------|--------|--------|--------|
| 160 meters       |   0    |   0    |   0    |   1    |
| 80 meters        |   0    |   0    |   0    |   1    |
| 60 meters        |   0    |   0    |   0    |   1    |
| 40 meters        |   0    |   0    |   0    |   1    |
| 30 meters        |   0    |   0    |   0    |   1    |
| 20 meters        |   0    |   0    |   1    |   0    |
| 17 meters        |   0    |   0    |   1    |   0    |
| 15 meters        |   0    |   0    |   1    |   0    |
| 12 meters        |   0    |   0    |   1    |   1    |
| 10 meters        |   0    |   0    |   1    |   1    |
| 6 meters         |   0    |   1    |   0    |   0    |
| 2 meters         |   0    |   1    |   0    |   0    |
| 70 centimeters   |   0    |   1    |   0    |   1    |
| Out of Band      |   0    |   0    |   0    |   0    |

## Supported ICOM Voltage Outputs

| Amateur Band     | Band Min Voltage | Band Max Voltage | Average Voltage |
|------------------|------------------|------------------|-----------------|
| 160 meters       | 7                | 8                | 7.5             |
| 80 meters        | 6                | 7                | 6.5             |
| 40 meters        | 5                | 6                | 5.5             |
| 30 meters        | 0                | 1                | 0.5             |
| 20 meters        | 4                | 5                | 4.5             |
| 17 meters        | 3                | 4                | 3.5             |
| 15 meters        | 3                | 4                | 3.5             |
| 12 meters        | 2                | 3                | 2.5             |
| 10 meters        | 2                | 3                | 2.5             |
| 6 meters         | 1                | 2                | 1.5             |
| 2 meters         | Not Available    | Not Available    | Not Available   |
| 70 centimeters   | Not Available    | Not Available    | Not Available   |
| Out of Band      |   0              |   0              |   0             |

