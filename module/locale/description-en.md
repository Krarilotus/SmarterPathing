# Smarter Pathing

**Author**: Monsterfish
**Version**: 1.0.3

Units find their way better. Every part can be switched off in the settings.

## Assassins carry on after a fight

Before, assassins sent somewhere would fight any enemies they ran into on the way and then
just stand there, as if they had forgotten the order. Other soldiers didn't do this.

It happened because assassins may climb walls only while their order is being given. When
the fight was over (or when someone blocked their way), the game worked out the route again
as if they were ordinary soldiers. If the only way there was over a wall, it found none,
and they stopped.

Now assassins remember whether their order let them climb, and they carry on to where you
sent them, over walls if needed. Assassins sent out together with other troops still stay
off the walls, the same as before.

They keep remembering when you save and load the game (this needs the Map Extensions
module, which is switched on along with this one).

## Assassins only climb when it is clearly shorter

Assassins used to climb up and down walls even when walking around would have been just
as quick, and climbing is slow. Now they look for a way on the ground first:

* A short walk (under 30 tiles) is always taken.
* For a longer walk they also look for a way over the walls, and climb only if it is
  clearly shorter: at least 25% shorter than walking.
* If there is no way on the ground at all, they climb, as before.

Both numbers can be changed in the settings.

## Workers on a break don't get stuck

When your people are happy, workers take breaks and walk to a garden, a maypole or another
nice building. The break only ended once they got there. If their way was blocked on the
way (a new building or wall, a gate that closed), they kept trying for ever and never went
back to work.

Now a worker whose way to the break is blocked picks another place to go, or goes back to
work if the break is over.

## Workers stuck on the way to work are replaced

The same thing could happen on a worker's way to work, to the stockpile or to the granary:
the game only checked roughly whether the place could be reached, so a worker could keep
trying a blocked way for ever.

Now a worker who still can't get through after about five seconds of tries leaves, the
way the game already handles workers who can't reach their work, and the building gets a
new worker from the campfire. Anything they were carrying is lost, as in the game.

## Aggressive troops leave quarry stockpiles alone

Troops on aggressive stance used to wander off to attack an enemy's quarry stockpile (the
stone pile next to a quarry). The game already made them ignore the main stockpile, but
it forgot the quarry's. Now they ignore both. You can still order them to attack it.
