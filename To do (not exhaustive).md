	• Make a proper CollisionQueue (with priority)
	• PointTowardsMovementBehaviour
		○ Or maybe, TurnWithMovementBehaviour?
	• Make collision transitions able to check colliding object
		○ (How to do this without being kludgy, I'm not sure.)
	• Add continuous versions of ButtonPressed, ButtonReleased for weapon phasing
	• Make enemy invincibility per-projectile
		○ Add phase boolean to preserve hit record in transitions
	• Add PhaseActiveState condition
		○ This also requires new information in the transition function
			§ Although, I think it can acquire it with what it gets?
	• (Fix enemy knockback and physics)
	• (More interesting enemy behavior)
