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

Enemy overhaul:
- Dying
- there *could* be a concept of same attacks having multiple ranges with different priorities but until it's needed im not making it. I think there's a reasonable chance we can make the whole game without that.
- awkwardly i feel like angle tolerances need to be higher when the player is closer... that or we look at the whole player bounding box (or well each corner) instead of just the origin?? that seems better, but still awkward. (like what if it stops being a box)