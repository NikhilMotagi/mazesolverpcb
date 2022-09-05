#                                                                     MILLI MOUSE

This repo is for pcbs that were designed for mazesolver MILLIMOUSE (RIP)

The project went through many changes, some were minor some were major. Following are short discriptions about each design.

## MAZESOLVERWITHIR

u(mew)controller of choice was STM32F103C8T6 , because why not, it is faster than Arduino and has a bigger storage.

Here IR sensors acted as proximity sensors. They woud send signals when walls are in a given range.

RGB led was used to give indications and also to flash like police strobe light becuase why not *FLEXXXXXX*(later it was understood "why not").

MPU6050 was used to get orientations of the bot, so that perfect 90 degree turns could be performed.

Battery - 7.4V 2S lipo orange battery, a buck converter was used to step it down to 5V. 

Points to be noted--> 

1)IR won't always work as intended and calibaration is a nightmare as the readings change with ambient light.
2) Do not flip the PCB print while exporting PDF for both back copper. Only valid for text 


## MAZESOLVERSTM32_ULTRASONIC

KNOCK KNOCK 

Who's there ?

Ambient light 

IR's were not the greatest choice for checking distance, also there was concern about centering the bot.

SO here comes the new component HC-SR04!

![image](https://user-images.githubusercontent.com/108187933/187035809-9d8ce7aa-5b93-409c-a6cf-48883612d72f.png)


The pcb had to be redesigned for ultrasonic and this time for good, the placement were done using dxf files from cad so everything was perfect.

![WhatsApp Image 2022-09-05 at 15 48 17](https://user-images.githubusercontent.com/79624087/188426844-40304372-0e6f-4091-9aff-40f026c11422.jpeg)

Other unsophisticated yet time saving efforts were also explored(We all agreed pcb is the way to go).

![WhatsApp Image 2022-08-08 at 16 50 47](https://user-images.githubusercontent.com/79624087/188428295-6e39c248-6e13-4d1f-80e8-6f5b0404e9cf.jpeg)






