# Spooky AC-130U

This plane comes from the USAF mod, so rearming can be done either through ACE or the USAF Mod service menu which can be accessed through the missile racks\[or mission editor placed stuff].

There are 7 seats available in this plane,

1. Pilot - Flys the plane
2. Co-Pilot - Blasts any modern music\[2000>]
3. Flight Engineer - Just sits there for now, questioning life
4. IR Operator - Controls all 3 guns
5. TV Operator - Controls a weapons systems which is chosen using the Scroll wheel menu\[Either the GAU or the Howitzer]
6. One Electronics Warfare Operator - Spoofs radar-guided missiles and other radar systems
7. Navigator Seat - Supposed to navigate but currently does fuck all.

**Suggested seating arrangement -> One Pilot\[will switch to TV operator once autopilot is engaged] and One IR Operator.**

## Flying

Does not handle like the RHS C-130, it is far more heavier considering the fact it has 3 big-ass fuck you weapons namely the GAU, L60 Bofors 40mm Cannon and the M105 Howitzer.

A slightly larger runway is required at half flaps or deploy full flaps. Start to pitch the nose up at around 150km/h, but not too high otherwise the aircraft will stall shortly after takeoff. After takeoff maintain a climb of 300feet/min or a pitch of 1-3 degrees upwards.

One thing to note is that the HUD is quite small so while using TrackIR or VR keep your head still otherwise you won't be able to see what is on the hud.

![Heads-Up Display](https://gitlab.com/Detachment207Hawkeye/Detachment207Hawkeye.gitlab.io/raw/master/static/hud.jpg)

While landing two lines will pop on the HUD which shows the deviation of the plane from the start of the runway. The horizontal line represents height offset while the vertical line represents horizontal offset. Try to keep them in the centre as they help in making sure you are on the correct approach angle. and make sure you are on full flaps as the speed will be decreasing drastically.

Reference the above picture for landing, those scaled vertical and horizontal lines only appear on full flaps and gear down.

If still slightly confused ask Alien to fly with you.

### Autopilot

The autopilot can be activated via the scroll menu. **The moment the autopilot screen pops up the throttle control is lost so activate it around 500m AGL.** A screen will appear with a map and 3 fields to be entered namely height ASL, radius of turn and speed to maintain.

There is a fourth field which gives how height AGL for the plane. Keep that in mind while inputting the flight altitude as it should not be negative or too low.

A sweet spot is 1000m ASL, 1200m radius turn and 305 km/h. Beware you will be in AA range. I'll find another spot which will keep the plane safe from AA.

The point to fly in a circle has to be marked on the map. Basicallt right-click on the map, hold and move the mouse a bit. There may be some offset so you can change the centre of the turn by clicking on the marker and moving it around. Only one center point can be chosen at a time.

There are two options on the right, one for turn direction and another for turning on the autopilot. Choose a counter-clockwise\[_CCW_] turn as the guns are on the left side. When everything is set turn on the autopilot. Currently there is a small bug where the autopilot does not work if the set altitude is less than the current altitude of the plane.

The autopilot can be activated from anyhwere after takeoff as a waypoint is set by the mod for the plane to reach and go into a loiter position at the specified parameters. Even when orbiting a certain point, the autopilot parameters can be changed without switching to the pilot's seat.

There needs to be at least one empty seat for the autopilot to start functioning, so we can have at least one person inside the plane apart from the pilot.

![Autopilot Settings](https://gitlab.com/Detachment207Hawkeye/Detachment207Hawkeye.gitlab.io/raw/master/static/autopilot\_settings.jpg)

Recommended Autopilot Settings

| Height ASL | Turn Radius |  Speed  |
| :--------: | :---------: | :-----: |
|    1000    |     1500    |   305   |
|    1500    |     2500    | 250-300 |
|    1500    |     2000    |   305   |

### Side Hud

This is to be used by the pilot to keep a reference marker in the center of the turn. I'll insert a picture and explain everything or I can just use the one from the Steam workshop page.

![Side Hud](https://steamuserimages-a.akamaihd.net/ugc/1622941034166258685/B19EB5EC69F37284554018B930BF373E277C4FAA/?imw=5000\&imh=5000\&ima=fit\&impolicy=Letterbox\&imcolor=%23000000\&letterbox=false)

This comes more into play when the all seats on the plane are staffed. It can get quite disorienting while using it, so not recommended.

### Tac Map

Still need to test this out.

## Countermeasures

### Thermal

While flying the pilot is in control of the thermal countermeasures. There are different modes with each corresponding to different number of flares released in a set number of seconds.

While in auto-pilot mode the flares are released automatically by the plane. It takes the medium/highest setting. There are about 500-600 flares so don't worry about running out of them while in the air, but do restock them upon landing.

### Electronic

Currently the plane does not hold any radar spoofing chaff. Instead there is an Electronics Warfare seat in the plane which can be used to spoof radars of any AA threat. Jamming of radar guided missiles does not work. There was a video by the USAF mod team for ECM jamming but it is no longer available.

## Weapon Systems

For multiple weapons systems to be used at the same time, one gunner should be present, preferrably in the TV operators seat. The IR operator can be the pilot when the autopilot is activated.

Ah the big guns come out. So there are 3 guns which are controlled by the IR operator. There is a TV operator seat which can take control of a gun through the scroll wheel menu. The pilot\[TV Operator] and IR Operator will ahve to decide who controls which gun.

As the calibre of the round increases the inaccuray or the offset of the gun increases, so the most accurate is the GAU and the least accurate is the Howitzer.

For automatically ranging the weapons, first switch on the laser, switch to any gun and press T. The gun systems will automatically range themselves.

Each gun system has an offset as compared to the orientation of the plane. This offset appears on the HUD as a circle with 4 perpendicular lines on it. The offset marker is both horizontally and vertically inverted. There is a weapons limit which is reached if the gun is pointed to much to any side. **WPN LIMIT** text appears on the bottom of the reticule if the limit is reached and the rounds become very inaccurate beyond this point.

The speed of the aircraft and the distance from the target also decide the offset of the weapons system. Do not expect pin-point accuracy like in COD/Battlefield. There is _some major deviation_ for the larger rounds with increased speed and/or distance from target.

The mortars and howitzer need some leading up to the target while the GAU is fairly accurate.

|      Weapon     | Number of Rounds |     Types of Rounds     |
| :-------------: | :--------------: | :---------------------: |
|      GAU-12     |       2000       |      High Explosive     |
| 40mm L60 Bofors |       256x2      | High Explosive/SABOT AP |
|  M105 Howitzer  |        100       |      High Explosive     |

### GAU-12

Something similar to the gun present on the A-10. It has three burst modes, 25, 50 and 100. 100 is a bit of an overkill, while 25 and 50 are nice. This gun can used against infantry, MRAP type vehicles and for immobolising armoured threats. can take out the gun and turret in the 25 round burst.

The guns lands the rounds wherever the camera is pointing, unless the weapon limit is reached.

### L60 Bofors

A 40mm mortar round is fired. Here the offset of the gun as compared to the plane comes into effect. There are two ammunition types which can be changed using the scroll wheel menu. Each type has the same number of rounds.

This gun system is useful againt lightly armoured targets, and immobility kills against heavily armoured targets. This gun also exploded a Tu-95 Bear\[though it may have been damaged from a gun run before]. Can also be used against large groups of infantry.

There are 2 types of rounds for this, High Explosive and SABOT Armour Piercing. They can be interchanged using the scroll wheel menu.

### M105 Howitzer

Has the capability to destroy anything it touches. Takes multiple hits but does the job effectively. The offset has a larger effect on the round impact than on the other two weapons systems.

It only has one type of ammunition and does take time to load. An automated voice script yelling _Gunner_ plays when the howitzer has finished loading.

## Overt Laser Designator

This requires the [A3TI](https://steamcommunity.com/sharedfiles/filedetails/?id=2041057379) mod to be loaded in by the player and the laser of the camera to be turned on. It basically creates a beam of light ending at the point where you are looking at. Press "_L_" to activate and "_L.Ctrl + L_" to toggle between pulsing and steady glow.

This comes in handy for pinpointing targets/HVT on the ground. Beware that if the enemy has night-vision, you are lighting yourself up for easy target practice.
