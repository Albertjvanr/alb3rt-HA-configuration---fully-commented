# Home Assistant Configuration

## Here's my [Home Assistant](https://home-assistant.io/) configuration. 
I try to keep my repo updated as I change or add to my HA environment. I'm currently running HA version [here](.HA_VERSION). If this helps you in your automation, please :star2: my repo!

## I run two HA instances:  

###### The first HASSIO runs passive add-ons which are not required for automation:

- ###### [Raspberry Pi 3 Model B] (http://a.co/d/0pbf4mV) with a [32GB Class 10 U3 SD Card] (http://amzn.eu/d/8QAG2rw)
- There is one component loaded to monitor the hardware usage [sensor.systemmonitor] (https://www.home-assistant.io/components/sensor.systemmonitor/)

- The add-ons running on this HASSIO are:
  - Aircast
  - Phlex
  - Pi-hole
  - Samba Share
  - TasmoAdmin
  - Unifi Controller
  
## The second HASSIO runs everything else used in automations and monitoring
- ###### [Raspberry Pi 3 Model B+] (http://amzn.eu/d/5RpW4iO) with a [32GB Class 10 U3 SD Card] (http://amzn.eu/d/8QAG2rw)

## Devices used with HA
	
  * **Network**
    - [Netgear R7800 Nighthawk X4S AC2600] (http://a.co/d/5OqR3Ms)
    - [Ubiquiti UAP-LR AP] (http://a.co/d/4sCwuTp) controlled with Unifi Controller set up on different HA instance
    - Pi-hole set up on different HA instance
    - [Netgear WN2500RP Wireless Extender] (http://a.co/d/52VTbSx)
  * **Voice Interaction**
    - [Google Home Mini] (https://www.walmart.com/ip/Google-Home-Mini-Chalk-2-Pack/599120369) x 2
    - Google TTS
  * **Media and sound**
    - Plex running on local server desktop (Intel(R) Core(TM) i7-8700 CPU @ 3.20Ghz 8 BG DDR4 RAM Samsung SSD 850 EVO 250 GB (WIN 10) 20 TB (5 Seagate 4 TB SkyHawk 3.5” HDD) 
    - **Lounge**:
      - [Xbox One] (http://a.co/d/j3hOXwk) (HDMI output to soundbar)
      - [Samsung TV - UA60JU6400] (https://www.samsung.com/africa_en/tvs/uhd-ju6400/UA60JU6400KXXA/) (HDMI input from soundbar)
      - [LG Soundbar SJ9] (http://a.co/d/6yMQZkd) (HDMI input from Xbox One, HDMI output to Samsung TV)
      - [Apple TV 3] (https://support.apple.com/kb/SP648?locale=en_US) (HDMI output to Xbox One)
    - **Bedroom**:
      - [Apple TV 4] (https://support.apple.com/en-za/HT207936) (HDMI output to Sansui TV, bluetooth output to JBL Extreme speaker)
      - [Sansui TV STY1232] (https://www.bradlows.co.za/sansui-32in-81cm-led-tv-sty0632) (HDMI input from Apple TV 4) - Non-smart TV (had to find alternative ways to control and monitor)
      - [JBL Extreme] (http://a.co/d/gkN13MM) (bluetooth sound from Apple TV)
  * **Switches (power and lights) and energy monitoring (all Sonoffs are flashed with Tasmota firmware) (https://github.com/arendst/Sonoff-Tasmota)**
    - [Sonoff POW] (http://a.co/d/9RN6YRc) x 21
    - [Sonoff Basic] (http://a.co/d/2CjNuC3) x 4
    - [Sonoff TH16 with Temperature and Humidity Sensor] (http://a.co/d/0iX6ZQ6) x 2
    - [Sonoff SV with reed switch] (http://a.co/d/5tVlqeX) x 1
    - [Sonoff Touch US1] (http://a.co/d/2HTQjRI) x 1
  * **IR control**
    - [Harmony Hub with additional IR transmitter] (http://a.co/d/iR1lRTu - http://a.co/d/abvFSP4)
  * **Lights and motion**
    - [Philip Hue Bridge] (http://a.co/d/ilgeKVX)
    - [Philips Hue Motion Sensor] (http://a.co/d/71q3MCT) x 6
    - [Philips Hue Colour GU10] (http://a.co/d/2uo5FRV) x 21
    - [Philips Hue White Ambiance GU10] (http://a.co/d/2GPoJGa) x 17
    - [Philips Hue Dimmer Switch] (http://a.co/d/5SZ3rIa)
  * **Presence detection**
    - Netgear Device Tracker
    - Google Maps
    - iOS app
    - iCloud
  * **Weather**
    - Darksky
  * **Notifications**
    - iOS app

## Control and Automations
	
  * Bedroom TV control (ON/OFF)
  * Arriving home automations
  * Day/night light automations
  * Garage door control
  * Geyser automations (ON/OFF, limit simultaneous power usage)
  * Home announcements
  * Light scenes
  * Bathroom extractor fan control (ON/OFF based on humidity sensor)
  * Nursery (baby) temperature control via wall panels (heat only)
  * Nursery (baby) sleep time control (ON/OFF fairy lights)
  * Pool pump timer control
  * Set home to sleep mode automation
  * Create snapshots and upload to Dropbox
  * Soundbar volume control
  * Toilet or bathroom occupied light automation (turn ON/OFF lights outside room if occupied/unoccupied)
  * TV globe lights automation
  * TV monitoring when turned ON/OFF manually
  * Update of iCloud device statuses every 1 minute when home (used in other automations)
  * Xbox volume control

## Non-HA Automations
	
  * Philips Hue light in motion areas are directly controlled by the Hue Montion sensors

## My Home Assistant dashboard

I switches over to Lovelace and don't use the default UI anymore. Screenshots of my UI below:

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_home.png" alt="Home Assistant dashboard" />

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_lounge.png" alt="Home Assistant dashboard" />

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_bedroom.png" alt="Home Assistant dashboard" />

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_nursery.png" alt="Home Assistant dashboard" />

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_kitchen.png" alt="Home Assistant dashboard" />

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_garden_and_pool.png" alt="Home Assistant dashboard" />

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_network.png" alt="Home Assistant dashboard" />

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_monitors.png" alt="Home Assistant dashboard" />

<img src="https://github.com/Albertjvanr/alb3rt-HA-configuration---fully-commented/blob/master/view_motion_areas.png" alt="Home Assistant dashboard" />


