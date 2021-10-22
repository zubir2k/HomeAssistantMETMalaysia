# HomeAssistantMETMalaysia ![visitors](https://visitor-badge.glitch.me/badge?page_id=zubir2k.homeassistantmetmalaysia.visitor-badge)
Weather forecast from Malaysia Meteorological Department (MET) API.\
Sensors are based on General Forecast with range of Today, Yesterday and Tomorrow.

Please register and obtain METToken from [https://api.met.gov.my/](https://api.met.gov.my/)

**UPDATE/CHANGELOG** 

**22/10/2021 @ 11:30AM:**\
Enhancement to sensors to support custom weather template. 

**24/09/2021 @ 11:30PM:**\
Enhancement to sensors using for loop to determine the correct array. Removed some of the sensor attributes.

**21/09/2021 @ 9:00PM:**\
As suspected, the response from the api will generated in random sequence
Thus impacting the array and causes the sensors to get wrong data. Will need to test few more rounds.

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
![image](https://user-images.githubusercontent.com/1905339/134056863-58bcd82f-2afe-4cb5-aaa8-edc743483d7d.png)\
![image](https://user-images.githubusercontent.com/1905339/138391388-d2e0ecc4-f71a-438d-b589-9361dc8daab7.png)\
![image](https://user-images.githubusercontent.com/1905339/138391416-0ecda0a6-2c4c-41e2-9217-60da0ee8de8b.png)

### Special Thanks
- [Bro Anas](https://github.com/anas-ivs) for pointing out MET API 
- [HomeAssistantMalaysia](https://www.facebook.com/groups/homeassistantmalaysia)
