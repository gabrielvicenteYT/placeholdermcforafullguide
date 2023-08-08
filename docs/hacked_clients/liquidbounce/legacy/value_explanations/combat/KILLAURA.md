## KillAura
KillAura is arguably one of the most important modules, if not *the* most important module. This tells you about what each value does, to make you bypass most anti-cheats. Have fun, and don't forget- stay safe!

### Simulate Cooldown
- Simulates the 1.9+ cooldown, good for when you're on a server that has 1.9+ combat, bad for everything else.

- Recommended value: false

### MaxCPS
- Defines the maximum CPS you should get.

- Recommended value: 13

### MinCPS
- Defines the minimum CPS you should get.

- Recommended value: 8

### ClickOnly
- Makes KillAura only work while you are holding left click.

- Recommended value: false

### HurtTime 
- Waits for targets to stop turning red (10 = doesn't wait 5 = waits halfway 0 = waits fully).

- Recommended value: 10

### Range 
- Range in which targets will be attacked.

- Recommended value: 3.0

### ScanRange
- Range in which targets will be aimed at.

- Recommended value: 3.5

### ThroughWallsRange 
- Range in which targets through walls will be attacked (0 disables this behaviour).

- Recommended value: 3.0

### RangeSprintReducement 
- Reduces range by set value while sprinting.

- Recommened value: 0.0

### Priority
- Sets the KillAura's target priority

#### Priority Modes
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

### Target
- Sets the target mode, self explanatory really.

#### Target Modes
- Single: Selects one target (by priority), and then locks onto it.
- Switch: Switches to next priority target after hitting the first one.
- Multi: Hits multiple targets at once.

- Recommended mode: Single

### Limited Multi Targets
- Limits the amount of targets the Multi target mode can hit at the same time (To make it infinite, set the value to 0)

- Recommended value: 0

### Switch Delay
- Sets the delay from switching to the targets while using the Switch target mode

- Recommended value: 150

### Swing
- Makes KillAura swing every attempted hit

- Recommended value: true

### KeepSprint 
- Allows KillAura to sprint every attempted hit

- Recommended value: false

### AutoBlock
- Makes your sword block every attempted hit in most modes

#### AutoBlock Modes
- Off: Disables AutoBlock
- Packet: What you'd consider the normal AutoBlock mode
- AfterTick: Only blocks after attempting to hit the enemy
- Fake: Fakes you blocking

- Recommended mode: Fake

### InteractAutoBlock
- Makes the AutoBlock interact with ememies

- Recommended value: true

### Smart AutoBlock
- Makes AutoBlock only work when specific conditions are met
- When to use: If the server you're on has patched NoSlow, this can help you still AutoBlock while not getting slowed down too much.

- Recommended value: false

> SmartAutoBlock-dependent values start

### Force Block When Still
- Ignores all SmartAutoBlock settings when standing still. Still gets fully affected by BlockRate, though

- Recommended value: false

### Check Enemy Weapon
- Only blocks when an enemy is either using a sword or an axe.

- Recommended value: false

### Block Range
- Only blocks when you are in range (depending on the value here). Has a bug that makes it not block further than set attack range.

- Recommended value: 3.2

### Max Own HurtTime
- Doesn't block when you can't get damaged at all (Same method as HurtTime).
- When to use a high value: If you are in a gamemode that has a low hitdelay, adjust accordingly.

- Recommended value: 2

### Max Opponent Direction Diff
- Only blocks when the enemy is looking close enough at you.

- Recommended value: 60

### Max Opponent Swing Progress
- Doesn't block if an enemy is still swinging somewhere else, and therefore cannot attack you.

- Recommended value: 1
> Smart AutoBlock-dependent values end

### Block Rate 
- The chance (in percentage), that AutoBlock will do its thing.

- Recommended value: 100

### Max Turn Speed
- The maximum speed (In radians) that KillAura rotates to its target.
- When to use higher value: Whenever possible, as long as the anti-cheat does not detect higher values. If the anti-cheat is sophisticated enough, make sure to keep this value at least 1/4 higher than Min Turn Speed.

- Recommended value: 50

### Min Turn Speed
- The minimum speed (In radians) that KillAura rotates to its target.
- When to use higher value: Whenever possible, as long as the anti-cheat does not detect higher values. If the anti-cheat is sophisticated enough, make sure to keep this value at least 1/4 lower than Max Turn Speed.

- Recommended value: 35

### RayCast
- Hits any entity in the Targets that is between you and your target.

- Recommended value: true

### RayCast Ignored
- Makes RayCast hit all entities between you and your target, instead of just the ones in Targets.

- Recommended value: true

### Living RayCast
- Makes RayCast ignore all non-living entities between you and your target.

- Recommended value: false

### AAC 
- Makes KillAura bypass Advanced AntiCheats by hitting entities which appear inside of your opponent.

- Recommended value: false

### KeepRotation Ticks

### Angle Treshold Until Reset

### Micronized
- Makes the KillAura rotations weaker.

- Recommended value: true

### Micronized Strength
- The strength of the Micronized option.

- Recommended value: 1.4 (?)

### Silent Rotation
- Makes the KillAura have silent rotations; if you don't want to flag with it on, use Strict strafe

- Recommended value: true

### Strafe
- Makes the player move accordingly to KillAura's rotations.

#### Strafe Modes
- Off: Does nothing, moves accordingly to the client-side rotations.
- Silent: Moves 99% accordingly to KillAura's rotations, but seems to flag on anti-cheats like Grim.
- Strict: Moves 100% legit.

- Recommended value: Strict

### Random Center
- Makes the KillAura shake a ton, not recommended since anti-cheats seem to detect it.

- Recommended value: false

### Outborder
- Makes the KillAura shake a ton, and make it go to the borders of the hitbox, also not recommended.

- Recommended value: false

### FOV
- Makes the KillAura only hit when it's in a lower distance (field of view-wise, client-sidedly) than the specified value.

- Recommended value: 180

### Predict 
- Predicts where the target is moving and aims ahead of them.

- Recommended value: false

### Max Predict Size
- The maximum (in float) that KillAura aims ahead of the target's movement.

- Recommended value: 1.0

### Min Predict Size
- The minimum (in float) that KillAura aims ahead of the target's movement.

- Recommended value: 0.5

### Fail Rate 
- The percentage of hits that will fail.

- Recommended value: 0

- Q: Why?
- A: The FailRate even fails hits that would suceed if you would hit the enemy by yourself, in the exact same location. This can actually make anti-cheats detect you even further, so yeah.

### Fake Swing 
- Swings your arm before hitting the target, for bypassing heuristic checks.

- Recommended value: true

### No Inv Attack 
- Makes the KillAura not attack whilst you have your inventory open.

- Recommended value: true

### No Inv Attack Delay 
- How long it takes for the KillAura to stop / start attacking after you open / close the inventory

- Recommended value: 10

### Mark
- Will show a square on top of the target you are attacking.

- Recommended value: purely visual, choose it yourself

### FakeSharp
- Shows fake sharpness enchantment particles.

- Recommended value: purely visual, choose it yourself
