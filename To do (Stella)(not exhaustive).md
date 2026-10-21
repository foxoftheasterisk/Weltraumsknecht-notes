* ~~Make a proper CollisionQueue (with priority)~~
    - ~~so actually it looks like the Simulation might already have a sort of priority system? and i just need to use it~~
    - it seems that as long as the hurtboxes are well defined this isn't needed?
        - ~~We're getting null pointers due to wrong order of handling. It's not causing any major problems (yet) but should still be fixed.~~
            - ~~At least I think that's why...~~
            - ~~actually this might have been from use of BreakOnContactBehavior. Should text if it's still present~~.
- add event listening to Simulation
* PointTowardsMovementBehaviour
	* Or maybe it should be called TurnWithMovementBehaviour?
* Add a ButtonState to WeaponInfo
* Start Phase trigger for transitions
* Make enemy invincibility per-projectile
	* Add phase boolean to preserve hit record in transitions
	* or just give brief projectile immunity at the start of a phase?
    	* no, that has problems for some weapons
        	* although if it's defined by the phase, maybe...?
* Add PhaseActiveState condition
    * this will require some additions to AttackEvent
* Hit-cooldown weapons
* finish buzzy
    * sprites remaining: hurt. I guess this is acceptable.
- Prevent player-enemy collisions while enemy flinching (turn off layer?)
    - really player and enemy should never interact, physics-wise (exceptions may apply)
        - but they still need to detect collisions! for contact damage!
        - i would say make enemies triggers, but some weapon projectiles (chiefly axe) need to have real physics interactions with them
        - i guess they could have trigger *and* collider on them... that's awkward though...
        - or. We can make the *player* be a trigger. Possibly we still need a collider for the environment but it's much easier and more practical to double up on the player than *every enemy.*
- proper one-button dash (works even if not holding a movement button)
- fix dash (and move lock) drop
- improve jump feel?
- ground kick
- Enemy detection radius
- bake time into transitions? (Instead of having time range conditions)
    - or in addition, since sometimes we might want to have several phases' times linked together
    - This can be just the minimum time, max time is much rarer
- Since trigger consumption is now an option, end last phase shouldn't do it by default.

Big project:
- **Rooms!**
