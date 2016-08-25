# conky_solar_burn
Conky theme with weather support and a spiffy layout:

![Screenie](solar-burn-conky-screenie.png)

---

### Dependencies:

- **[conky](https://github.com/brndnmtthws/conky)**  v1.10+, as the new config file uses Lua syntax
- **[apcaccess](http://linux.die.net/man/8/apcaccess)** for reading the *Load* level of the UPS
- (Proprietary) **[nVidia drivers](https://launchpad.net/~graphics-drivers/+archive/ubuntu/ppa)** for reading GPU status

### Installation:

- Copy the **.conky-google-now** and **.conkyrc** files to your home folder
- Install the included **Play** font in **~/.fonts/truetype/play**, then update your font cache with: **```sudo fc-cache -fv```**
- Copy the **logos/** folder anywhere, but *update the 3 references* within **.conkyrc** (**lines 65, 80, 87**) - the same can actually be done with the **.conky-google-now/** folder which contains the weather icons
 
### .conkyrc Required edits for personalized info:

- **[line 45]** Edit the Yahoo! Weather URL to search for your city, replacing **```%22toronto%22```** with **```%22YOUR_CITY_NAME%22```** (you can pop this URL in a browser to inspect the response)
- **[line 62]** Replace the hardcoded data
- **[line 65]** Edit the CPU name/family
- **[line 99-101]** Edit the disk paths
- **[line 103-105]** Edit the disks to monitor r/w speeds
- **[line 106-108]** Replace the **```eno1```** network interface with whatever yours is

### Notes:

- This layout was built for 1440p resolution, but you can adapt it to 1080p (or anything else really) by simply adding/removing some elements/lines
- The modified *conky-google-now* icons and code are from [satya164](http://satya164.deviantart.com/art/Conky-Google-Now-366545753)
- The current weather text in the preview is partially borked (reads "Mostly") -- this shouldn't be the case once you've updated the Yahoo! URL to your city
- The music text that is near the bottom, as well as the Prev/Stop/Play/Next buttons, are not from this Conky theme. They are from the **gmusicbrowser** Desktop plugin

### Donations from awesome people

It has taken me a long while to build and perfect this layout, so if you'd like, you can toss some **Bitcoin** my way to:

![Bitcoin and cryptocurrency rock!](icon-btc.png) **```1PaV8LVJTqwt23M9WXK4jcVu2Bp6rWHwnv```**

Thanks, and hope you enjoy!