
## Trinus Specifications
This section will go over the specs that are currently known about the Trinus. 

### Extruder Assembly
The information in this section was completely provided by Roi Igarashi @ Kodama [[Forum Post](http://www.kodamaforums.com/phpBB3/viewtopic.php?f=22&t=1721)]. Right now this is a **work in progress** and will be updated as it gets updated on the forums.

![Extruder Breakdown - Labelled](chapter-09-maintenance/img/extruder-breakdown-roi-kodama.jpg)

This topic has two purposes. 

**(1)** Standardize the names of the extruder assembly parts so that the community can discuss them with minimum confusion

**(2)** Provide a brief explanation on the purpose of the parts so that it becomes more clear what is going wrong in case something does go wrong.

The photo does not show all the parts due to the angle of the lens when the photo was taken. I will mention them briefly, but will most probably post another photo showing those parts.

<div class="verbose-list">
* **(A) Filament Entrance #1 :** This is the filament hole which we can see on top of the extruder assembly when completely covered by the black box. There are two holes into which the filament has to enter when we manually feed the filament. The other hole is not visible if the extruder assembly is covered by the box (more on that later.)
* **(B) Filament Grip Release Lever :** This is what we press when we want the grip on the filament to be released. We press this when we manually feed the filament. What it does is push away the filament pinch bearing to allow the filament to freely move up or down (by our pushing or pulling the filament).
* **(C) Cold Block :** [ "C" jumped down intentionally to make the letter coincide with the name "Cold"] This is the main frame of the extruder. It's purpose in life are two: 
    * **(1)** To hold in place all the parts of the extruder assembly and 
    * **(2)** serve as a heat sink or radiator for any heat that may have creeped up the throat tube (L).
* **(D) Pinch Bearing Set Screw :** This keeps the pinch bearing in place. Do NOT tighten this screw. It has to be loose so that the pinch bearing can turn. If you tighten this screw, the pinch bearing will stop to freely turn making filament feed very heavy and will cause extruder filament feeding to fail. It may also cause the extruder motor to burn due to overload.
* **(E) Extruder Motor Shaft :** This is what turns together with the grip gear (name subject to change...anybody has a good name for this?). This can get hot if the extruder load becomes too heavy as any motor gets hot when it is overloaded. An "always on" fan is pointed here to cool it among others.
* **(F) Pinch Spring :** This is the force which is applied to the pinch bearing. It always wants to cause the pinch bearing (G) to get as close to the grip gear so this is what makes sure the filament will move when the extruder motor turns. This has no adjustments related to it.
* **(G) Filament pinch bearing :** This is what pushes the filament against the grip gear of the extruder. This has no adjustments, BUT if you tighten its set screw (D), this will stop to turn and cause the filament movement to become heavy. Please read about (D) above.
* **(H) Heat Block :** This is where heat is "stored" which will eventually be used to melt the filament that is inside the nozzle (N). It is also where the heater cartridge (M) is attached. Not shown is the thermistor (T) which is the sensor to constantly report the temperature of the heat block to the firmware so that the target temperature can be maintained by turning on and off the heater when necessary.
<br/><br/>
The Nozzle (N) is also screwed into here.
<br/><br/>
As can be seen, the Heat Block's main purpose is to be the heated center for the hotend. So the nozzle (N), heater cartridge (H) and thermistor (T - not shown) all have to be efficiently attached to the Heat Block so that heat can move from the heat cartridge to the nozzle and thermistor efficiently.
<br/><br/>
But the Heat Block's purpose is to also hold on the throat tube (L) which is its only physical attachment to the whole extruder assembly. This physical hold to the throat tube has to be firm, and yet not too firm that heat from the Heat Block can creep up the throat tube (L). That is THE main challenge to the hotend design... hold the elements of the hotend in place and firm relative to the extruder body BUT with minimal thermal connection to the throat tube.
<br/><br/>
Edit: I originally called it Hot Block, but changed it to Heat Block based on input from two experienced 3d printer users who replied that this part should be called "heat block." I will also change references to this part to heat block accordingly.
* **(I) Grip Gear :** This is what actually holds on to the filament and push the filament down when the extruder motor turns. This part should not get hot or it may melt the filament and make the filament too soft to push down into the hotend. An "always-on" fan is pointed to this part to try to keep it cold.
* **(J) Throat tube cold end set screws :** These set screws have two purposes in life 
    * **(1)** to hold firmly the throat tube (L) which in turn holds the whole hotend assembly below where the nozzle (N) is.
    * **(2)** provide a very efficient (?) physical contact to the cold block (C) so that any heat that creeps up the throat tube from the hotend can be sunk into the cold end. If the heat does not sink properly to the cold block, the throat cold end can get too hot and make the filament entering it to become too soft for the extruder grip gear and pinch bearing to push down the soft filament to the hot block/nozzle.
* **(K) Throat Tube Cold End :** [or Filament Entrance #2] This is the "hidden hole" where the filament has to enter when you manually feed the filament. Since it is not usually visible, a curved filament string (they curve because they have been wrapped around a spool) can cause the tip of the filament end to "miss" this hole when you try to push the filament into the hotend manually into this hole. The best way to make manual feeding into this Throat Tube Cold End is to cut the tip of the filament tip with a 45 degree angle so that the filament end is pointed rather than flat; then turn the filament slowly while trying to push the filament into this hidden hole.
<br/><br/>
It is very important to keep the throat Tube Cold End as cold as you can possibly make it. For my Trinus, I put some thermal paste around the hole in the cold end where the tube enters to make an efficient physical thermal contact between the Throat Tube (L & K) and the Cold Block (C) which is suppose to absorb all the heat that creeps up from the heat block (H) to the Throat Tube (L).
* **(L) Throat Tube :** This throat tube as 3 purposes in life:
    * **(1)** Hold firmly the hotend assembly (Heat Block [H], Nozzle [N], Heat Cartridge [M], - not shown [T] Thermistor [heat sensor]) relative to the rest of the extruder assembly.
    * **(2)** Serve as a heat shield between the Heat Block (H) and the Cold Block (C) so that as little heat as possible migrates up to the Cold Block (C).
    * **(3)** A path for the stiff filament to be pushed down into the hotend assembly.
* **(M) Heat Cartridge :** This is the actual part that gets very hot. It has to have a good physical contact to the Heat Block (H) so that it can efficiently heat the Heat Block (H). I would actually recommend applying thermal paste in the hole where this heat cartridge (M) is inserted. This cartridge is held in place by one set screw. That screw must be tight (but not too tight as you can damage both the screw hex hole or the aluminum threaded hole).
* **(N) Nozzle :** It is inside this nozzle where the filament is actually in the melted state, and this is where molten plastic is extruded via the nozzle hole when a STIFF filament is pushed down the Throat Tube (K & L).
<br/><br/>
The Nozzle (N) should be physically in good contact with the Heat Block (H) so that heat can efficient travel to heat the Nozzle (N). You might also consider apply a very small amount of thermal paste on the thread of the nozzle (but away from the edge of the big hole of the nozzle as you will never want thermal paste to enter the nozzle itself.)
* Not Shown in the main picture:
    * **(1)** Thermistor (heat sensor) with 2 white wires, which is held in place by one set screw to a side of the Heat Block (H)
    * **(2)** Set Screw to hold the Heat Cartridge (M) in the heat block. 
    * **(3)** Set Screw to hold the Throat Tube (L) firmly to the Heat Block (H)
    * **(4)** The Throat Tube hot end which has a ptfe tube inside.
    * **(5)** Two Fans<br/>Note: The set screws to hold the heat cartridge and throat tube in the heat block has to be tight enough to hold them and create a good thermal connection with the heat block BUT they should not be too tight since steel screw set screws can get damaged (the hex hole becomes round) or the heat block holes for the set screws can get stripped threads because aluminum is softer than steel.<br/><br/>
    I would recommend applying some thermal paste in the hole where the thermistor (T) is inserted (This photo does not show where it is, but it is the cartridge which has two white wires) . This will improve the thermistor thermal contact with the heat block so the sensor's temperature reading will be more stable and consistent with the actual temperature of the heat block.
</div>

> ##### WARNING {.warning}
> Before you attempt to disassemble the hotend, please be sure to follow the instructions in this [Forum Topic](http://www.kodamaforums.com/phpBB3/viewtopic.php?f=22&t=1579) (or you risk damaging your throat tube permanently.)

**Breakdown: Trinus - Extruder Assembly** <br/>
[https://youtu.be/Fdubyv2CV6o
![Breakdown the entire extruder assembly](chapter-10-trinus-specs/img/extruder-breakdown-video-screenshot.jpg)
](https://youtu.be/Fdubyv2CV6o)
This video will help you break down the entire extruder assembly incase you need to replace / upgrade parts.