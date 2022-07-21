# Advanced and Simple Flight Model in Arma 3

This document will contain the elements of both Advanced and Simple flight models, how each should be used and transition between each.

In Arma 3 the pitch of the blades changes automatically both in AFM and SFM, the game engine calculates the pitch needed to maintain a standard RPM for the main and tail rotors.

I am not sure how the altitude affects the helicopter in each flight model, as we never fly that high anyhow. We will have to find a map which is that high to test it out.

## Simple Flight Model

This is the _default flight model_ which exists in Arma 3. It's good for basics and when flying with a keyboard and mouse. It can also be configured for when flying with a HOTAS.

### Collective

It is uses a _fixed_ collective, i.e., that the helicopter remains at the same height unless the collective is either raised or decreased. It's quite useful in maintaining a _hover in one place_ while fast-roping players onto the ground as the game engine will not simulate a settling with power while the helicopter is one place.

The pitch of the blades can be seen changing while decreasing/incresing the collective, but it does not have that much of an impact as the rate of ascent/descent is only changed. The longer the press, the more the change. I think the only impact of the blade pitch comes when the pilot is doing auto-rotation.

### Pitch, Roll and Yaw

Depends upon the airframe slightly. If the airframe is light enough, a small change in either of the three can increase the deviation of the flight path from your intended flight path. Heavier the air frame, more time taken for the effect to take place so be careful while changing either of the three axes. Too much input for any axis without any correction will make the helicopter go into a salsa dance. You do not want the **salsa dance**.

### Torque Effect

SFM Physics is _not_ real life physics. The moment of inertia is not modelled by the game engine while flying in SFM. So no matter how much collective is applied, the helicopter does not spin like a pole dancer. The only time that happens is when the pilot looses their tail rotor. Then pray to the casting couch god that you will land safe and sound.

### Wind Effects

A simple resistance effect is modelled. It will simulate the helicopter slowing down while in level flight due to air resistance. That's about it.

### Wheels

They are treated like skis, so do not land too fast otherwise the helicopter will be launched into the stratoshpere.

### Stress Damage

Not modelled, but land gently like how a cat lands. Do not land like a superhero, you and the chopper are not Hulk and given Arma's physics, it will be anyone's guess what will happen to you. Mostly you will go out in an explosion.

### Gauges

The gauges are present in all helicopters. Some can be read and some cannot. Most of the time they are out of our field of vision, so sit slightly raised and look slightly down if you want the gauges to be present at all times.

There is a mod we can use which will give a helmet mounted display for all choppers. We can use that in helicopters which do not have an in-built HMD.

For speed in km/h and altitude above ground level use the info bar which pops up when the pilot boards the helicopter.

### Auto-Rotation and Tail Rotor Loss

Basic aim is to land with the slightest damage to the helicopter. In case the other systems go yellow, that's fine and acceptable, just fix up the red parts and come back to base. In case the entire helicopter has gone red, and you still haven't exploded, land as fast as possible so that you can fix up your fuel tank.

SFM also has a smaller margin compared to AFM for skidding. So in both Auto-Rotation and Tail Rotor loss land at less than or equal to 20 knots\[40km/h].

#### Auto-Rotation

To safely return to the ground in SFM the pilot needs to maintain the energy and RPM of the rotors until the pilot needs to release that energy at the very end to arrest the descent and make a soft touchdown. The energy and RPM of the blades are co-dependent on each other.

This energy state can be monitored by the sound the blades make, the amount of motion blur on the blades as well as some helicopters having an engine RPM instrument (keep it to 60% or higher). If the sound becomes too low and quiet and the motion blur of the blades decreases then you are entering a failed state and the energy in the rotors has reduced to a dangerous level. If this continues then the blades may not be able to be brought up to speed and you will fall out of the sky.

You helicopter has energy in the form of speed and altitude. Use this energy bank to balance the amount of energy in the blades (their RPM), your forward speed and your rate of decent.

**Steps to Follow**

1. As soon as the engines are lost, drop collective and pitch up to either level with horizon or higher to reduce forward airspeed and increase motor RPM. If the pilot looks at the blades, it should feel like as if they are on full collective. Keep a forward airspeed and do not bother about the rate of descent, you are dropping like a stone anyhow, all you are trying to make sure is that you only compress your character's spine and not break it.
2. If the motor RPM is decreasing, pitch the nose forward slightly, gain some airspeed and descent rate and then pull back on the stick to bring the nose level with the horizon.

This part comes from _intuition and practice_. Practice can help in obtaining intuition.

1. At a certain altitude above ground level, pull back on the stick and raise the collective slowly. The pitch of the blades will change and push air down. This downward thrust will counter-act the stone dropping of the helicopter and allow the pilot to land the helicopter. Recommended airspedd and altitude is 30km/h and 30m respectively.
2. If the pilot is too high and applies full collective, the main rotor will slow down as it will loose all it's momentum in just fighting against air resistance. In this case, decrease collective like a madman and pitch 5 degrees nose up. The pitch combined with zero collective allows the air to get the main rotor spinning again. Just that this time the pilot may land slightly harder.
3. If the pilot is too low and applies full collective slightly/too late, it will become a medavac rescue mission for the pilot and passengers.

#### Tail Rotor Loss

1. Start mouthing expletives as you do anything to gain airspeed. High airpseed and/or low collective is the only thing which will prevent the helicopter from spinning out of control. The minimum recommended airspeed is 130km/h, below this and the engine's torque is greater than the drag effect of wind.
2. Airspeed can be gained by pointing the nose to the ground and diving. Just remember to pull up. Advised to gain altitude before this.
3. Find a long and safe place to land. It will be crucial as you are coming in fast.
4. Initiate a slight turn in the direction of the spin of the helicopter. It will help in counter-acting the torque generated by the helicopter's engine.
5. Take a risk and try to land at 40 knots\[80km/h]. And keep decreasing collective, it will reduce the torque generated by the helicopter's engine.

* Another way to land is keep decreasing collective to reduce the spin of the chopper. This gives more stability to the chopper and allows the pilot to set the bird down safely.

Just land and patch up.

Practice on the training server, there is no correct way to do it precisely.

## Advanced Flight Model

A pilot can change to AFM through _Options -> Game_. This flight model requires a HOTAS as keyboard and mouse will not be smooth enough. Most of the physics experienced by helicopters is modelled, but dialed down.

First thing **enable Auto-Trim** and **disable Wind Effects**. Auto-Trim keeps the helicopter in steady flight while increasing or decreasing the collective. It automatically calculates the amount of tail input to be applied allowing the pilot to focus on using the tail rotor only for turning. Wind Effects increases the difficulty of flying the helicopter and can push the helicopter. Unless you want act like a masochist fly with it disabled.

Stress Damage can be either disabled or enabled. Depends upon the pilot. No one will judge you.

Fly with guages on or off, your choice. We have a mod which can add a helmet mounted display\[HMD], so guages may not be required.

Altitude also determines whether a helicopter can fly or not.

### Collective

Here the amount of thrust provided by the main rotor is modelled. So it is quite easy to settle with power if you hover in one place, without changing the thrust provided continously.

Here the pitch of the blades has a more significant presence than in SFM. At certain angles and collective values, the RPM of the motor can decrease, resulting in a loss of thrust. This happens because the pitch kind of becomes parallel to the airflow.

1. If pitch is backwards, decrease collective, it align the pitch of the blades allowing them to bite into the air, generating the thrust required to keep the helicopter flying.
2. If pitch is forwards, increase collective. Same reason as above.

Over torquing the engine also exists. It basically means that you are providing way more power to the helicopter's engine than specified. I have mostly seen it happen when suddenly providing full collective while in a hover or at low speeds.

To maintain a steady flight at a certain altitude, the collective and stick will have to be adjusted continously.

#### Settling with Power or Vortex Ring State

This occurs when there is no fresh air for the main rotor to bite into to provide thrust to keep it flying. It gets straddled in a column of disturbed air with no proper flow of air over the blades.

This is quite common when in a stationary hover. Lower altitudes have a higher chance than higher altitudes as there is very little fresh air flowing over the blades after sometime. A pilot can get trapped in a ring state on final approach too, as you decreasing collective and with a sudden pitch up, the rotor gets enveloped within it's own downwash.

To avoid a ring state, maintain a slight to moderate forward airspeed with a continous change in collective.

### Pitch, Roll and Yaw

Slightly better modelled and with a HOTAS more control over how much the helicopter is rotating on either axis. Lesser chance of the helicopter going into a _salsa dance_.

Weight of the airframe can change how the aircraft behaves to input on any axis. Most mods do not have it, so the helicopter may actually fly like it is in SFM, but with the game engine simulating an AFM environment.

There is no major change if using the joystick in both SFM and AFM. Change comes when migrating from keyboard+mouse to Joystick. Major things happen in the [effect of weight](https://detachment207hawkeye.gitlab.io/docs/afm-and-sfm/##effect-of-weight) section.

### Effect of weight

All if the described effects below are more prominent in light-weight airframes such as the _LittleBirds_. Heavier airframes may experience this if total weight of objects in/attached to the helicopter is more than the standard weight of the helicopter.

#### Collective Effect

AFM takes into account the weight of all objects\[passengers, boxes, missiles, fuel]. Heavier the total weight, greater the initial thrust required to take off from a stationary point.

To counteract the high collective, a rolling takeoff is preferred. A runway or long patch of flat land is required. Though the helicopter will need wheels for this as with skids there is a possibility that the helicopter may flip. Increase the collective enough to get taxiing, and then push the joystick down. Keep increasing the collective to increase airspeed and ease up on the joystick slightly by slightly. Something like a STOL aircraft take-off.

#### Rotation Axes Effect

Distribution of objects in/attached to the helicopter will make it tilt in the direction of the heavier side. The pilot will have to account for that will maintaining a steady flight.

Passengers jumping off the helicopter will make it lurch in the opposite direction of the passenger jumping off. So keep that in mind while doing a hot landing.

### Main Disc Angle

The angle of the main rotor disk controls the direction of the airflow produced by the rotors when in stable condition.

Take the Blackhawk for example. By default it is tilted about 3 degrees forward. So at 0 degrees pitch, the helicopter will still have a slight forward airpseed as the main rotor is pushing the air backwards and downwards. To maintain zero knots, a pilot will have to maintain at least 3 degrees nose up.

### Torque Effect

Here Auto-Trim comes into effect. The moment of inertia is modelled. Without Auto-Trim, a pilot will have to give continous inputs to the pedals to keep the helicopter from spinning around. Manual trim can also be set which provides an offset for the pedals so that the pilot does not have to keep their legs twisted.

Greater the power supplied to the engine, higher the spin rate opposite to the rotation of the main rotor. Lesser the power supplied to the engine, lower the spin rate opposite to the rotation of the main rotor.

Though Auto-Trim is not a life saver, a pilot still needs to provide some input to the pedals, especially on take-off and landing to keep the helicopter in a straight line. Auto-Trim works best when in flight.

### wind Effects

Keep it disabled. If enabled be prepared to provide a ton of inputs to prevent the helicopter deviating from it's flight path. Also land into the wind as the wind will help in slowing down, if landing with the wind, it will be a very fast and hard landing.

### Wheels

A helicopter can taxi at idle to 10% power with the joystick pushed all the way forward. This comes in handy while doing a rolling take-off.

A helicopter can **land at a faster speed** in this flight model. I have personally landed with a tail rotor loss at 60 knots\[120km/h]. You can skid a lot more.

You can even land like a plane on a runway, the only thing is you won't move that far.

**Keep your parking brake on at all times**. Failure to do so will result in the chopper sliding upon touchdown, especially on slopes. A good example was the _Guardian Flight_ crash on Kujari. Parking brake was off and they slid into a house.

If you turn it off for a taxi, you better check twice that you have turned it on. Best way to do it is check the information bar.

### Stress Damage

A very different model from SFM. If you are diving and suddenly pull up while appyling power, your main rotor can shear straight off.

Land too hard\[greater resilience value than SFM] and parts of the chopper will be damaged.

Lesser chance of exploding into pieces, but a greater chance of damaging systems.

If disabled, the game engine simulates a SFM damage model.

Preferred is keep it on, as stuff is definitely different and kind of helps in not exploding too much.

### Guages

In AFM, you get a velocity vector, radar altitude, speed\[km/h], power and vertical velocity indicator, and a compass with wind direction\[imp if wind effects are enabled]

There is a [mod](https://steamcommunity.com/sharedfiles/filedetails/?id=312724602) which can be used both in SFM and AFM. It will replace the vanilla guages and give a better Quality of Life\[QoL] for pilots.

The velocity vector is good for knowing where you are going and can be used as guide for landing at the correct spot.

### Auto-Rotation and Tail Loss

Same aim as in [SFM](https://detachment207hawkeye.gitlab.io/docs/afm-and-sfm/#auto-rotation-and-tail-rotor-loss). Basic aim land to fly another day.

#### Auto-Rotation

Similar to SFM's [auto-rotation](https://detachment207hawkeye.gitlab.io/docs/afm-and-sfm/#auto-rotation).

Decrease collective to 0% and pitch slightly forward. The rate of descent will not be as high as in SFM due to the thrust being produced by the spinning blades.

The helicopter can also move more horizontally, if the correct inputs are provided. Three ways of doing this,

1. Pitch all the way down with zero collective, and at a certain altitude as the pilot sees fit, level off with 40%-50% collective. As soon as the blades slow down, decrease collective and repeat. The kinetic energy produced as a result of diving is translated into forward airpseed for the helicopter while levelling off.
2. Pitch 0-3 degress nose down. Decrease collective to 0%. The direction of the airflow will provide some lift as well as thrust in the forward direction.
3. Combine 1 and 2.
4. One point to note is not get stuck in your **rotor vortex**. The forward airpseed helps in that. Maintain at least _40km/h_ forward airspeed.

There is no constant method, but Point 1 should not be used at low altitudes\[30 MGL/ 100 FGL]. Reason is obvious, you will literally become a kamikaze, and will go on youtube and casting couch.

#### Tail-Rotor Loss

1. Gain airspeed still applies here.
2. The helicopter can be kept more stable using the joystick.
3. Gain altitude, power has to be applied, a necessary evil. Here keeping the helicopter steady using the joystick comes in handy. When the pilot feels that they are high enough, start to decrease power. The decrease in power will reduce the spinning and vomiting. Pitch down and scream.
4. As you gain airspeed the effect of the engine's torque decreases due to good old wind, start to decrease altitude\[not too low such that you are skimming tree tops], find a nice large patch of land and start your approach.
5. You can safely land at 60 knots\[120 km/h], it's enough to keep your helicopter from spinning out of control while on approach and also not too fast such that you explode on contact.
6. Be careful not to get stuck in your own rotor vortex. If you feel you are getting stuck in one, pitch the nose down and push the helicopter into fresh air.
