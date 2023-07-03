
# Devil-Twin  = Evil Twin + Deauther   -ESP8266 

<p align="center">
<img title="Version" src="https://img.shields.io/badge/Version-1.0-green">
<img title="Support" src="https://img.shields.io/badge/Support-No-red">
</p>

Welcome to the project.
This project is Moddified with https://github.com/p3tr0s/PhiSiFi and https://github.com/SpacehuhnTech/esp8266_deauther
Use this tool only on networks that you have permission for.

<img src=https://github.com/mahadidot/DEVIL-TWIN_esp8266/blob/main/meme.jpg></img><br>

It uses an ESP8266 to attack a WiFi network using Deauther & Evil-Twin AP method.

## FEATURES :
* Now you can control web interface with simple android app **NEW
* Dark themed UI
* WIFI Refresh button (without reloading the page manually)
* Wi-Fi Signal Strength show with -dbm
* Deauthentication of a target WiFi access point
* Evil-Twin AP to capture passwords with password verification against the og access point
* It can do both attacks at the same time, no toggling of the deauther is required.

## Screenshots

<table>
  <tr>
    <th>Victim POV</th>
    <th>Checking Password/ </th> 
    <th>192.168.4.1/pro</th>
    <th>192.168.4.1 Main UI/</th>
  </tr>
  <tr>
    <td>This is the main page. Here the user will write his password and send it.</td>
    <td>This is the post page. The user will be redirected here after entering the password.</td>
    <td>This is where the attacker can the passwords that has been Pawned.</td>
    <td>Here the attacker index, wifi names, mac, signal strenth (-dbm).</td>
  <tr>
    <td><img width="200px" src="https://github.com/mahadidot/DEVIL-TWIN_esp8266/blob/main/victim.jpg" title="victim pov"></td>
    <td><img width="200px" src="https://github.com/mahadidot/DEVIL-TWIN_esp8266/blob/main/check.jpg" title="checking password"></td>
    <td><img width="200px" src="https://github.com/mahadidot/DEVIL-TWIN_esp8266/blob/main/gotpass.jpg" title="pass"></td>
<td><img width="200px" src="https://github.com/mahadidot/DEVIL-TWIN_esp8266/blob/main/ui.jpg" title="ssid"></td>
  </tr>
</table>


## Install using Arduino IDE
1. Install Arduino IDE
2. In Arduino go to `File` -> `Preferences` add this URL to `Additional Boards Manager URLs` ->
   `https://raw.githubusercontent.com/SpacehuhnTech/arduino/main/package_spacehuhn_index.json`  
3. In Arduino go to `Tools` -> `Board` -> `Boards Manager` search for and install the `deauther` package  
4. Download and open [Devil-Twin](https://github.com/mahadidot/DEVIL-TWIN_esp8266/releases/download/Deauther-Evil-M4H4DI/Deauther-Evil-M4H4DI.ino) with Arduino IDE
6. Select an `ESP8266 Deauther` board in Arduino under `tools` -> `board`
7. Connect your device and select the serial port in Arduino under `tools` -> `port`
8. Click Upload button

# How to use:
- Connect to the AP named `M4H4D!~H4$$4N` with password `devil2in` from your phone/PC.
- Select the target AP you want to attack .
- Click the Start Deauthing button to send deauth frames and start kicking devices off the selected network.
- Click the Start Evil-Twin button. {optionally reconnect to the newly created AP named same as your target. (will be open)}
- You can stop any of the attacks by visiting 192.168.4.1/pro while conected to Evil-Twin AP or by resetting the ESP8266.
- Once a correct PASSWORD is found, AP will be restarted with default ssid "M4H4D!~H4$$4N" / "devil2in" and at the bottom of a table you should be able to see something like "Successfully got password for - `TARGET_SSID` - `PASSWORD`

## DISCLAIMER
The source code given in this public repo is for educational use only and should only be used against your own networks and devices!<br>
Please check the legal regulations in your country before using it.


## Credits:
* https://github.com/SpacehuhnTech/esp8266_deauther
* https://github.com/M1z23R/ESP8266-EvilTwin
* https://github.com/adamff1/ESP8266-Captive-Portal
* https://github.com/p3tr0s/PhiSiFi

## License 
This software is licensed under the [MIT License](https://opensource.org/licenses/MIT).
