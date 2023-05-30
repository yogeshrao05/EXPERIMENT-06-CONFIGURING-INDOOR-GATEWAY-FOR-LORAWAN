# EXPERIMENT-06-CONFIGURING-INDOOR-GATEWAY-FOR-LORAWAN

## Aim: To Interface a Analog Input (soil moisture sensor) to ARM IOT development board and write a program to obtain the data on the com port
## Components required: Dragino LPS8 Indoor LoRaWAN gateway, ETHERNET cable RJ45,Internet connection 

## Theory :
Dragino LPS8 Indoor LoRaWAN gateway
![image](https://github.com/vasanthkumarch/EXPERIMENT-06-CONFIGURING-INDOOR-GATEWAY-FOR-LORAWAN/assets/36288975/6ad9d336-ac3f-43b2-9801-1a647c936b37)

 
The LPS8 is an open-source LoRaWAN Gateway. It lets you bridge LoRa wireless network to an IP network via WiFi, Ethernet. The LoRa wireless allows users to send data and reach extremely long ranges at low data rates. The LPS8 uses a Semtech packet forwarder and is fully compatible with the LoRaWAN protocol.
![image](https://github.com/vasanthkumarch/EXPERIMENT-06-CONFIGURING-INDOOR-GATEWAY-FOR-LORAWAN/assets/36288975/74ae1f27-5105-4998-af15-b9de7e26ff3b)

 
It includes an SX1308 LoRa concentrator, which provides 10 programmable parallel demodulation paths. LPS8 has pre-configured standard LoRaWAN frequency bands to use for different countries. Users can also customize the frequency bands to use in their own LoRa network.
The gateway has an antenna to receive the LoRa Packets in 8-channels. On the front side, it has a USB Type C port for Input Power of DC 5V,2A. Apart from the power, it also has an Ethernet port, USB Host Port & a Toggle button to reset the gateway.
![image](https://github.com/vasanthkumarch/EXPERIMENT-06-CONFIGURING-INDOOR-GATEWAY-FOR-LORAWAN/assets/36288975/19c6189c-ebfa-423b-83bd-113cd24b76f4)

 
At bottom of the gateway, it has the LoRa Pico Station information Like Model-LPS8, Frequency Band, Serial Number, and the WiFi mac address.
 
 LED Indicators
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-06-CONFIGURING-INDOOR-GATEWAY-FOR-LORAWAN/assets/36288975/e0042eb3-e451-4d55-aa7c-664c5f8c57c3)

 
LPS8 has totally four LEDs, They are:
➢ Power LED: This RED LED will be solid if the device is properly powered.
➢ LoRa LED: This RGB LED will blink GREEN when the LoRaWAN module starts or transmit a
packet.
➢ SYS LED: This RGB LED will show different colors in the different states:
✓ SOLID BLUE: The device is alive with a LoRaWAN server connection.
✓ BLINKING BLUE: a) Device has internet connection but no LoRaWAN Connection. or b)
The device is in the booting stage, in this stage, it will BLINKING BLUE for several seconds and
then with SOLID RED and BLINKING BLUE together
✓ SOLID RED: The device doesn’t have an Internet connection.
➢ ETH LED: This LED shows the ETH interface connection status.
## Procedure :

The LPS8 is configured as a WiFi Access Point by factory default. You can access and configure the LPS8 after connecting to its WiFi network, or via its WAN Ethernet port.
1. Connect via WiFi
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-06-CONFIGURING-INDOOR-GATEWAY-FOR-LORAWAN/assets/36288975/b5dfbc1b-9632-4641-b904-4376616a8e52)
2. At the first boot of LPS8, it will auto-generate a WiFi network called dragino-xxxxxx with password: dragino+dragino
You can use a PC to connect to this WiFi network. The PC will get an IP address of 10.130.1.xxx and the LPS8 has the default IP 10.130.1.1.
3. Connect via Ethernet with DHCP IP from router
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-06-CONFIGURING-INDOOR-GATEWAY-FOR-LORAWAN/assets/36288975/fd2b1577-59ab-47f4-b6f5-202ceba6e7f2)
 
 Alternatively, connect the LPS8 Ethernet port to your router and LPS8 can obtain an IP address from your router. In the router’s management portal, you should be able to find what IP address the router has assigned to the LPS8. You can also use this IP to connect.
 4. Connect via WiFi with DHCP IP from router

![image](https://github.com/vasanthkumarch/EXPERIMENT-06-CONFIGURING-INDOOR-GATEWAY-FOR-LORAWAN/assets/36288975/56fcc965-4bb0-48cf-82f9-e30f4f268819)


