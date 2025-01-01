![metmalaysia](https://user-images.githubusercontent.com/1905339/221524236-022f5460-1e30-4c00-81a8-a9560d36a668.png) \
![visitors](https://visitor-badge.glitch.me/badge?page_id=zubir2k.homeassistantmetmalaysia.visitor-badge)
[![Donate](https://img.shields.io/badge/donate-Coffee-yellow.svg)](https://zbrj.ml/buymecoffee)

> [!Tip]
> Home Assistant Integration is available as a successor to this template. \
> [https://github.com/zubir2k/homeassistant-malaysiaweather](https://github.com/zubir2k/homeassistant-malaysiaweather)

Weather forecast from Malaysia Meteorological Department (MET) API.\
Please register and obtain METToken from [https://api.met.gov.my/](https://api.met.gov.my/)

### What's New
- 2 Weather entity: weekly and current day
- Location code is now available as dropdown list.
- METToken number is now defined in `secrets.yaml`
- Satellite imagery can be selected from a dropdown list.
- Included satellite imagery from [Windy](https://windy.com)
- Added sensors from [wttr.in](https://wttr.in)

## Installation
### 1. Copy all files
- Browse into your Home Assistant directory and paste all files into `\config`.

### 2. Add your METToken to [secrets.yaml](secrets.yaml)
- Add the following line into the secret yaml file. (**IMPORTANT**: replace below with your acquired METToken)

```yaml
metmalaysia: METToken 1234567890abcdefghijklmnopqrstuvwxyz1234
```

### 3. Enable package in [configuration.yaml](configuration.yaml)
- Add the following line into the config file

```yaml
homeassistant:
  packages: !include_dir_named HAMY/
```

- Restart Home Assistant to take effect.

### 4. Dashboard [lovelace-ui.yaml](lovelace-ui.yaml)
- Add new card, scroll at the bottom and choose Manual. 
- Copy & paste the YAML respectively.

### 5. Configuration
- Select location from the drop down list
- Select the satellite imagery \
[It may take a while for the sensor to fully update]

## Automation Ideas
- Idea #1: Prompt/notify to take your laundry if its going to rain.
- Idea #2: Send reminder on today's weather before going out.
- Feel free to apply any automation from these sensors

### Example output
![image](https://user-images.githubusercontent.com/1905339/212635754-3eaefad6-ee02-4e63-b93c-2813c50b4570.png)

### Special Thanks
- [Bro Anas](https://github.com/anas-ivs) for pointing out MET API 
- [MET Malaysia](https://www.met.gov.my/)
- [HomeAssistantMalaysia](https://www.facebook.com/groups/homeassistantmalaysia)
