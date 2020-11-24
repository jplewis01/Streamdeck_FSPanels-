# Streamdeck_FSPanels-
 StreamDeck Panels for FS2020 using Flight Stream plugins

This is the Beginnings of my efforts to integrate my StreamDeck XL into my FlightSimulator 2020 experience. I got the Streamdeck to fullfill a number of needs one being tpo experiment with it as a controller for a number of aspects of a flight simulator. I've not used external panels or built a cockpit before and may or may notin the future but thus far Streamdeck has me highly intrigued.
When I started out I was just leverage native streamdeck functionality to find out what was possible and found it to be functional and useful but still incomplete.
Enter FlightTracker and the plugin to allow more direct connectionto the simulator through Microsoft Simconnect connector. The rest is history (sort of).

As I just noted my first experiences with Streamdeck Drove the Simulator by simulating KeyStrokes just as the Keyboard does and it worked pretty but but had all the usual limitations. I perserved and built button and functionality to first drive the C152 then the C172 Glass cockpit complete with Autopilot. I got that working well and fashioned as set of useful Buttons and have been learning about what works for me and what doesn't. 

What this package contains is a my current (early C172 profile), a set of ICONs I'm currently using and the Ivery MESSY ICON template files I've constructed that have allowed me to build a bunch of small stanardized icon components that I recolor and reu-use as needed. I wanted an efficient capable image editor that did not take 2 years and a rocket science degree to learn to use. I settled on Paint.NET which can be purchased from the Windows App Store for like $6-$8. I'm working to cleanup the ICON Template files and further standarize their layouts. These are ICONs that work for me. If you don't like them, Create your own that fit your needs. I hope / plan to work with the Flight Tracker dev team to help improve their product and make it better than it already is.     

As far as possible as I converted over my Buttons from Hotkey switch to Flight Tracker Generic Toggles I've chosen to have the buttons show the control state i.e. dimmed grey for off and bright with an indicator in the top left showing on. I'm going for functional state rather than getting caught up in making it look like the button on the actual cockpit.

I derived the Button Toggle and feedback values using both FSUIPC7 and the List of toggle events events and values in the structs.cs file that Ngyuen and Pieter are creating as they implement new functions.Many of my current Autopilot function are built using the Preset Toggle and Increase / Decrease values. The Rest is just hacking up ICONS that a meaninglful.I found the capability to switch GPS to VOR for navigation and how to enable Localizer lock. both using the regular generic toggle. If you are struggling to make sense of what goes where then those two may point the way.
I used FSUIPC7 to tell me what EVENT the onscreen buttons triggered then scanned through the struct.cs file Toggle values to find what I thought would be it toggle value and dropped that into the Feedback value. Most times it worked fine but on some occassions it required some further experimentation to get it to work.

I am yet to implement a working gauge using Flight Tracker, partly because of time available and partly due to my own inexperience with the gauges. Rest assured when I get one to work I will shortly thereafter post up a sample and how-to details. 


I'm building my controls based on the StreamDeck XL. at this point I have no idea how scale down to the small units. Let me know if you know. This profile should import fine IF you have Flight tracker plugin installed already. 

Images are all .PNG files and most are 500X500 image size which seems to scale down well in the software.

The Template files are all in .PDN format which I think you'll need to Paint.net to read. 

Coming in a few days will be a cleanup of the Template files and I will be moving to more standard font sizes and screen layouts.
