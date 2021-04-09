# Pi-hole on ink 

Display the **number of blocked requests, and filtered traffic**, from [Pi-Hole](https://pi-hole.net), on [Pimoroni's Inky-Phat](https://github.com/pimoroni/inky-phat/issues).

- Setup **Pi-Hole**, follow the [installation instructions](https://learn.adafruit.com/pi-hole-ad-blocker-with-pi-zero-w/install-pi-hole).
- Setup **InkyPhat**, follow the [installation instructions](https://learn.pimoroni.com/tutorial/sandyj/getting-started-with-inky-phat).
- Clone this repo on your [Raspberry Pi Zero W](https://www.raspberrypi.org/products/).

## Reload automatically every n minutes

Edit `crontab`. 

```
crontab -e
```

Add the following line:

```
*/n * * * * python /home/pi/inky-hole/main.py
```

## python3 main.py > no module 'urllib2'

Use python2 or nano the main
```
urllib2 -> urllib
```

## Change pi.hole/admin 

```
pi.hole/admin -> aeo.uae.oua.eox/admin
```

Enjoy.

<img src='https://raw.githubusercontent.com/nuoxoxo/pihole-on-ink/master/00.jpg' width="64%"/>


