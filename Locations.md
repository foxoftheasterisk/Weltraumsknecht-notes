(May want to split this page further)

The map, in general, is like a metroidvania: One big map, divided into several themed areas, but you can move between those areas freely.

Comparable to Rogue Legacy (2)'s map, but leaning more into the metroidvania aspects: hidden (and not so hidden) upgrades, regions blocked off until later, rooms that may be a bit of a challenge to navigate, etc.

Compared to a classic metroidvania though, it's more likely we'll have "soft" barriers that you can cheat, since we don't have the option of requiring specific weapons.

I'm currently thinking we'll have three areas, arranged into a rough triangle so there are connections between each pair of areas.
It could be fun to instead have the areas not have a consistent layout, but it's also that much harder to work with. So, stretch goal?

Since I was thinking about a Metroid Fusion kind of aesthetic... maybe we should *not* have pass-through platforms?

I just kind of assumed we should (bc my main inspiration is RL2, which *does* have them) but in addition to giving Metroid Fusion vibes, not having them means simpler controls in a way (don't have to have a drop-through control) and more predictable projectile/enemy behavior

(I *think* Fusion doesn't have any pass-through platforms anyway? Except I think the save room has one, but that hardly counts)
(For that matter, does Castlevania have pass-throughs? I can't remember.)

It does mean we'd likely want larger rooms, to fit the structures needed to allow ascent without pass-throughs.

For secrets/breakable walls: we may not have different categories of weapons we can guarantee (apart from kick and not kick) BUT we can make it so breakable walls only break from (skill) crits.
(This is easier to manage with some weapons than others but that seems fine.)

... Could also just be a certain amount of damage. Or number of hits.

Assuming one boss per area for now. 
More feels more metroidvania actually, but too many bosses has problems, plus it's more to design.

Bosses give heart containers? (May or may not full heal.)
Thinking each boss also gives a movement upgrade (that you need (or "need") to reach the next area)

Altho it's very nice in RL2, I think no boss door heals. Manage your own health. >:)

Actually, if boss heart containers do full heal, that introduces a temptation to *use the boss to heal*.
Not sure if that's a desired result or not.
Having some challenge that full heals at the end seems nice, but I'm not sure it should be bosses.
... actually, *yes*, that *is* good for bosses. you beat the boss, big climax, and now you're fresh for the next area. (Which you're otherwise unprepared for because that's how roguelikes work, ideally.)
Using bosses to heal is possible if you're a badass, but probably not recommended.

Hmm. Other thought—metroidvanias do like to spring Surprise Bosses on you. Should we do that? Or is that too cruel with permadeath in the mix?

And, related but not necessarily the same question—should boss rooms be on the map directly, or a separate plane like in RL2?
I'm thinking directly on the map. But I also want to let players have the chance to turn around and *not* face the boss yet.

Not sure how best to implement that—I'm pretty sure I *don't* want the boss room to be indicated on the map before finding it though.
Maybe just a "lobby" room with a teleporter? Hmmn.
... I kinda want the teleporter to not be available until after you beat the boss, though. Cause otherwise trapping you in a specific area is just not possible.

~~"Heirloom" challenges—i.e. a full heal followed by a challenge—seem appropriate. May or may not give an ability of some sort (or just have weapon/shop at the end, like sword portals?)~~

~~"Fairy chest" challenges for heals? (Probably just one heart heal, but maybe not?)~~
~~They could also just be for rarer weapons or something.~~
~~Crystal hearts—2 heal + piece of heart~~

~~Average one full heart from pieces per area? (May not all be from Fairy chests, rootchoice room also might exist.)~~
~~(This doesn't have to be four pieces.)~~
~~Maybe more, actually, bc i think it should be typical to get one heart before the boss, and we've (not definitively) established there's more area you can get to after the boss (and after other bosses)~~

~~I like that idea, but it's equally viable to have "Fairy chests" give weapon mods. (Or these could both exist.)~~

At this point I'm thinking crystal hearts should have any special challenges or whatever, they're just *hidden*. Same with the weapon mods. They just work like Fusion's tank pickups.

(Which does mean occasionally they aren't even hidden, they're just off in a side room.)

Hmm. If we're aiming for around 4-6 crystal hearts per area... that's about the same as how many weapon mods we want, I think. I kinda like that they end up about the same rarity.

(It might be a little more than that, actually. If there's three areas, and 4 weapons * 5 slots when evolved... it would be 7 per area to fill them all, and that's discounting the possibility of *replacing* weapons.)

~~...It does kinda feel like post boss heals + crystal heart challenges + heirloom challenge heals + random drops is maybe too much healing, especially if we're trying to get 4-6 crystal hearts per location. I mean it all depends on how much damage you'll take, but... when it's all laid out, that sounds generous.~~
~~The first thing to cut would probably be heirloom challenges... That, or cut down the healing from crystal hearts.~~
~~... Or if half the crystal hearts are rootchoice ones that actually damage you. That would probably do it.~~

~~Still not sure what form heirloom challenges should take. Sword portal type enemy rushes? Those should exist, certainly, but not sure they should be the same.~~

Thinking maybe you can spin off spikes, but not terrain? That's kind of a weird thing to justify though
(Because reclaiming "coins" without magnet or double jump)
Or. You actually claim coins by damaging them, and spikes and other damaging hazards count.
Better, you claim coins by damaging them, and therefore can kick off the coins themselves.
(Possibly both.)

But Also there can be a "danger floor" in some area that's a kickable damage field

World generation—I like the idea of it being like RL2, with the medtroidvania-style areas and coming back to earlier areas
(Particularly, I like how that interacts with health levels)
Probably would then lean into the metroidvania, have parts of early areas you can't get to without double jump, long dash, etc (or, like the Study, where you *can* if you do it right, but it's clearly discouraged)

However it would probably be much simpler to do the classic roguelike "floors".

... it could be even more metroidvania if areas don't have a consistent arrangement, so you actually have to explore to find them. But that also is a bit counter to the HP management play, so, I'm not sure there.
... well, is it though? Sure, it can lead you to having to use up some of the earlier area when you might not need it, but that's already going to be a thing. And if you actually maybe *have* to explore the early areas, that means your low-HP exploration isn't going to be *only* to recover health, it also might progress you.

... although it could also mean that runs get easier or harder based on where the areas spawn. Which, that variability is somewhat inevitable, but also keeping it *relatively* consistent is somewhat desirable.

Teleporters for sure, obvs.
- Starting room
- every boss room
- every side quest destination
- possibly others

... Well, I say that, but there are actually some disadvantages to having teleporters. Mainly, it makes it less possible to trap the player in one area.

Now having no consistent layout could make area identities less distinct, but it's probably fine.

Speaking of, yeah, distinct area identities is a major goal here. RL2 does a great job of it and I want to replicate that. (Not with the same areas, of course.)

... It would be cool and enhance the metroidvania feel if we didn't always have the same areas, and/or didn't always take them in the same order. BUT that would also mean we'd have to have multiple areas at the same difficulty level? Which seems difficult while also giving them distinct identities.

Also would be cool to have "complete half this area, then do this other area, then return"... but to do that we'd need—
...I was going to say we'd need mid-area mobility drops, but it could just be, like, some kind of key. Mobility increasers are the *biggest* keys we want to do, but we could just do, like, actual keys, for some things. (Probably not too many though.)

Other, non-mobility keys:
- Impenetrable darkness
- damaging areas (varia suit)
- ... *or* damaging areas like the electric water
- just actual locked doors (boring) (but perfectly serviceable)
- environment destruction (Probably by the other landsknecht!)
- *probably* don't have a countdown-to-destruction bit... but maybe!

the nice thing here is we can potentially have these "keys" be pointed to by NPCs, and thus, objectives!

However must keep in mind that some of these are not "hard" barriers and thus do not guarantee other upgrades... or even themselves, necessarily.
The mobility increases (mostly) also fall into that category. Something that "requires" a wall jump may still sometimes be doable without it, by kicking off enemies or some such.
(Suppose we could remove kick, but kick is *fun.*)
So always make sure there's a way out without needing the upgrade. (Or, a way to *get to* the upgrade, since getting stuck in an area can be kinda fun.)

If there *are* minibosses, putting them with the "keys" makes sense

There's also the concept, if we're leaning in to Fusion, of the stage itself being damaged by events not (directly) caused by you. (SA-X, that guard robot.) That could also be a "key", although I think we'd want to keep it to a relatively small area to prevent search frustration. Or have a map indicator (and something that prompts you to *check* the map), I guess.

Ok so a big aspect of what makes Fusion the way it is, is that you're constantly breaking open walls and finding secret passages *as part of the plot.*
So you don't so much have "Oh, a secret passage, time to get an upgrade!"
Instead it's more like "Hmm, here's yet another secret passage, is this one an upgrade or does it lead to the objective?"
feels much more exploratory in that way
And yeah, I think I like that.

There's also the concept of going through a (small part of) a later area to reach the next area, that could be fun. (Not sure if this involves nerfed versions of the enemies or not—might depend on how *much* later an area it is.)

And then there's the metroidvania standby of doing something that ends up getting you stuck in a new area, until you find another way out / a new upgrade that lets you get back the way you came. We can play with that. (But not *too* much.)

... But in trying to make it metroidvania, make sure not to make it end up too long or frustrating. This is a roguelike with metroidvania theming, not the other way around. And a roguelike needs to be short.

Six areas is probably about the maximum. Especially since we have to develop each of them.
Four might be more achievable.
Actually, probably should aim for just three for now. 

I like the idea of "secret areas" that don't show up on the map. The only issue with that is, we'd need to have a map reveal for it to make sense! (I don't *object* to that, I'm just not sure where it fits in.)

Since this isn't started outright: Rogue Legacy 2 has a concept where the same rooms can spawn in different areas, but with some elements determined by the area. For example some rooms have "round hazards" which are swinging chains in the castle, but growing ice chunks in the cold area. I thought this concept seems useful.

If "danger floors" are a thing (im not sure) then one could be a floor you can kick off, but not walk on.

... I don't know if this kind of hazards should even feature. Maybe we should just keep it simple and stick to enemies.

(Although "floors" you can't walk on, for whatever reason—lava, spikes, whatever—are both a classic trope and a useful tool. So we probably do at least that.)

Areas:
Areas (and the setting generally) lean towards the Metroid side of Metroidvania.
* Zoo: starting area
	* Trap: shackles (temporarily tethers player, can break by dashing; does no damage)
		* Not literal shackles but the forcefield equivalent
	* Some rooms that are like mini habitats of different themes (which could be the other areas?)
	* More horizontally open rooms?
* Maintenance/engineering: more cramped and twisty
	* Bursting pipes—but as trap, wall shooter, or both?
	* ooh, wall shooters that are like, electrical/laser mechanisms
		* why aren't they contained? shhh don't worry about it.  ... maybe because the station is having An Emergency
* Habitat?: more open (esp vertically) and rounded/organic shapes
	* Seems weird for there to be zoo *and* habitat, but
		* Unless *this* habitat is for the aliens that run the place?
* Cold storage?
* Bridge/operational areas?
* The promenade (like ds9)
* Docking bays?
    * not sure if this would be a whole area, maybe a sub-area? Of ops maybe?
* ~~Tower climb — I don't know how to flavor it, but the sun tower is cool and I want to steal its glory~~

