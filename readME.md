### Mood Lamp

#### What should it do?
- Lamp mode
- Notifications
- Time based
- User controlled

##### IFTTT Triggers with thinger.io

#### Working
'vnbv'

For Notifications 'Service' + 'number' will be the unique key.

- receive web request
- if new, generate color palette

### code
```
check and set mode

if lamp mode
  random pattern start
```
##### thinger.io
Define credentials
```
#define USERNAME "balsimpson"
#define DEVICE_ID "notiCloud"
#define DEVICE_CREDENTIAL "noticloud"
```
Declare variable
```
ThingerWifi thing(USERNAME, DEVICE_ID, DEVICE_CREDENTIAL);
```
##### wifi

```
#define SSID "Zion"
#define SSID_PASSWORD "wormwood"
```

**List of modes/actions**
- Reveal
  - backlight on
  - frontlight fade in
  - color?

- Chase
  - band of lights going around
  - number of leds is directly proportional to notification priority

- Lightning
  - random flashing
  - color mapped to time?

- Lamp palettes
  - load different color palettes
  - random rotation or fixed

- Notifications
  - color palette based on service icon
  - animation speed mapped to notification priority

- Timer based
  - weather - rain/ sunny/ humidity
  - sunset / sunrise / moonrise

- Gauge - button activated
(how to cycle through?)
  - RescueTime productivity
  - Moves activity level
  - Calendar appointments
  - ToDo list completion
  - Twitter/ Instagram follower count

Some way a log should be maintained of all the commands being executed with timestamp.

**Easy Control**

`Color` should be a manipulatable variable
`num_leds` should be a variable
`notification_priority`

[color palettes](http://www.fubiz.net/en/2015/04/20/the-colors-of-star-wars-palettes/)
