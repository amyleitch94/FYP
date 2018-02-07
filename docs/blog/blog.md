# Blog: NFC-ATTENDENCE TRACKER

**Amy Leitch**

## Blog 06/02/2018

I have watched NFC tutorials online, and today I attempted to practice some of them as well as creating a base app to work with.
This led to me realising that the Android Emulator in Android does not support NFC and I needed to research alternatives.
OpenNFC sdk seems to be the only solution, but their website is down and I cannot find the correct download. I am currently attempting to use my own phone to test some basic NFC functionality. 

My aim for this week is to complete a base app with NFC functionality that can be tested using the emulator, and then tested on my own device with NFC tags I purchased.


##Blog 07/02/2018

The following features have been implemented into the base app:
-Detect when devices NFC is on/off
-Detect when an NFC tag is tapped to device
-Ability to Write text to NFC tag - includes detecting when tag is unwritable
-Aility to Read text to NFC tag - includes detecting when there is nothing to read
-Ability to Lock the tag/make the tag Read Only (This needs to be worked on)

I also discovered a way to possibly changing the code so when a tag is tapped with no app open, the app will open. If the app is already open when the tag is tapped, then it reads the tag. I am unsure if I want this functionality yet.

While implementing these functions with the help of "NFC Tutorials" on Youtube, I learned about NdefMessage. 

"NDEF (NFC Data Exchange Format) is a light-weight binary format, used to encapsulate typed data. It is specified by the NFC Forum, for transmission and storage with NFC, however it is transport agnostic.

NDEF defines messages and records. An NDEF Record contains typed data, such as MIME-type media, a URI, or a custom application payload. An NDEF Message is a container for one or more NDEF Records.

When an Android device receives an NDEF Message (for example by reading an NFC tag) it processes it through a dispatch mechanism to determine an activity to launch."