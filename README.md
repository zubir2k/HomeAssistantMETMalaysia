# HomeAssistantMETMalaysia ![visitors](https://visitor-badge.glitch.me/badge?page_id=zubir2k.homeassistantmetmalaysia.visitor-badge)
Weather forecast from Malaysia Meteorological Department (MET) API.\
Please register and obtain METToken from [https://api.met.gov.my/](https://api.met.gov.my/)

### What's New
- Location code is now available as dropdown list.
- METToken number is now defined in `secret.yaml`
- Satellite imagery can be selected from a dropdown list.
- Included imagery from [Windy](https://windy.com)
- Added sensors from [wttr.in](https://wttr.in)

## Installation
### 1. Copy all files
- Browse into your Home Assistant directory and paste all files into `\config`.

### 2. Add your METToken to [secret.yaml](secret.yaml)
- Add the following line into the secret yaml file

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
- [HomeAssistantMalaysia](https://www.facebook.com/groups/homeassistantmalaysia)
