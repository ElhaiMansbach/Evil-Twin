# Protection-of-wireless-and-mobile-networks




An evil twin attack is a spoofing cyberattack that works by tricking users into connecting to a fake Wi-Fi access point that mimics a legitimate network. Once a user is connected to an “evil twin” network, hackers can access everything from their network traffic to private login credentials.

--------------------------------------------------------------------------------------------------

<h3>Checking Wifi Adapter</h3>   
Install Details: https://www.aircrack-ng.org/doku.php?id=install_aircrack (Under Compiling and installing)   

Dependencies:   
- 'sudo apt-get update -y'   
- 'sudo apt-get install libz-dev'   
- 'sudo apt-get install libssl-dev'   
- 'sudo apt-get install ethtool'   
    
Utility At: 'sudo aircrack-ng'   

Injection Test Details: https://www.aircrack-ng.org/doku.php?id=injection_test   
   
   
Interfaces Details: 'sudo /usr/local/sbin/airmon-ng' OR 'sudo /usr/sbin/airmon-ng'   
    (can be found with 'find / -name airmon-ng')
    
Start: 'sudo airmon-ng start wlan0'   

Injection Test: 'sudo aireplay-ng -9 wlan0mon'   

Checking attack types (2 cards are needed): 'sudo aireplay-ng -9 -i wlan1mon wlan0mon'   
    (When the attacking card is wlan0mon)   
    
 Should run before: 'sudo airmon-ng check kill'   
