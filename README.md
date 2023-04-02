# cityeetbikes
Fork of [homeassistant/core -> /homeassistant/components/citybikes](https://github.com/home-assistant/core/tree/dev/homeassistant/components/citybikes) but with e-bike availability, based on https://github.com/home-assistant/core/pull/85279

## Setup

* Setup [HACS](https://hacs.xyz/)
* Go to HACS tab in home assistant
* Click three dots in top right corner, then "Custom Repositories"
* Repository: https://github.com/glenrobertson/cityeetbikes 
* Category: Integration
* Restart Home Assistant, then add [sensor config](https://www.home-assistant.io/integrations/citybikes/) to home assistant configuration.yaml, except replace platform "citybikes" with "cityeetbikes", example below

## Example

### Configuration

```yaml
sensor:
  - platform: cityeetbikes
    name: Home Stations
    stations:
       - 66dcecfa-0aca-11e7-82f6-3863bb44ef7c # UID for NYC Citibike 'Stagg St & Union Ave' station
```

### Output
The additional `ebikes` property on the sensor is shown below

<img src="https://github.com/glenrobertson/cityeetbikes/blob/main/docs/stagg-and-union-nyc-citibike-sensor.png?raw=true" />
