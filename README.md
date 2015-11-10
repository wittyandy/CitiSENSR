# CitiSENSR

<b>Objective:</b>
This project aims to develop a mobile environmental monitoring platform using Arduino (open-source prototyping platform) and commercially available air pollution and meteorology monitoring devices.
 
<b>Motivation:</b>
It all came naturally from my own needs to develop a custom datalogger to connect different air pollution monitoring devices. Air pollution monitoring devices, such as TSI's DustTrak and Thermo Scientific's pDR 1500, all come with different communiaction protocols and software to download data from the device to a computer. Often times, downloading process takes unnecessarily longer time in addition to the time it takes to sample air quality. 

<b>Devices used:</b>
TSI P-Trak: capable of counting ultrafine particles in outdoor environment. It operate by drawing an aerosol sample continuously through a heated saturator, in which alcohol is vaporized and diffuses into the sample stream. Isopropyl alcohol cartridge needs to be replaced every 3 hours depending on the temperature of a sampling site.

Temperator/Relative humidity sensor: Vaisala HMP50 temperature and humidity probe
 
Wind direction/speed sensor: Gill WindSonic Ultrasonic Anemometer 
TSI DustTrak 8520: capable of measuring PM 10 or PM 2.5 concentrations in outdoor environment. The communication protocol is RS232, and uses specific command to communicate with the device
 
TSI CPC 3007: capable of measuring much finer ultrafine particle concentrations than the P-trak. It operates with the same principle as the P-Trak, but it has faster response to freshly emitted traffic pollution, therefore, it is used widely for measuring near-road traffic pollution.

<b>Progress:</b>
We were successful at reading signals from analog devices. We will soon post a sketch (code) that enables reading analog signals. The major challenges with this project is that different devices use different communication protocols. So it is difficult to directly connect monitoring devices to Arduino system and expect Arduino to automatically read the signals. The device that uses analog signal is much simpler because there is no protocol issues. But when it comes to reading digital signals, each manufacturer and even with the same manufacturer, different models use different protocols. So it is a big challenge to have Arduino talk to the device through diginal signals. 
