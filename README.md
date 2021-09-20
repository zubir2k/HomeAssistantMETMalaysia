# HomeAssistantMETMalaysia ![visitors](https://visitor-badge.glitch.me/badge?page_id=zubir2k.homeassistantmetmalaysia.visitor-badge)
Pull weather forecast from Malaysian Meteorological Department (MET) API.\
Sensors are based on General Forecast with range of Today, Yesterday and Tomorrow.

Please register and obtain METToken from [https://api.met.gov.my/](https://api.met.gov.my/)

## Installation
### 1. [configuration.yaml](configuration.yaml)
- Copy the sensors to your current configuration.yaml.
- Change the METToken number to your own given number in line 19
- Change the location code (also in line 19) `locationid=LOCATION:288` to your desired location [here.](LOCATION.md)

### 2. [lovelace.yaml](lovelace.yaml)
- Create a new page
- Copy and paste 😋

### 3. Automation Ideas
- Idea #1: Prompt/notify to take your laundry if its going to rain.
- Idea #2: Send reminder on today's weather before going out.
- Feel free to apply any automation from these sensors

### Example output
![image](https://user-images.githubusercontent.com/1905339/134056863-58bcd82f-2afe-4cb5-aaa8-edc743483d7d.png)

### Special Thanks
- [Bro Anas](https://github.com/anas-ivs) for pointing out MET API 
- [HomeAssistantMalaysia](https://www.facebook.com/groups/homeassistantmalaysia)
