# CatBandDecoder (under development)

CatBandDecoder is a C# Windows Application that reads the frequency of an Amateur Radio Tansceivers or Receivers.
Based on that frequency, a given amateur band is determined (supported bands are 160m, 80m, 40m, 30m, 20m, 17m, 15m, 12m, 10m and 6m).
Once the band is determined, band information is send to an USB device that outputs band information using two different protocols:

- Yaesu BCD Band Data
- ICOM Band Voltage

This app is intended at the Amateur Radio Operators community.

The application supports the following CAT (Computer Aided Transceiver) protocols:

- CI-V, Communications Interface 5
- KSI, Kenwood Serial Protocol
- CAT, Yeasu CAT Computer Aided Transceiver)

CI-V is used by ICOM and Xiegu Transceivers. KSI is used by Kenwood Transceivers. CAT is used by Yeasu Transceivers.
If there's enough interest, support for Elecraft K3 protocol can easly be added.
