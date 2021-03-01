# Goal Zero-based second battery system

```{figure} images/installed-gz-1.jpeg
---
name: installed-gz-1
---
The "finished" project (as if any van project is ever finished). 
```

We use a [Goal Zero Yeti 3000X](https://amzn.to/3bpxnqB) to run our 12V system and our inverters ({numref}`installed-gz-1`). We can charge this by solar, shore power, or from the vehicle’s alternator while the vehicle is running. The benefit of this system for us is that it is largely all-in-one: the cost now seems relatively similar to designing and building a custom system. When we factor our time into the project costs, the all-in-one system makes a lot of sense to us. 

I still learned a lot about these systems from faroutride.com. I bought their [Wiring Guide and Tutorial](https://faroutride.com/store/wiring-diagram/) and learned a lot from it. Well worth the money (especially considered how much time and money they saved me on other projects).

```{tableofcontents}
```

## Inputs (how we charge this thing)
We can charge this by solar with the [Goal Zero 200W solar panels](https://amzn.to/37ygdWH); using shore power; or using the vehicle alternator using the vehicle integration kit (waiting on link for this that is compatible with the 3000X. 

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

Once it's all back together, you can connect the EC8 12FT Extension Cable from the outside of the battery compartment. 🎉

### Shore power

```{figure} images/inlet-1.jpeg
---
name: inlet-1
---
The inlet allows us to charge from shore power by plugging into a typical 120V AC outlet (e.g., at home, a campgound, etc). See faroutride.com for install instructions.
```

One inlet splits to two outlets:
 - Shore outlet 1 (SO1): Goal Zero AC charging
 - Shore outlet 2 (S02): 
    - Cabin shore outlet 1:
        - Cabin shore outlet 2
        - Fridge

### Solar

Not installed yet, but connects directly to GZ. We'll be installing a roof rack and mounting solar on that.

## Outputs (how we discharge this thing)

### 12V system

Parts:
 - [Ring terminals to Anderson connections](https://amzn.to/3bCADis) - connects fusebox to GZ
 - [Fuse block](https://amzn.to/2Mzpjvg)
 - [Fuse kit](https://amzn.to/3bJa3V8)
  - 12V DC loads (see https://faroutride.com/van-build/learn/electrical-system/)
  - Fridge: we have a [Nova Kool](https://www.novakool.com/) [R3100](https://www.novakool.com/r3100-1) AC/DC - it runs great from the GZ, we couldn't be happier with it

12V fuse block ({numref}`fuse-block-1`) - numbers are etched down center of fuse block, they run left-to-right, top-to-bottom
 1. Ceiling vent fan (15A fuse - is this too high?)
 2. Ceiling LEDs (runs into header from behind fridge)
 3. Driver-side (i.e., kitchen) 12V outlet (15A fuse)
 4. Currently unused
 5. Passenger-side header (one 12V outlet, small fan - 5A fuse, may turn out to be too small) 
 6. Currently unused
 7. Toilet fan (5A fuse - probably too big)
 8. Currently unused
 9. Passenger-side outlet (splits to mutli-outlet charging station - 15A)
 10. Currently unused
 11. Fridge (15A)
 12. Currently unused

Fuse block mounts really nicely on the front of the GZ battery compartment with velcro ({numref}`fuse-block-2`). If you want to mount it somewhere else, you'll need longer Anderson connection wires. I can't really think of a reason I'd want to mount the fuse block somewhere else though. 

```{figure} images/fuse-block-1.jpeg
---
name: fuse-block-1
---
12V fuse block, not fully wired. The fuse block cover is on the right. Labeling the wires with a Sharpie is helpful when routing wires, and to facilitate future maintenance that might require disconnecting wires from fuse block. 
```

```{figure} images/fuse-block-2.jpeg
---
name: fuse-block-2
---
12V fuse block velcro'ed to GZ. The fuse block cover is off in this photo.
```

#### 12V System Loads

These photos give an idea of how I did the wiring in the header. Use a box cutter with a brand new blade to make cutouts for fixtures. Pull the whole headliner out to work on if you have enough space. I have a rolling 4'x8' workbench in my wood shop, which is convenient for work on this. Alteratively, a couple of saw horses with two 8 foot 2"x4"s should support it well too. Or just work on one section at a time.

```{figure} images/12v-loads-1.jpeg
---
name: 12v-loads-1
---

```

```{figure} images/12v-loads-2.jpeg
---
name: 12v-loads-2
---

```

### 120V AC Inverter
Two GZ outlets:
 - GZAC1: 
    - Kitchen outlet
    - GZ AC2:
        - Device cabinet outlet 1
        - Device cabinet outlet 2
 - GZAC2 outlet
    

### Exterior lighting
We’re going to experiment with the [Goal Zero Light-A-Life 350 LED Lights](https://amzn.to/2NHvJbZ) for outdoor lighting. These are nice little lights, and we used them for internal lights before installing our recessed lights (they’re a little clunky for interior use, but they are versatile with hanging and magnetic options for mounting and two brightness levels). They also chain together, which is convenient. We’d like to be able to connect these through a port of some sort on the outside of the van - I’ll update if I figure that out. 



