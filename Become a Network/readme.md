# **Become a Network**
---
#### Why is it important to know how a network works? Well without networks you wouldn't have the internet which basically means no YouTube/Multiplayer Games/anything from this generation LOL
- Let's go ahead and get the basics down for a network
---
### Network basics (15 Minutes)
- Quick talk about devices make it out to the internet
- Demonstrated website traffic with Wireshark
---

## With the basics down, it's time for our plan

### Setup access point software with NodeMCU (10 Minutes)
1. Open a Browser
2. Go to this link **https://rebrand.ly/wifijammercode**
3. Save the File
4. Let's go ahead and extract the zip folder
5. Go ahead and open the .ino file with Arduino
6. BOOM, project opened
7. Go to "Tools" and verify it's still using the same port as last time
8. Now on line 439 & 443 of the A_config.h file, let's change our SSID to "myname"and password to "", the lines should look something like this

```c++
#ifndef AP_SSID
  #define AP_SSID "pwned"  
#ifndef AP_PASSWD
  #define AP_PASSWD "deauther"
```

after changes:  

```c++
// ===== ACCESS POINT ===== //
#ifndef AP_SSID
  #define AP_SSID "myname"
#endif /* ifndef AP_SSID */

#ifndef AP_PASSWD
  #define AP_PASSWD ""
#endif /* ifndef AP_PASSWD */
```
9. With changes to the ssid and password, go ahead and upload the code
---

### Implementation (35 Minutes)
1. Find or think of a common SSID found in public that gives out free WiFi
2. Put it under the ssid where we previously put your name
3. To see how many people actually joined:
  - Join your own network on the laptop you have
  - Then go to 192.168.4.1 on that device you have
  - Agree to the website conditions
  - Scroll down and see the count of devices connected besides "Saved Devices"
4. Just remember to subtract one since your laptop is one of the devices
