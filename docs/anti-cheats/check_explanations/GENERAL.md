## Explaining Anti-Cheat checks
Since the very first anti-cheats, a lot has changed; they're not that easy to bypass anymore… Or are they…
This tutorial will cover multiple checks and will explain them in depth, and will guide you towards the journey to being a config maker.

### Combat

#### Aim Checks

##### Rotation Consistency 
- Description: Checks for unnaturally consistent aim.

- How to bypass it: Use legit-ish (60 min - 100 max, for example) Rotation Speed values.

##### Rotation Speed 
- Description: Checks for rotations too fast to be legit.

- How to bypass it: Reduce rotation speed, to about 30 - 60.

##### Rotation Accuracy 
- Description: Checks for rotation accuracy, aka Aim Accuracy that is either too good or too bad to be legit.

- How to bypass it: Use RandomCenter and other methods such as using Predict (In LiquidBounce) at -0.5 min 0.5 max.

But in a nutshell, those other methods fully simulate a player's aiming behavior, and are 100x better than RandomCenter, though you have to possibly spend years to make those methods work.

##### Aim Shakiness 
- Description: Checks for overly shaky aim.

- How to bypass it: Make sure that your RandomCenter / whatever is called on your hacked client is not too high.

##### Sensitivity / GCD Flaw exploit 
- Description: Checks for the aim GCD not matching the detected sensitivity for everything else.

- How to bypass it: Use a hacked client that has patched / fixed the bug.

