---
title: Airplay 2 audio with an Ethernet only Airport Express 
date: 2018-11-26T11:15:00-07:00
summary: How to use your Airport Express as an Airplay Audio hub
tags: 
- Apple
- technology

---

# Airplay 2 audio with an Ethernet only Airport Express 

It had slipped my radar that [Apple had release a new firmware update for their Airport Express product](https://support.apple.com/kb/DL1975?locale=en_US). The major feature in the updated 7.8 firmware is that it adds Airplay 2 support to the Express. I've been wanting to upgrade my home music stereo system for sometime but don't want to shell out the money for a HomePod. A [TidBits article reminded me about the Home app](https://tidbits.com/2018/08/28/apple-adds-airplay-2-to-the-discontinued-airport-express/) and from there the wheels got turning in my head.

The HomePod, by all accounts, "sounds" amazing but the fact that it is a single user device when it comes to the Siri features ("check my email") seems like a real drawback when the thing is going to live smack-dab in the middle of my living room with family of five Apple users.

Airplay 2 seems pretty cool particularly the ability to stream music to multiple AirPlay devices at the same time. Our current "home speaker" is usually our Apple TV playing music through our TV speakers over HDMI. It is not great but it works and it is easy for everyone to use... for the most part.

I just so happen to have an Airport Express lying around, not used. We retired our Airport-based WiFi network after years of Apple neglecting it and the performance being subpar giving our home's fast fiber connection. The interesting thing about the Express is that you can disable the WiFi radio, put the device into "bridge mode", and just plug into your existing router with an ethernet cable. 

With that in mind I plugged a pair of old computer speakers that sound reasonably decent into the Airport Express optical audio input. I updated the device's firmware and used the Airport Utility to configure it as an ethernet-only AirPlay hub as noted. Then I used the Home app on iOS 12 to add it as HomeKit device. This was a little finicky but I had to "Add an Accessory", then select the manual "I don't have a HomeKit code" option. It took a few tries but the Express device did show up and was added in a just few seconds. I added it to same HomeKit room as my Apple TV (which is also in the same "main floor" zone.)

From there I went back to my Phone's Music app picked a song and was able to tap both speaker options and music was streaming at the same time with no lag from both my Apple TV and the Express speaker output. It is pretty amazing. I suspect this setup will not work if I wanted to say watch a movie on my Apple TV and have the Audio come out of both places but I'm going to mess around and see if I can get it to work.

*Update:* I'm not sure what I was thinking about audio not working from both sources during movies - it works just fine and there was nothing else required. A nice little bit of Apple magic.
