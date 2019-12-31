# broadlink_sp4_customcomponent
First try for an integration of custom component with added broadlink sp4 support

This is a custom component, and a rough one at that. 

You will get a warning in your log about using an untested custom component,
and MANY posts in you log about status updates from the component working. 

This is not really a problem, but maybe not so pretty. 

But it helps any troubleshooting, so until there have been more testing, it will most likely stay for now. 



INSTRUCTIONS:

Copy directory sp4 into your directory custom_components in your config directory. (Thats alot of directorys... your config dir is where your configuration.yaml is. custom_components might need to be created if you have not done so already)

You also need to add this:

switch:
  platform: sp4
  
to your configuration.yaml.

Then there is configuration, now you need to add your devices in switch/sp4.py

In this python file there are lines with "EDIT" on the end, focus on these. In the file as uploaded there are two devices configured, guestroom and computercorner. Hopefully this should get you started, you can add or remove devices and auth if you have more or less devices.

This is of course not standard changing the python directly, nor is that the modded I/O lib for sp4 broadlink switch is included right there instead of as a dependency, but this works for now and is reasonably understandable?


