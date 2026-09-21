* Make a proper CollisionQueue (with priority)
    * player bouncing may want to happen immediately, though?
        * actually it seems to be working fine now without immediacy
        * i might want to expand the hurtbox a bit more though actually
        * (RL2's kick is actually pretty huge.)
    - so actually it looks like the Simulation might already have a sort of priority system? and i just need to use it
* PointTowardsMovementBehaviour
	* Or maybe it should be called TurnWithMovementBehaviour?
* Add continuous versions of ButtonPressed, ButtonReleased for weapon phasing
    * (Rather, a ButtonState in the event—with states Up, Down and Blocked)
* Start Phase event for transitions
* Make enemy invincibility per-projectile
	* Add phase boolean to preserve hit record in transitions
	* or just give brief projectile immunity at the start of a phase?
    	* no, that has problems for some weapons
        	* although if it's defined by the phase, maybe...?
* Add PhaseActiveState condition
    * (checks whether a particular other phase is active)
	* This also requires new information in the transition function
		* Although, I think it *can* acquire it with what it gets? (through a chain of references)
    		* ehh, isn't ideal; let's just expand the Event
* Fix enemy knockback and physics (will see how this is after re-adding a moving enemy)
* move Projectile Properties to transition?
    * Pros: less duplicate Phases, possibly easier to get phase event info
    * Cons: less intuitive(?), can't define properties for initial phase
* Hit-cooldown weapons
* second enemy
* let enemy attacks use phases?
    * this is mainly useful for if they have projectiles that make projectiles (on contact, over time, whatever)
- Prevent player-enemy collisions while enemy flinching (turn off layer?)
- proper one-button dash (works even if not holding a movement button)
- make boomerang show crits
    -  Add target finding to HomingBehaviour
- ... maybe we Do want enemy hitboxes to change by curve, might prevent some of the weirdness
    - adds new different weirdness though...
- random next phase
    - not sure if actually desirable, but worth testing at least
- Add & display weapon descriptions