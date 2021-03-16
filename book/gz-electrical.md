(gz-install)=
# Goal Zero-based second battery system

```{figure} images/gz/installed-gz-1.jpeg
---
name: installed-gz-1
---
The "finished" project (as if any van project is ever finished). 
```

We use a [Goal Zero Yeti 3000X](https://amzn.to/3bpxnqB) to run our 12V DC system and our 120V AC inverters ({numref}`installed-gz-1`). We can charge this by solar, shore power, or from the vehicle’s alternator while the vehicle is running. A benefit of this system is that it is largely all-in-one. Throughout this document I refer to the Goal Zero Yeti 3000X unit as _GZ_. 

The cost for an all-in-one system, as of fairly recently, seems relatively similar to designing and building a custom system. When we factored our time into the project costs, the all-in-one system made a lot of sense to us.

```{warning}
I learned a lot about these systems from faroutride.com. I bought their [Wiring Guide and Tutorial](https://faroutride.com/store/wiring-diagram/) and found it very helpful even though they have a custom-built electrical system (opposed to our all-in-one system). They cover important safety points that I don't cover in detail here, such as choosing wire gauge and fuse size for the 12V system. Learning about their system made the GZ less of a mysterious black box for me. Their guide was well worth the money for me (especially considering how much time and money they saved me on other projects).
```

## Inputs (how we charge this thing)
We can charge this by solar with the [Goal Zero 200W solar panels](https://amzn.to/37ygdWH); using shore power; or using the vehicle alternator using the [Yeti Link vehicle integration kit](https://www.goalzero.com/shop/yeti-accessories/yeti-link-expansion-module/) (see Yeti Link Car Mode on that page). Details on each of these charging mechanisms (with the exception of solar - that's not installed yet) are presented in the following subsections. 

```{warning}
A safety modification was made to the vehicle integration kit for the X series. Do not buy or use older versions of this hardware!
```

### Alternator-based charging

Parts:
* [Male EC8 to Ring Terminal](https://www.goalzero.com/shop/power-station-accessories/male-ec8-ring-terminal/)
* [EC8 12FT Extension Cable](https://www.goalzero.com/shop/accessories/ec8-12ft-extension-cable/)

#### Remove seat to access the battery compartment
The battery is installed under the driver’s seat. Unusual, but it fits well, so I can’t complain. 

**Before removing the seat, unplug the wiring harness under the seat from the front.** One #7 hex head screw holds the wiring harness in place under the driver seat. Unscrew that to loosen and unplug the wire harness (the screw shouldn't come all the way out; {numref}`wire-harness-1`).

```{figure} images/gz/wire-harness-1.jpeg
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

```{figure} images/gz/scopema-screw-1.jpeg
---
name: scopema-screw-1
---
One of the four screws that you’ll need to remove to deattach the Scopema driver swivel to access the battery.  
```

##### Other swivel base configurations
I’ve never installed other swivel bases, but if I imagine it’s easy to figure out how to take others off (especially if you installed it). 

#### Connect to battery terminals and route cable

First, route the cable. I drilled a 1/2” hole through the rear plastic cover. Drill this hole from inside the battery compartment (or risk drilling into the metal framing). To pass the connector rings through, you’ll need to widen the hold a little after drilling - do that with a file, or just make a second hole. A bigger initial hole won’t fit (at least where I made it) due to the metal framing. Run the wire through the hole. 

```{figure} images/gz/gz-battery-wire-port-1.jpeg
---
name: gz-battery-wire-port-1
---
New port for routing [Male EC8 to Ring Terminal](https://www.goalzero.com/shop/power-station-accessories/male-ec8-ring-terminal/).
```

Remove the #10 hex head nuts to connect rings to battery terminals ({numref}`battery-terminal-1`). Do this one terminal at a time, starting with the negative terminal. Obviously, be very careful when accessing the positive terminal in particular. If you create a path between the positive and negative terminals - especially if that path runs  up one arm and down the other with your heart in the middle - you’ll be sorry. 

```{figure} images/gz/battery-terminal-1.jpeg
---
name: battery-terminal-1
---
Negative battery terminal with ring connected.
```

#### Put it all back together

```{figure} images/gz/battery-compartment-1.jpeg
---
name: battery-compartment-1
---
The battery compartment after putting it all back together. Note that the cable for our wire harness comes through a new custom hole in the top of our plastic battery cover to allow for the Scopema driver swivel. If you don't have a driver swivel, you won't need to route your wiring harness this way.
```

Once it's all back together, you can connect the EC8 12FT Extension Cable from the outside of the battery compartment. 🎉

### Shore power

Parts:
 * [Power inlet](https://amzn.to/3sVFdPU)
 * [Recessed Power Strip](https://amzn.to/3rqV2xN)

```{figure} images/gz/inlet-1.jpeg
---
name: inlet-1
---
The inlet allows us to charge from shore power by plugging into a typical 120V AC outlet (e.g., at home, a campgound, etc). See faroutride.com for install instructions.
```

The one inlet splits to two outlets.

The first of these (SH1) we use to charge the GZ unit. 

To the second of these (SH2) I daisy-chained two recessed power strips. This gives us one outlet in our kitchen which provides the AC to the fridge and two outlets in our bed-side cabinet. (Our fridge connects to both our shore power system and our 12V system. When connected to shore power, the fridge will draw from that instead of from the 12V system.)

One inlet splits to two outlets:
 1. Shore outlet 1 (SH1): Goal Zero AC charging
 2. Shore outlet 2 (SH2): Kitchen outlets
    1. Fridge AC power
    2. Bedside cabinet outlets (daisy-chained)
        1. Open
        2. Open

### Solar

Parts:
 * [Goal Zero 200W solar panels](https://amzn.to/37ygdWH)

Not installed yet, but connects directly to GZ. We'll be installing a roof rack and mounting solar on that. Right now I pull the solar panels out when I need to charge by solar. It's miserable, and they are a huge pain to travel with when they're not mounted. Mounting these will be my next project, once my project bank account recovers enough for me to buy a roof rack.

## Outputs (how we discharge this thing)

### 12V system

Parts:
 - [Ring terminals to Anderson connections](https://amzn.to/3bCADis) - connects fuseblock to GZ
 - [Fuse block](https://amzn.to/2Mzpjvg)
 - [Fuse kit](https://amzn.to/3bJa3V8)
  - 12V DC loads (see https://faroutride.com/van-build/learn/electrical-system/)
  - Fridge: we have a [Nova Kool](https://www.novakool.com/) [R3100](https://www.novakool.com/r3100-1) AC/DC - it runs great from the GZ, we couldn't be happier with it

12V fuse block ({numref}`fuse-block-1`) - numbers are etched down center of fuse block, they run left-to-right, top-to-bottom
 1. Ceiling vent fan (10A fuse)
 2. Ceiling LEDs (3 total; runs into header from behind fridge; 2A fuse)
 3. Driver-side (i.e., kitchen) 12V outlet (5A fuse)
 4. Currently unused
 5. Passenger-side header ([USB A/C outlet](https://amzn.to/3rOC6t2) and small fan - 7.5A fuse) 
 6. Currently unused
 7. Toilet fan (3A fuse)
 8. Currently unused
 9. Passenger-side (i.e., bedside) outlet (5A)
 10. Currently unused
 11. Fridge (15A)
 12. Currently unused

The fuse block mounts really nicely on the GZ battery compartment with velcro ({numref}`fuse-block-2`). If you want to mount it somewhere else, you'll need longer Anderson connection wires. 

```{figure} images/gz/fuse-block-1.jpeg
---
name: fuse-block-1
---
12V fuse block, not fully wired. The fuse block cover is on the right. Labeling the wires with a Sharpie is helpful when routing wires, and to facilitate future maintenance that might require disconnecting wires from fuse block. 
```

```{figure} images/gz/fuse-block-2.jpeg
---
name: fuse-block-2
---
12V fuse block velcro'ed to GZ. (There's some velcro on the front too - I used to have it mounted there, but the side ended up being more convenient for my final configuration.)
```

#### 12V System Loads

These photos give an idea of how I did the wiring in the header. I used a box cutter with a brand new blade to make cutouts for fixtures. It worked great. Pull the whole headliner out to work on if you have enough space. I have a rolling 4'x8' workbench in my wood shop, which is convenient for working on this. Alteratively, a couple of saw horses and two 8 or 12 foot 2"x4"s should support it well too. Or just work on one section at a time.

```{figure} images/gz/12v-loads-1.jpeg
---
name: 12v-loads-1
---

```

```{figure} images/gz/12v-loads-2.jpeg
---
name: 12v-loads-2
---

```

### 120V AC Inverter

Parts:
 * [Recessed Power Strip](https://amzn.to/3rqV2xN)
 * [1L electric tea kettle](https://amzn.to/3sSwVZc) (this draws a lot of power, but it sure is nice to be able to make our first [cup of coffee](https://amzn.to/2PHc9xp) of the day without turning our camp stove on!)

There are two 120V AC outlets on the GZ unit. 

To the first of these (GZAC1), I daisy-chained two recessed power strips. This gives us one outlet in our kitchen cabinet and two outlets in our bed-side cabinet. 

I leave the second of these (GZAC2) open so I can connect loads directly to it when needed. This has been really convenient for powering tools while working on the build. s

Two GZ outlets:
 1. GZAC1: Kitchen outlets
    1. Open (usually used for our tea kettle)
    2. Bedside cabinet outlets (daisy-chained)
        1. Open
        2. Open
 2. GZAC2: open 
    

### Exterior lighting
We’re going to experiment with the [Goal Zero Light-A-Life 350 LED Lights](https://amzn.to/2NHvJbZ) for outdoor lighting. These are nice little lights, and we used them for internal lights before installing our recessed lights (they’re a little clunky for interior use, but they are versatile with hanging and magnetic options for mounting and two brightness levels). They also chain together, which is convenient. We’d like to be able to connect these through a port of some sort on the outside of the van, maybe when we run wires for the solar. I’ll update this if I figure that out, and once we have a little more experience with these lights.

## Mounting

We mounted the GZ to its 3/4" plywood shelf by using the nuts built-in to the bottom of the GZ unit. I first figured out the hole pattern on a piece of scrap wood, and then used that as a template for the drilling the holes on the final shelf. Here's a couple of views of the unit mounted to the scrap wood. 

```{figure} images/gz/gz-mount-1.jpeg
---
name: gz-mount-1
---
GZ mounted to work cart (side-view). 
```

```{figure} images/gz/gz-mount-2.jpeg
---
name: gz-mount-2
---
GZ mounted to work cart (bottom-view). The eye bolts let me tie it down if needed. 
```

I also put some casters on the scrap wood to make a little cart for the unit to use while I was doing the install. This unit is heavy so I found it convenient to have a little cart for it. Plus it made me feel like I had a little droid to hang out with while I working, so that's a bonus. I had the casters on-hand already, and had already drilled the holes to test my hole pattern. I wouldn't have built this cart just for its own purpose, but I'm glad I have it.

```{figure} images/gz/gz-mount-3.jpeg
---
name: gz-mount-3
---
GZ-PO (i.e., GZ mounted to work cart). 
```

## System controls

You can connect to the GZ by wifi or bluetooth with the GZ app. It seems to work reasonably well so far. This allows you to monitor input and loads, as well as turn systems on and off. Pretty cool! 

```{figure} images/gz/gz-app-1.jpeg
---
name: gz-app-1
height: 400
---

```
