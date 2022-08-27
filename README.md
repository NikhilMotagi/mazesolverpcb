## mazesolverpcb aka MILLI MOUSE

This is repo for pcbs that were designed for mazesolver(RIP)

The project went through many changes some were minor some were major. Following are short discription about each design.

# MAZESOLVERWITHIR

ucontroller of choice was STM32F103C8, because why not, it is faster than Arduino and has bigger storage.
Here IR sensors act as proximity sensor. They send signals when walls are in given range.
RGB led was used to give indications and also to flash like police strobe light becuase why not *FLEXXXXXX*(later it was understood "why not").
MPU6050 was used to get orientation of the bot, so that perfect 90 degree turn would be performed.
Battery - 7.4V 2S lipo orange battery, a buck converter was used to step it down to 5V. 

Points to be noted--> 

1)IR won't always work as intended and calibaration in nightmare as the readings change with ambient light.
2) Do not flip the PCB print while exporting PDF for both back copper. Only valid for text 

#MAZESOLVERSTM32_ULTRASONIC

KNOCK KNOCK 

Whose there 

Ambient light 

IR's were not the greatest choice for checking distance, also there was concern about centering the bot.

SO here comes the new component HC-SR04![image](https://user-images.githubusercontent.com/108187933/187035809-9d8ce7aa-5b93-409c-a6cf-48883612d72f.png)

The pcb had to be redesigned for ultrasonic and this time for good the placement were done using dxf files from cad so everything was perfect.

![image](https://user-images.githubusercontent.com/108187933/187036156-738f1b72-ef58-4832-a75d-38c501753ac5.png)

