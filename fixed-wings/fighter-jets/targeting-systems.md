---
description: >-
  Explaining the various targeting systems which exist with the fixed wing jets
  flown by Hawkeye
---

# Targeting Systems

## Laser Designation

![Figure 1 : Bomb Drop Position](../../.gitbook/assets/107410\_20220531080232\_1.png)

A solid white cross with a dot in the centre represents where the bomb/missile will hit the ground. It's marked in the image with a red circle. This is the munitions cross

The big cross with the broken line box is the camera targeting reticule. A few cameras will not have a cross, but only the box.



A similar cross but with broken lines represents a laser. If using Laser guided munitions, line up the plane on a straight path to the laser location, and when both the laser cross and the munitions cross appear in the targeting reticule, drop the bomb. An offset of 5-10 degrees from the target location is acceptable. Anything more and well good luck explaining a bomb crater to 1-1 HQ.

If the plane is self-lasing, it is advised to keep the camera on the target for as long as possible. Depending upon which side the camera is located, take a shallow turn in the opposite direction for about 5 seconds and then a shallow orbit to the camera's side.\
If the target is being designated by anyone else, drop the bomb and then bug out.

For the best hits, drop the bomb when the munitions cross has crossed the laser cross but within the camera targeting reticule cross. This will make the bomb land almost perpendicular to the ground on the target, minimising collateral damage.

#### LG Missiles

LG Mavericks just need a laser, point the aircraft in the general direction of the laser, keep spamming _<mark style="color:orange;">R</mark>_ until you get a lock. If the lock does not appear, then the laser designated target is out of detection cone of the Mavericks. Change the approach angle.&#x20;

## I-TGT System

The I-TGT system is used for GPS guidance of bombs onto their target. A player can either select the a point on the map or enter 8/10 digit coordinates to the I-TGT system. The I-TGT system does not accept 6 digit coordinates.

To obtain 8/10 digit coordinates, either use Map Tools or Vector 21 with MicroDAGR.

The point where the camera is looking at can also be used to designate via the _<mark style="color:yellow;">POI</mark>_ bezel key. <mark style="color:red;">**NOT TO BE USED UNLESS YOU KNOW WHAT YOU ARE DOING**</mark>.

For a bomb to lock onto a target, the target information has to be sent to the pylon first. If the bomb is dropped without any GPS input, it will default to either unguided or laser if it can be laser guided.

To change the target information on a pylon, the current targeting information will have to be cleared from the pylon, then the new targeting information can be inputted to the pylon.

Multiple targets can be selected and sent to different pylons. Multiple targets cannot be sent to the same pylon.

### Steps

{% embed url="https://youtu.be/_cGHZNwLjME" %}
_**Video 1 : Showcasing I-TGT system**_
{% endembed %}

The below steps correspond to the video above.

1. Using scroll wheel open I-TGT system. It will appear in the bottom-right corner.
2. Either choose a point via the map. _<mark style="color:yellow;">DGN</mark>_ bezel key has to be pressed. OR Enter the grid coordinates in a box in the bottom left corner after pressing the _<mark style="color:yellow;">GRID</mark>_ bezel key.
3. Click on the _<mark style="color:blue;">LIST</mark>_ bezel key to obtain a list of pylons with GPS guided munitions and target locations.
4. Select a pylon and a target location.
5. Click on the _<mark style="color:yellow;">SEL</mark>_ bezel key to send the targeting information to the selected pylon. Multiple pylons can have the same targeting location, but preferred to do that one by one.
6. A confirmation message will appear when the target is locked to the pylon. Example, \
   SYSTEM : TARGET LOCKED - PYLON : 3/TGT : TGT\_0_\__Orion
7. Make sure CTAB is set to zoom level 4/8. Anything higher or lower will result in the bomb missing the target completely. And make sure that the plane is within a 10-20 degree arc of the target, otherwise the bomb will not be able to correct itself enough.
8. Before dropping the bomb, make sure it set to use GPS and not unguided/laser. This can be confirmed by observing the ammunition state. Refer Figure 2. The ammunition state should be a broken white line with an arrow halfway through. \
   A solid white line represents laser/unguided.
   1. If the pilot is dropping the bomb, on the HUD the bomb state will change from _<mark style="color:green;">DIRECT</mark>_ to _<mark style="color:green;">I-TGT</mark>_ mode.
9. When the target just crosses the inner green circle, drop the bomb. It will guide itself to the target on it's own.

![Figure 2 : GPS Guidance activated on bomb](../../.gitbook/assets/GPS\_Guided\_Ammo.png)

