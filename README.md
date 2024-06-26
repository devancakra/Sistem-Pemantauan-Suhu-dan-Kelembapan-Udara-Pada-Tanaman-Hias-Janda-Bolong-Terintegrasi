[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?style=flat)](https://github.com/ellerbrock/open-source-badges/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?logo=github&color=%23F7DF1E)](https://opensource.org/licenses/MIT)
![GitHub last commit](https://img.shields.io/github/last-commit/devancakra/Sistem-Pemantauan-Suhu-dan-Kelembapan-Udara-Pada-Tanaman-Hias-Janda-Bolong-Terintegrasi)
![Project-IOT](https://img.shields.io/badge/Project-Bot-%2DWeb%20of%20Things-light.svg?style=flat&logo=arduino&logoColor=white&color=%23F7DF1E)

# Monitoring-Suhu-Kelembapan-Udara-Tanaman-Hias-Janda-Bolong
<strong>Team Project - Informatics UPN Veteran Jatim</strong><br><br>
Janda bolong is a plant from the Araceae or taro species that can survive optimally in temperatures of 23-30°C, with air humidity of less than 40%. Temperature and humidity must be monitored at all times, as extreme changes can cause the plant to wilt. This project was created to make it easier for users to monitor changes in temperature and humidity in the janda bolong planting area in real time, so that users will benefit more in terms of time and energy. This project has been implemented and took approximately 1 month. The benefit of making this project is none other than to maintain the growth and development of janda bolong plants. The results showed that the system created can function properly. The system interface uses Telegram Bot and Website.

<br><br>

## Project Requirements
| Part | Description |
| --- | --- |
| Development Board | NodeMCU V3 ESP8266 Lolin |
| Code Editor | • Arduino IDE<br>• Visual Studio Code |
| Application Support | Telegram Bot |
| Driver | CH340 USB Driver |
| IoT Platform | ThingSpeak |
| Communications Protocol | • Hypertext Transfer Protocol (HTTP)<br>• MTProto |
| IoT Architecture | 4 Layer |
| Framework | Bootstrap |
| Programming Language | • C/C++<br>• JavaScript<br>• PHP |
| Arduino Library | • ESP8266WiFi (default)<br>• ThingSpeak<br>• DHT_sensor_library<br>• CTBot<br>• ArduinoJson |
| Sensor | DHT22: Air Temperature & Humidity (x1) |
| Other Components | • Micro USB cable - USB type A (x1)<br>• Jumper cable (1 set)<br>• Casing box (x1)<br>• Adaptor DC 5V (x1) |

<br><br>

## Download & Install
1. Arduino IDE

   <table><tr><td width="810">

   ```
   https://bit.ly/ArduinoIDE_Installer
   ```

   </td></tr></table><br>

2. CH340 USB Driver

   <table><tr><td width="810">

   ```
   https://bit.ly/CH340_USB_Driver
   ```

   </td></tr></table>
   
<br><br>

## Project Designs
<img width="840" src="https://github.com/devancakra/Sistem-Pemantauan-Suhu-dan-Kelembapan-Udara-Pada-Tanaman-Hias-Janda-Bolong-Terintegrasi/assets/54527592/6a251217-20c2-4576-8f6a-d9e64415f456">

<br><br>

## Arduino IDE Setup
1. Open the ``` Arduino IDE ``` first, then open the project by clicking ``` File ``` -> ``` Open ``` : 

   <table><tr><td width="810">
      
      ``` monitoring_suhu.ino ```

   </td></tr></table><br>
   
2. Fill in the ``` Additional Board Manager URLs ``` in Arduino IDE

   <table><tr><td width="810">
   
      Click ``` File ``` -> ``` Preferences ``` -> enter the ``` Boards Manager Url ``` by copying the following link :
      
      ```
      http://arduino.esp8266.com/stable/package_esp8266com_index.json
      ```

   </td></tr></table><br>
   
3. ``` Board Setup ``` in Arduino IDE

   <table>
      <tr><th width="810">

      How to setup the ``` NodeMCU V3 ESP8266 Lolin ``` board
            
      </th></tr>
      <tr><td>
         
      • Click ``` Tools ``` -> ``` Board ``` -> ``` Boards Manager ``` -> Install ``` esp8266 ```. 
      
      • Then click ``` Tools ``` -> ``` Board ``` -> ``` ESP8266 Boards ``` -> ``` NodeMCU 1.0 (ESP-12E Module) ```.

      </td></tr>
   </table><br>
   
4. ``` Change the Board Speed ``` in Arduino IDE

   <table><tr><td width="810">
   
      Click ``` Tools ``` -> ``` Upload Speed ``` -> ``` 9600 ```

   </td></tr></table><br>
   
5. ``` Install Library ``` in Arduino IDE

   <table><tr><td width="810">
   
      Download all the library zip files. Then paste it in the: ``` C:\Users\Computer_Username\Documents\Arduino\libraries ```

   </td></tr></table><br>

6. ``` Port Setup ``` in Arduino IDE

   <table><tr><td width="810">
   
      Click ``` Port ``` -> Choose according to your device port ``` (you can see in device manager) ```

   </td></tr></table><br>

7. Change the ``` WiFi Name ```, ``` WiFi Password ```, and so on according to what you are currently using.<br><br>

8. Before uploading the program please click: ``` Verify ```.<br><br>

9. If there is no error in the program code, then please click: ``` Upload ```.<br><br>

10. If there is still a problem when uploading the program, then try checking the ``` driver ``` / ``` port ``` / ``` others ``` section.

<br><br>

## ThingSpeak Setup
1. Getting started with ThingSpeak :

   <table><tr><td width="810">

      • Please <a href="https://thingspeak.com/login">Log in</a> to access the ThingSpeak service.
      
      • If you don't have a ThingSpeak account yet, please create one.

   </td></tr></table><br>

2. Create a channel :

   <table><tr><td width="810">

      • After logging into the account -> click ``` New Channel ```.
   
      • Fill in the form according to your needs.
   
      • Click ``` Save Channel ```.
   
      • Click ``` Sharing ``` -> in the ``` Channel Sharing Settings ``` section please select -> ``` Share channel view with everyone ```.

   </td></tr></table><br>

3. Create visualizations :

   <table><tr><td width="810">

      • Make sure you are in the ``` Channel ``` menu -> ``` Public View ``` section.
   
      • Click ``` + Add Visualization ```.
   
      • Click ``` Field Chart ``` -> then select ``` Save ```.
   
      • If you want to change the visualization content, please click ``` Field Chart Option ``` -> then select ``` Save ``` to save.

   </td></tr></table><br>

4. Create widgets :

   <table><tr><td width="810">

      • Make sure you are in the ``` Channel ``` menu -> ``` Public View ``` section.
   
      • Click ``` + Add Widgets ```.
   
      • Click ``` Numeric Display ``` -> then select ``` Next ```.
   
      • In the ``` Configure widget parameters ``` section, please fill in according to your needs -> then select ``` Create ```.
   
      • If you want to change the widget content, please click ``` Widget Option ``` -> then select ``` Save ``` to save.

   </td></tr></table><br>

5. Firmware configuration :

   <table><tr><td width="810">

      • Make sure you are in the ``` Channel ``` menu -> ``` Public View ``` section.
   
      • Copy the ``` Channel ID ``` -> paste it into the firmware code. For example :
   
      <table><tr><td width="780">

      ```ino
      unsigned long ChannelID = '1504372'; // ID ThingSpeak
      ```

      </td></tr></table>
   
      • Please go to the ``` API Keys ``` section -> paste it into the firmware code. For example :
   
      <table><tr><td width="780">

      ```ino
      const char * APIKey = "TF3UPJK9O1QA5FAU"; // Apikey ThingSpeak
      ```

      </td></tr></table>
   
      • Click ``` Field Chart IFrame ``` to display the selected chart link -> paste the link into the web program code.
   
      • Click ``` Widget IFrame ``` to display the selected widget link -> paste the link into the web program code.

   </td></tr></table>

<br><br>

## Local Web Server Setup
1. Move the ``` Website-Project ``` directory into the ``` htdocs ``` directory, the details of which you can see as follows: ``` C:\xampp\htdocs ```.<br><br>
  
2. Open ``` index.php ``` inside the ``` Website-Project\iot-monstera\index.php ``` directory via ``` Visual Studio Code ```.<br><br>
   
3. The ``` <iframe> ``` tag please match the ``` visualization / widget link ``` in ``` ThingSpeak ```. For example :

   <table><tr><td width="810">

   ```html
   <iframe style="width:85%;height:240px;" src="https://thingspeak.com/channels/1504372/charts/1?bgcolor=%23ffffff&color=%23d62020&dynamic=true&results=60&title=Grafik+%28Temperatur+Udara%29&type=line"></iframe>
   ```

   </td></tr></table><br>
   
4. Open ``` XAMPP ```, then start the ``` Apache ``` section. This aims to be able to support the website optimally.<br><br>
   
5. To ``` access the website ```, open your ``` browser ``` by writing : ``` localhost/Website-Project/iot-monstera/index.php ```.
    
<br><br>

## Telegram Bot Setup
1. Open <a href="https://t.me/botfather">@BotFather</a>.<br><br>

2. Type ``` /newbot ```.<br><br>

3. Type the desired bot name, for example: ``` monistera_bot ```.<br><br>

4. Type the desired bot username, for example: ``` monistera_bot ```.<br><br>

5. Also do it for bot image settings, bot descriptions, and so on according to your needs.<br><br>

6. Copy ``` your telegram bot API token ``` -> then paste it into the ``` #define BOTtoken "YOUR_API_BOT_TOKEN" ``` section. 

   <table><tr><td width="810">

   For example :

   ```ino
   #define BOTtoken "2006772150:AAE6Fdjk3KbiySkzV6CLbd6ClJDzgTfJ5y0"
   ```

   </td></tr></table>

<br><br>

## Get Started
1. Download and extract this repository.<br><br>
    
2. Make sure you have the necessary electronic components.<br><br>
   
3. Make sure your components are designed according to the diagram.<br><br>
      
4. Configure your device according to the settings above.<br><br> 
 
5. Please enjoy [Done].

<br><br>

## Demonstration of Application
Via Telegram: <a href="https://t.me/monistera_bot">@monistera_bot</a>

<br><br>

## Highlights
<table>
<tr>
<th width="840">Product View</th>
</tr>
<tr>
<td><img src="https://user-images.githubusercontent.com/54527592/133962095-8baa3737-3bf0-4d6b-bc65-c0cff1c37021.jpg" alt="product-view"></td>
</tr>
</table>
<table>
<tr>
<th colspan="2">Telegram Bot View</th>
</tr>
<tr>
<td width="420"><img src="https://user-images.githubusercontent.com/54527592/133962195-70e38df7-8e56-422b-ba30-3b42a642c62b.JPG" alt="bot-menu1"></td>
<td width="420"><img src="https://user-images.githubusercontent.com/54527592/133962202-2399d06a-4f97-4335-86b4-4c043d7d1d17.JPG" alt="bot-menu2"></td>
</tr>
</table>
<table>
<tr>
<th width="840">Monitoring Website View</th>
</tr>
<tr>
<td><img src="https://user-images.githubusercontent.com/54527592/133962162-8856e20d-9e84-43c4-ac4a-0316d2c65004.jpg" alt="monitoring-web-view"></td>
</tr>
</table>

<br>
<strong>More information:</strong> <a href="https://ejournal.upnvj.ac.id/informatik/article/view/3436"><u>Click Here</u></a>

<br><br>

## Appreciation
If this work is useful to you, then support this work as a form of appreciation to the author by clicking the ``` ⭐Star ``` button at the top of the repository.

<br><br>

## Disclaimer
This application has been created by including third-party sources. Third parties here are service providers, whose services are in the form of libraries, frameworks, and others. I thank you very much for the service. It has proven to be very helpful and implementable.

<br><br>

## LICENSE
MIT License - Copyright © 2020 - Devan C. M. Wijaya, S.Kom

Permission is hereby granted without charge to any person obtaining a copy of this software and the software-related documentation files to deal in them without restriction, including without limitation the right to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons receiving the Software to be furnished therewith on the following terms:

The above copyright notice and this permission notice must accompany all copies or substantial portions of the Software.

IN ANY EVENT, THE AUTHOR OR COPYRIGHT HOLDER HEREIN RETAINS FULL OWNERSHIP RIGHTS. THE SOFTWARE IS PROVIDED AS IS, WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, THEREFORE IF ANY DAMAGE, LOSS, OR OTHERWISE ARISES FROM THE USE OR OTHER DEALINGS IN THE SOFTWARE, THE AUTHOR OR COPYRIGHT HOLDER SHALL NOT BE LIABLE, AS THE USE OF THE SOFTWARE IS NOT COMPELLED AT ALL, SO THE RISK IS YOUR OWN.
