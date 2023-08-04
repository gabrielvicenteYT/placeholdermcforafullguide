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

    Advanced Deep Learning Aim Heuristics - Machine Learning checks, that compare cheater and legit player behavior, to stop any aim assist bypasses (Though this creates a vicious cycle and may falsely flag legit players if not enough data is given; and I'll tell you all about that right now).

It can get bypassed by a Machine Learning aim assist or killaura, that fully copies legit behavior. This would need alot of legit players' data, thus, if someone hacked Lunar Client, and got all the legit aiming behavior it needed, it would work quite well. The 'virus' would need to check if any ghost clients got injected, though, otherwise the results can be possibly not as good as they could've been. Anyway, anti-cheats would catch up and so would the hacked clients.

    Aim Shakiness - Checks for extraordinarily shaky aim. For example, it would flag you if you did 500 360s in a second, since it's not legit at all.

It can get bypassed by making the RandomCenterStrength lower, and turning on the Micronized option + turning up the MicronizedStrength.

    Sensitivity / GCD Flaw exploit - Checks for the aim GCD not matching the GCD for everything else.

It can get bypassed by using a Client that doesn't have the bug, or a Client that has the bug, but has an easy way to patch it (Example: Old b73 builds before cross-version had this issue, though it could be fixed with CzechHek's KillAuraPatch).
