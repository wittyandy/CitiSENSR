# CitiSENSR

<b>Objective:</b>
This project aims to develop a mobile environmental monitoring platform using Arduino (open-source prototyping platform) and commercially available air pollution and meteorology monitoring devices.
 
Motivation: 
It all came naturally from my own needs to develop a custom datalogger to connect different air pollution monitoring devices. Air pollution monitoring devices, such as TSI's DustTrak and Thermo Scientific's pDR 1500, all come with different communiaction protocols and software to download data from the device to a computer. Often times, downloading process takes unnecessarily longer time in addition to the time it takes to sample air quality. 
 
Devices used: 
DataLogger: Arduino YUN and Arduin Uno
Portable monitoring devices:

Objective:
This project is a collaboration with UCLA and Placemeter (TM) to apply and validate computer-vision technology to detect and quantify pedestrians, bicyclists, and vehicles using IP and surveillance cameras.
 
Motivation:
The motivation to partner with Placemeter came while I was doing a study on the impact of CicLAvia (car-free street event) on traffic and air quality. Traditionally, we have been using pneumatic tubes and human labor to count pedestrians, bicyclists, and traffic. However, Placemeter offers much easier and cheaper ways to quantify traffic data which do not require any of the installation or human labor. If this approach can be proven successful in counting bike/peds with higher accuracy, then this technology has the potential to disrupt the traditional traffic engineering practice of counting bikes/peds/vehicles. 
 
Progress:
The major challenges to this technology is to get access to city-owned CCTVs or IP cameras. New York City already opens their traffic CCTVs to the public, so Placemeter has no problem getting the traffic feeds from the internet.  For the Culver City CicLAvia event, we successfully recorded traffic camera feeds. Special thanks to Gabe Garcia (traffic engineering Analyst at Culver City) who helped us get the traffic camera feeds. Placemeter has successfully turned the traffic videos into valuable traffic count data. 

In the case of Los Angeles, however, there is no publicly available CCTV camera feeds, so we had to get permission from LA Department of Transportation to get access to their traffic feeds. It turns out that they have legal and security issues with regard to plugging any device to their system. So we couldn't use Placemeter technology for our project. In the future, if many cities adopt internet-connected CCTV cameras and made them available publicly, Placemeter technology has a bright future. At the moment, the legal and security hurdles the prohibit access to city-owned traffic feeds are the major barrier to applying this new technology.
 
What is Arduino?
Arduino is a small but powerful microcontroller (i.e. computer) that enables anyone to interface with any electronic devices and sensors. It was originally developed by Massimo Banzi and David Cuartielles to teach their students about electronic circuit boards, but now its use has been expanded beyond the classroom.
 
Arduino is now being used and implemented by commercial developers and engineers as a cross platform to connect and control different devices. The beauty of Arduino is that, thanks to its open-source approach,  you can customize any electronic devices to suit your needs with simple lines of codes based on C programming lanuage. There is also a huge community of developers, hobbists, students, and researchers that help each other's projects. 
What is Placemeter?
Placemeter is a company based in New York City that develops computer vision algorithm to offer users with convenient ways to quantify foot, bike, and vehicle traffic. They process video feeds from CCTV cameras, and their algorithm detects pedestrians, bicyclists, and vehicles with an accuracy of close to 90%. 
 
The computer vision algorithm was developed a long time ago around 60s, but what's unique about Placemeter is that they provide very convenient front-end user interface to monitor traffic in realtime. They also allow users to record video feeds using their smart phones and use that video to quantify traffic information. 
 
TSI P-Trak: capable of counting ultrafine particles in outdoor environment. It operate by drawing an aerosol sample continuously through a heated saturator, in which alcohol is vaporized and diffuses into the sample stream. Isopropyl alcohol cartridge needs to be replaced every 3 hours depending on the temperature of a sampling site.
 
Temperator/Relative humidity sensor: Vaisala HMP50 temperature and humidity probe
 
Wind direction/speed sensor: Gill WindSonic Ultrasonic Anemometer 
TSI DustTrak 8520: capable of measuring PM 10 or PM 2.5 concentrations in outdoor environment. The communication protocol is RS232, and uses specific command to communicate with the device
 
TSI CPC 3007: capable of measuring much finer ultrafine particle concentrations than the P-trak. It operates with the same principle as the P-Trak, but it has faster response to freshly emitted traffic pollution, therefore, it is used widely for measuring near-road traffic pollution.
Progress:
We were successful at reading signals from analog devices. We will soon post a sketch (code) that enables reading analog signals. The major challenges with this project is that different devices use different communication protocols. So it is difficult to directly connect monitoring devices to Arduino system and expect Arduino to automatically read the signals. The device that uses analog signal is much simpler because there is no protocol issues. But when it comes to reading digital signals, each manufacturer and even with the same manufacturer, different models use different protocols. So it is a big challenge to have Arduino talk to the device through diginal signals. 
