## Explaining LiquidBounce's module values
LiquidBounce is currently the best free hacked client; but it needs to be configured properly.
This tutorial will cover multiple values and will explain modules in depth, and will guide you towards the journey to being a config maker.
## Combat
### KillAura
KillAura is one of the most important modules, if not *the* most important module, unless of course you're the best PvPer.
#### Simulate Cooldown
- Simulates the 1.9+ cooldown, good for when you're on a server that has 1.9+ combat, bad for everything else.

- Recommended value: false
#### MaxCPS
- Defines the maximum CPS you should get.

- Recommended value: 13
#### MinCPS
- Defines the minimum CPS you should get.

- Recommended value: 8
#### ClickOnly
- Makes KillAura only work while you are holding left click.

- Recommended value: false
#### HurtTime 
- Waits for targets to stop turning red (10 = doesn't wait 5 = waits halfway 0 = waits fully).

- Recommended value: 10
#### Range 
- Range in which targets will be attacked.

- Recommended value: 3.0
#### ScanRange
- Range in which targets will be aimed at.

- Recommended value: 3.5
#### ThroughWallsRange 
- Range in which targets through walls will be attacked (0 disables this behaviour).

- Recommended value: 3.0
#### RangeSprintReducement 
- Reduces range by set value while sprinting.

- Recommened value: 0.0
#### Priority
- Sets the KillAura's target priority
##### Priority Modes
- Health: Sort by target's health.
- Distance: Sort by target's distance to you (lowest).
- Direction: Sort by target closest to your Field of View.
- LivingTime: Sort by target's age in that world.
- Armor: Sort by target's armor.
- HurtResistance: Sort by target's with the lowest durability armor (?).
- HurtTime: Sort by target's hurttime.
- HealthAbsorption: Sort by target's health, along with the target's absorption.
- RegenAmplifier: Sort by target's regeneration effect.

- Recommended mode: Health
#### Target
- Sets the target mode, self explanatory really.
##### Target Modes
- Single: Selects one target (by priority), and then locks onto it.
- Switch: Switches to next priority target after hitting the first one.
- Multi: Hits multiple targets at once.

- Recommended mode: Single
#### Limited Multi Targets
- Limits the amount of targets the Multi target mode can hit at the same time (To make it infinite, set the value to 0)

- Recommended value: 0
#### Switch Delay
- Sets the delay from switching to the targets while using the Switch target mode

- Recommended value: 150
#### Swing
- Makes KillAura swing every attempted hit

- Recommended value: true
#### KeepSprint 
- Allows KillAura to sprint every attempted hit

- Recommended value: false
#### AutoBlock
- Makes your sword block every attempted hit in most modes
##### AutoBlock Modes
- Off: Disables AutoBlock
- Packet: What you'd consider the normal AutoBlock mode
- AfterTick: Only blocks after attempting to hit the enemy
- Fake: Fakes you blocking

- Recommended mode: Fake
#### InteractAutoBlock
- Makes the AutoBlock interact with ememies

- Recommended value: unknown
#### Smart AutoBlock
- Makes AutoBlock only work when specific conditions are met
- When to use: If the server you're on has patched NoSlow, this can help you still AutoBlock while not getting slowed down too much.

- Recommended value: false
> SmartAutoBlock-dependent values start
#### Force Block When Still
- Ignores all SmartAutoBlock settings when standing still. Still gets fully affected by BlockRate, though

- Recommended value: false
#### Check Enemy Weapon
- Only blocks when an enemy is either using a sword or an axe.

- Recommended value: false
#### Block Range
- Only blocks when you are in range (depending on the value here). Has a bug that makes it not block further than set attack range.

- Recommended value: 3.2
#### Max Own HurtTime
- Doesn't block when you can't get damaged at all (Same method as HurtTime).
- When to use a high value: If you are in a gamemode that has a low hitdelay, adjust accordingly.

- Recommended value: 2
#### Max Opponent Direction Diff
- Only blocks when the enemy is looking close enough at you.

- Recommended value: 60
#### Max Opponent Swing Progress
- Doesn't block if an enemy is still swinging somewhere else, and therefore cannot attack you.

- Recommended value: 1
> SmartAutoBlock-dependent values end
#### Block Rate 
- The chance (in percentage), that AutoBlock will do its thing.

- Recommended value: 100
#### Max Turn Speed
- The maximum speed (In radians) that KillAura rotates to its target.
- When to use higher value: Whenever possible, as long as the anti-cheat does not detect higher values. If the anti-cheat is sophisticated enough, make sure to keep this value at least 1/4 higher than Min Turn Speed.

- Recommended value: 50
#### Min Turn Speed
- The minimum speed (In radians) that KillAura rotates to its target.
- When to use higher value: Whenever possible, as long as the anti-cheat does not detect higher values. If the anti-cheat is sophisticated enough, make sure to keep this value at least 1/4 lower than Max Turn Speed.

- Recommended value: 35
#### RayCast 
- Hits any entity in the Targets that is between you and your target

- Recommended value: true
#### RayCast Ignored 
- Makes RayCast hit all entities between you and your target, instead of just the ones in Targets.

- Recommended value: true
#### Living RayCast 
- Makes RayCast ignore all non-living entities between you andd your target

- Recommended value: false
AAC: Makes KillAura bypass Advanced AntiCheats by hitting entities which appear inside of your opponent
Predict: predicts where the target is moving and aims ahead of them
PredictSize: how much it will aim forward of the target's movement
Failrate: the % the killaura fails to hit someone
LimitedMultiTargets: Multi-Mode will only be allowed to attack this many targets at once, 0 = infinite
Noinvattack: the killaura will not attack if you have your inventory open
NoinvattackDelay: how long it takes for the killaura to stop attacking when you have your inventory open
MinTurnSpeed: the minimum speed your head rotates
MaxTurnSpeed: the maximum speed your head rotates
FakeSwing: Swings your arm before hitting the target, for bypassing heuristic checks
SilentRotation: your head will only rotate on the server side.
RandomCenter: your aim will jitter slightly to appear more legitimate to anticheats mostly
Outborder: modifies RandomCenter to aim at the borders of the target's hitbox (?)
FOV: Field of view that the aura can hit.
Mark: will show the square to the entity you are attacking - Purely visual.
FakeSharp: shows fake sharpness enchantment particles - Purely visual.
