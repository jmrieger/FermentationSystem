# FermentationSystem
Design of system for fermenting beer.  Eventually used in conjunction with FermentPi repo

## About FermentationSystem
This system is designed to control the temperature of beer fermentation tanks.  It's designed to replicate a glycol chilling system, but on a homebrew scale.  The components are all readily available from your local hardware store, as well as online sources (motorized valves, glycol, et al).  The core of the system will control temperature of a single vessel, however the system is expandable to support multiple vessels.  

Specifically, the FermentationSystem described here is the physical configuration of a fermentation control system.  A temperature control system must be used in conjunction with this system.  The intention is to use the FermentPi respository / system in conjunction with this project, however there's no reason the builder couldn't use other existing control systems (BrewPi, individual Ranco or STC controllers, BCS products, etc).  As the specific control system is outside of the scope of this repository, the builder must take that portion into consideration.

## Principles
A spare mini fridge is used as a cooling source for a glycol reservoir.  The project suggests a 6 gallon reservoir, as the intent is to support 3 separate fermentation vessels simultaneously.  Feel free to scale up or down as your individual build requires.  A pump is used to circulate the chilled glycol around the fermentation vessel to chill the fermenting beer inside.  The spent glycol is then returned to the reservoir, where it can be re-chilled.

## Inspiration
The build was inspired by this thread on http://homebrewtalk.com: (http://www.homebrewtalk.com/showthread.php?t=413406).  The variations come in the size / scale of my home brewery - I generally brew 6 gallon batches at the moment, but have the capacity for 12 gallon batches.  I didn't want to purchase 15 gallon plastic fermenters, nor deal with the internal chilling coils - I believe sanitizing the fermentation vessel is more reliable if the temperature control is external to the vessel (with the obvious tradeoff being that chilling with coils directly in the fermenting beer is likely more efficient.

## Contributions
Feel free to submit a pull request if you see any errors in the documentation or major design flaws.
