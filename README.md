# Environment-Sensing-Node 

Video tutorial : [https://youtu.be/ULMnPckZp1M](https://www.youtube.com/watch?v=M5VGos3YTpI&list=LL&index=2)

![alt text](https://github.com/akarsh98/Helium-Environment-sensor/blob/main/Environment%20Sensor%20node/25.JPG)
In this project, we are going to make an Helium Network connected Environment Sensing Node using the Wisblock Helium Developer Kit from RAK. We are going to using the RAK 1906 Environment Sensing Node and Connect it to the RAK Core module with a LoRa Antenna and after that we will code and configure the node in order to conect it to our Helium Data only Hotspot. The node will be configured in such a manner that it will continuously monitor the environment conditions around it such as the Temperature, Pressure, Humidity and Gas Resistance and send the data collected to the Helium data only Hotspot. That data can be seen on the Staging console.

![alt text](https://github.com/akarsh98/Helium-Environment-sensor/blob/main/Environment%20Sensor%20node/21.JPG)

The data that we will receive will be encoded in base64 format and will not be human readable so we will use integrations available on the Helium Console to decode the received data and store that data in a Google Sheet. For that we will create a blank google form that will push the data into the Spreadsheet. We will also update the code block of the Google Sheets Integration to decode the data before storing it to the Sheet and after that we will link the Google Sheet with our added Device which is our data only Hotspot that receives data from the node.  

![alt text](https://github.com/akarsh98/Helium-Environment-sensor/blob/main/Environment%20Sensor%20node/24.JPG)

After all the configuration and Integrations part is done, we need to check if everything is working fine so for that we can open the Serial monitor of our Arduino IDE. There we will see the data sent by the Node. We can also check the Staging Helium Console to check if the data is getting received or not. If everything goes as planned, then we will see that at regular interval of times the Google sheet will update and the Environment data will continue to log in the Sheet.


![alt text](https://github.com/akarsh98/MQTT-ESP8266-demo-with-Reyax/blob/main/Home%20Automation%20Board/jlcpcb.JPG)


You must check out [JLCPCB](https://jlcpcb.com/aka) for ordering PCBs online for cheap!

You get 10 good quality PCBs manufactured and shipped to your doorstep for 2$ and some shipping. You will also get a discount on shipping on your first order. To design your own PCB head over to easyEDA, once that is done upload your Gerber files onto [JLCPCB](https://jlcpcb.com/aka) to get them manufactured with good quality and quick turnaround time
