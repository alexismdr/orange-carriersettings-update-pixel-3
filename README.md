# 🟧 Orange F : Update CarrierSettings
## Background
In June 2022, Google rolled out an update allowing **Google Pixel 3 / Pixel 3 XL** phones to take advantage of **VoLTE** and **VoWiFi**. Many French operators like SFR and Bouygues have enabled the option on this phone. But, almost a year later, Orange France has not made a single update to allow Pixel 3 users to enjoy this option. To this day, Orange customer service recommends customers to switch phones. It is unacceptable to hear this from a brand that claims to be environmentally friendly. It is certainly important to recycle old phones, but before that it is necessary to keep them as long as possible!

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
This module can also be used to simply update your carrier settings for another reason and on another phone model. For example, I have seen a significant improvement in network connectivity on my Pixel 3 XL since installing this module.
I don't guarantee it will work on other models than the Google Pixel since the operator configuration file was extracted from a Google Pixel 7 Pro image.
