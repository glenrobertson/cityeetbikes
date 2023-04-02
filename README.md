# cityeetbikes
Fork of [homeassistant/core -> /homeassistant/components/citybikes](https://github.com/home-assistant/core/tree/dev/homeassistant/components/citybikes) but with e-bike availability, based on https://github.com/home-assistant/core/pull/85279

## Setup

* Setup [HACS](https://hacs.xyz/)
* Go to HACS tab in home assistant
* Click three dots in top right corner, then "Custom Repositories"
* Repository: https://github.com/glenrobertson/cityeetbikes 
* Category: Integration
* Restart Home Assistant, then add [sensor config](https://www.home-assistant.io/integrations/citybikes/) to home assistant configuration.yaml, except replace platform "citybikes" with "cityeetbikes", example below

## Example configuration

```yaml
sensor:
  - platform: cityeetbikes
    name: Home Stations
    stations:
       - 66dce567-0aca-11e7-82f6-3863bb44ef7c # UID for Citibike 'McKibbin St & Manhattan Ave' station
```
