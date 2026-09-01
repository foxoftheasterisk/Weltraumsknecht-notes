* Make a proper CollisionQueue (with priority)
* PointTowardsMovementBehaviour
	* Or maybe it should be called TurnWithMovementBehaviour?.
* Add continuous versions of ButtonPressed, ButtonReleased for weapon phasing
* Make enemy invincibility per-projectile
	* Add phase boolean to preserve hit record in transitions
	* or just give brief projectile immunity at the start of a phase?
    	* no, that has problems for some weapons
        	* although if it's defined by the phase, maybe...?
* Add PhaseActiveState condition
    * (checks whether a particular other phase is active)
	* This also requires new information in the transition function
		* Although, I think it can acquire it with what it gets?
    		* ehh, isn't ideal; let's just expand the Event
* (Fix enemy knockback and physics)
* (More interesting enemy behavior)
