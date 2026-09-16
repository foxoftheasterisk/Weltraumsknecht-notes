* Make a proper CollisionQueue (with priority)
    * player bouncing may want to happen immediately, though?
        * actually it seems to be working fine now without immediacy
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
* Fix enemy knockback and physics
* incorporate enemy attacks into phase system
* move Projectile Properties to transition?
    * Pros: less duplicate Phases, possibly easier to get phase event info
    * Cons: less intuitive(?)
* Hit-cooldown weapons

Enemy overhaul:
- Fix animation facing
- compare attack ranges to corners of player bounding box rather than center
- attack range from source rather than enemy pivot
- ... or instead of all that we could just make the range more tolerant, like 120 degrees or something. that would work just fine.