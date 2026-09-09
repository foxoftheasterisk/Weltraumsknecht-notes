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
* implement enemies with different behaviors

Enemy overhaul:
- Enemy should probably be non-abstract, and have separate MovementAI and Attacks.
- Attacks may be largely reusable with just swapping of projectiles & animations. And range.
- multi-projectile Attacks maybe work like weapon phases? Probably don't need too be as complex though.
- MovementAI is a base class (/interface?) that probably *does* need several stages of abstract classes (GroundMovement to GroundApproaches, etc)