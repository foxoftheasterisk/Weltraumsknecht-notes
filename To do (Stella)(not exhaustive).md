* ~~Make a proper CollisionQueue (with priority)~~
    * ~~player bouncing may want to happen immediately, though?~~
        * ~~actually it seems to be working fine now without immediacy~~
    - ~~so actually it looks like the Simulation might already have a sort of priority system? and i just need to use it~~
    - it seems that as long as the hurtboxes are well defined this isn't needed?
    - also should have event listening!
* PointTowardsMovementBehaviour
	* Or maybe it should be called TurnWithMovementBehaviour?
* Add a ButtonState to WeaponInfo
* Start Phase trigger for transitions
    * (Also not immediately relevant)
* Make enemy invincibility per-projectile
	* Add phase boolean to preserve hit record in transitions
	* or just give brief projectile immunity at the start of a phase?
    	* no, that has problems for some weapons
        	* although if it's defined by the phase, maybe...?
* Add PhaseActiveState condition
    * this will require some additions to AttackEvent
* Hit-cooldown weapons
* finish buzzy
    * sprites remaining: hurt, die
- Prevent player-enemy collisions while enemy flinching (turn off layer?)
    - really player and enemy should never interact, physics-wise (exceptions may apply)
        - but they still need to detect collisions! for contact damage!
        - i would say make enemies triggers, but some weapon projectiles (chiefly axe) need to have real physics interactions with them
        - i guess they could have trigger *and* collider on them... that's awkward though...
- proper one-button dash (works even if not holding a movement button)
- ... maybe we Do want enemy hitboxes to change by curve, might prevent some of the weirdness
    - adds new different weirdness though...
    - Alternatively, don't have the hurtbox change at all? That's also weirdness.
    - Weirdness is probably unavoidable as long as we don't have in-between animation frames.
- fix dash (and move lock) drop
- improve jump feel?
- ground kick
- Enemy detection radius
- bake time into transitions? (Instead of having time range conditions)
    - or in addition, since sometimes we might want to have several phases' times linked together

Desired phase effects: 
- create object (done)
    - parameters for projectile properties. e.g. player position at attack start (instead of at projectile creation), speed from Longbow hold time
- move actor
    - ...I feel like the most flexible way to do this is make the Attacker the child of a created projectile. Is that crazy.
- trigger and/or time animation (trigger done)
    - haven't needed timing so far
- trigger other phases?
    - should be simple to add at this point
    - Or it could be default behavior?
- combinations of these
    - but not all every time
    - and also multiple of the same might be good?