# Introduction (Zorba Is Sleep-Deprived Edition)

Hey, dude! Do you have an AUTOMATIC THERMOSTAT in your house? Is it good? No! No it isn't. It fucking sucks! How do I know that? It's because *all* automatic thermostats fucking suck!

Yeah! Even the Nest! You heard me. I'm calling you out, Nest. You suck.

See, here is the problem.

The modern thermostat does four things. First, it measures the temperature. Second, it acts as a user interface so people can tell it what decisions it should make. Third, it makes decisions. Fourth, it communicates with your HVAC system.

With the exception of the third, all of these functions are in tension with each other. To measure the temperature, it must be in a useful place to get useful temperatures; so, in bedrooms and living rooms, where people spend most of their time. But you don't want it in people's bedrooms because that's a bad place for a user interface. Also, sometimes it's useful to get ceiling temperatures, but obviously you can't put it on the ceiling and have people use it! Finally it needs to be close to your furnace, otherwise you have to run, like, too many wires, which is TERRIBLE because NOBODY WANTS TO DO THAT and the end result is that I have a thermostat in an upstairs hallway which nobody uses and which collects warm air like nobody's business and nobody cares that it collects warm air but nevertheless it dictates the climate of like *half the house* and it's awful and why is it done this way.

The reason it's done this way is, of course, that most people aren't totally nuts, and aren't interested in building like twenty different devices that are installed all over their house, but *good news, I'm here, I got this covered*.

# The Plan

The Anemoi Project is very much a work in progress. As of this writing I've purchased some parts; they're sitting in a box in the garage for me to get to them. Don't hold your breath.

My eventual plan consists of four major modules.

**Eos** is the module that connects to the furnace. This will be a minimal construction with a few relays on it, likely supporting Ethernet (maybe PoE) and intended to be plugged in permanently. It has no user interface.

**Astraeus** is the system that decides what to do. This may be hosted on Eos, or it may be standalone in a Docker container on some other home server. I frankly have not decided.

**Minerva** is the user interface for the entire system. I currently plan for this to be an HTML/JS interface hosted on Astraeus.

**The Anemoi** are the first part I plan to build. These are a fleet of small inexpensive wifi-enabled USB-powered sensors. I'm building them cheaply on NodeMCU devices and spreading them throughout the house; I'm currently planning to deploy about two dozen of them.

That's the plan.

Maybe I can get to work on it in a few weeks!