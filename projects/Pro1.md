---
layout: project
type: project
image: images/first.3.jpg
title: Smart Farming System using Robot and Wireless Sensor Networks, IOT
permalink: projects/Smart Farming System using Robot and Wireless Sensor Networks, IOT
# All dates must be YYYY-MM-DD format!
date: 2015-07-01
labels:
  - Robotics & IoT
  - Microcontroller (AT89S52) 
  - Raspberry Pi
summary: My team developed a robotic mouse that won first place in the 2015 UH Micromouse competition.
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/first.1.jpg">
  <img class="ui image" src="../images/first.2.jpg">
  <img class="ui image" src="../images/first.3.jpg">
  <img class="ui image" src="../images/first.4.jpg">
</div>

Monitoring the environmental factors is not the complete solution to increase the yield of crops. Our system aims to make cultivation and irrigation more efficient as the farmer is able to make better informed decisions based on the data sent by sensor nodes at appropriate time and thus save time and resources. The diversity of location and climatic effects upon agricultural cultivation, along with other environmental parameters over time makes the farmer’s decision-making process more complicated and requires additional empirical knowledge. Applying wireless sensor networks for monitoring environmental parameters and combining this information with a user-customized web service may enable farmers to exploit their knowledge in an efficient way in order to extract the best results from their agricultural cultivation.

This data is sent to the farmer through interface of a website using raspberry Pi. After receiving the data farmer takes appropriate action by sending commands to the bot to perform the task via Application interface. The bot will then perform the necessary task such as watering the regions which require water in sufficient quantity. The bot will cater to the needs of the region as indicated by the soil moisture sensor autonomously. This bot can also be used for Livestock monitoring using image processing with help of camera module attached to the bot. The bot is mobile and can move around the field on a grid into which the farm will be segregated using the concept of maze solver bot.

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

Here is video that illustrates how we read values from the line sensors and control the bot: [Video] (https://vimeo.com/336328309).


