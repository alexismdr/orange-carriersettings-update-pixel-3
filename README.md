# 🟧 Orange F : Update CarrierSettings
## Background
In June 2022, Google rolled out an [update](https://www.xda-developers.com/pixel-3-xl-volte-roaming-update/) allowing **Google Pixel 3 / Pixel 3 XL** phones to take advantage of **VoLTE** and **VoWiFi**. Many French operators like [SFR](https://www.sfrbusiness.fr/assistance/ma-telephonie-mobile/appels-wifi-sur-mobile.html#:~:text=PIXEL%203%20/%20PIXEL%203%20XL) and [Bouygues](https://www.assistance.bouyguestelecom.fr/s/article/volte-appel-4g#:~:text=Google%20Pixel%C2%A03%20%2C%C2%A0Google%20Pixel%C2%A03XL) have enabled the option on this phone. But, almost a year later, Orange France has not made a single update to allow Pixel 3 users to enjoy this option. To this day, Orange customer service recommends customers to switch phones. It is unacceptable to hear this from a brand that claims to be [environmentally friendly](https://www.orange.com/en/commitments/oranges-commitment/to-the-environment). It is certainly important to [recycle old phones](https://www.orange.com/en/give-your-phone-second-life-orange), but before that it is necessary to keep them as long as possible!

Also, Orange blocks the activation of more important options (such as **MultiSIM of connected smartwatches** like Pixel Watch) in the absence of VoLTE/VoWiFi on your phone for absolutely no reason. 
## What Orange France could do
Orange can activate this option in two simple steps:
1. Update the `orange_fr.pb` file (containing the carrier settings). They can do this even if the Pixel 3 is no longer receiving OEM updates by pushing the update via Carrier Services.
2. Add the Pixel 3 to their "Whitelist" of compatible IMEIs on their servers.
## Solution
While waiting for Orange to fix the problem one day, it is possible to fix it ourselves via a few very simple steps.
### Requirements
- A rooted Android device with [Magisk](https://github.com/topjohnwu/Magisk) v20.4+
- A [Orange VoLTE/VoWiFi whitelisted phone](https://reseaux.orange.fr/nos-reseaux/internet-fixe/appels-wifi) IMEI number
### Steps
1. Install latest module release from this repository.
2. Change Pixel 3 IMEI to a Orange VoLTE/VoWiFi whitelisted phone IMEI using [this guide](https://gist.github.com/uragiristereo/7668e067e3b0525d6e4d4b12d9f71344).
3. Enjoy 😁
## Additional information
### Other benefits
This module can also be used to simply update your carrier settings for another reason and on another phone model. For example, I have seen a significant improvement in network connectivity on my Pixel 3 XL since installing this module.
### Other devices
I don't guarantee it will work on other models than the Google Pixel since the operator configuration file was extracted from a Google Pixel 7 Pro image.
### Tested on
- Stock (Rooted) :
  - VoLTE : ✅ Working
  - VoWiFi : ✅ Working
- Pixel Experience (Official, Android 13) :
  - VoLTE : ✅ Working
  - VoWiFi : ❌ Not working, see : https://github.com/PixelExperience/android-issues/issues/5286
- PixelBuilds (Unity, Android 14) :
  - VoLTE : ✅ Working
  - VoWiFi : ❌ Not working (crosshatch maintainer is aware of the issue and will try to fix it)
