# Goal Zero-based second battery system

We use a [Goal Zero Yeti 3000X](https://amzn.to/3bpxnqB) to run our 12V system and our inverters. We can charge this by solar, shore power, or from the vehicle’s alternator while the vehicle is running. The benefit of this system for us is that it is largely all-in-one: it _may_ cost more than designing and building a custom system, but for us when we factored our time into the project costs, the all-in-one system made sense. 

I still learned a lot about these systems from faroutride.com, and I bought their 

## Charge source
We can charge this by solar with the [Goal Zero 200W solar panels](https://amzn.to/37ygdWH); using shore power; or using the vehicle alternator using the vehicle integration kit (waiting on link for this that is compatible with the 3000X, **a safety modification was made for the X series, so do not buy or use older versions of this hardware!**). 

### Alternator-based charging
Parts:
* [Male EC8 to Ring Terminal](https://www.goalzero.com/shop/power-station-accessories/male-ec8-ring-terminal/)
* 



#### Remove seat to access the battery compartment
The battery is installed under the driver’s seat. Unusual, but it fits well, so I can’t complain. 

**Before removing the seat, unplug the wiring harness under the seat from the front.** One #7 hex head screw holds the wiring harness in place under the driver seat. Unscrew that to loosen and unplug the wire harness (the screw shouldn't come all the way out; {numref}`wire-harness-1`).

```{figure} images/wire-harness-1.jpeg
---
name: wire-harness-1
---
View of driver seat wire harness after detaching. 
```

We have a swivel base installed. See the [faroutride.com swivel seat review](https://faroutride.com/swivels-review/) to learn more about these (we have Scopema swivels on the driver and passenger seats and we love them). Ideally you would connect your Goal Zero to the battery while doing the driver swivel seat install, but we were waiting on the 3000X-compatible vehicle integration kit to be developed when we installed the driver swivel. Easy enough to remove the swivel though - this will be the same thing we need to do any time we access the vehicle battery directly (remember that there are jump start terminals under the hood). 

##### Factory configuration
If you don’t have a Swivel base installed, start with [Christopher Lum’s video on removing the driver seat to access the battery compartment](https://www.youtube.com/watch?v=0SsDbT-J8cU). If you’re not already familiar with Christopher’s channel and you are working on a Ford Transit passenger van, you’re about to discover one of the most useful educational resources around! 

##### Scopema swivel base congifuration

The swivel base stays with the seat when you take it off. Four 3/16” Allen bolts are used to remove the swivel base to access the battery compartment ({numref}`scopema-screw-1`). (If you have a passenger swivel installed already, it makes working on the battery compartment very convenient b/c you’ll have a nice spot to sit while you’re working.) 

```{figure} images/scopema-screw-1.jpeg
---
name: scopema-screw-1
---
One of the four screws that you’ll need to remove to deattach the Scopema driver swivel to access the battery.  
```

##### Other swivel base configurations
I’ve never installed other swivel bases, but if I imagine it’s easy to figure out how to take others off (especially if you installed it). 

#### Connect to battery terminals and route cable

First, route the cable. I drilled a 1/2” hole through the rear plastic cover. Drill this hole from inside the battery compartment (or risk drilling into the metal framing). To pass the connector rings through, you’ll need to widen the hold a little after drilling - do that with a file, or just make a second hole. A bigger initial hole won’t fit (at least where I made it) due to the metal framing. Run the wire through the hole. 

```{figure} images/gz-battery-wire-port-1.jpeg
---
name: gz-battery-wire-port-1
---
New port for routing [Male EC8 to Ring Terminal](https://www.goalzero.com/shop/power-station-accessories/male-ec8-ring-terminal/).
```

Remove the #10 hex head nuts to connect rings to battery terminals ({numref}`battery-terminal-1`). Do this one terminal at a time, starting with the negative terminal. Obviously, be very careful when accessing the positive terminal in particular. If you create a path between the positive and negative terminals - especially if that path runs  up one arm and down the other with your heart in the middle - you’ll be sorry. 

```{figure} images/battery-terminal-1.jpeg
---
name: battery-terminal-1
---
Negative battery terminal with ring connected.
```

#### Put it all back together

```{figure} images/battery-compartment-1.jpeg
---
name: battery-compartment-1
---
The battery compartment after putting it all back together. Note that the cable for our wire harness comes through a new custom hole in the top of our plastic battery cover to allow for the Scopema driver swivel. If you don't have a driver swivel, you won't need to route your wiring harness this way.
```

### Shore power

### Solar

## 12V system

## Inverter (120V **?** AC system)

## Exterior lighting
We’re going to experiment with the [Goal Zero Light-A-Life 350 LED Lights](https://amzn.to/2NHvJbZ) for outdoor lighting. These are nice little lights, and we used them for internal lights before installing our recessed lights (they’re a little clunky for interior use, but they are versatile with hanging and magnetic options for mounting and two brightness levels). They also chain together, which is convenient. We’d like to be able to connect these through a port of some sort on the outside of the van - I’ll update if I figure that out. 



