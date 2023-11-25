## Explaining ChestStealer Checks
ChestStealer checks are extremely useful in SkyWars, in order to detect most blatant cheaters. However, I am not here to tell you how to patch bypasses, I'm telling you how to bypass those checks.

#### Pick Consistency 
- Description: Checks for too consistent or too inconsistent delay between taking items.

- How to bypass it: Use legit-ish (60 - 80ms, for example) pick delay values.

#### Pick Speed 
- Description: Checks for taking items too quickly.

- How to bypass it: Increase the pick delay, to about 250 - 325ms, or 10 - 15 ticks.

#### Advanced Pick Check
- Description: Checks if the delay is consistent enough and oblivious to the time that it takes to move the mouse to different parts of the chest.

- How to bypass it: Make the ChestStealer calculate the time it would take for a legit player to move the mouse there.

#### Pick Accuracy 
- Description: Checks for too high item stealing accuracy.

- Types:
- Short Term (very rare, no anti-cheat that I know has it)
- Medium Term (also very rare, on Polar)
- Long Term (currently only Polar and maybe other private anti-cheats have it, patches pretty much every client)

- How to bypass it: Make ChestStealer fail clicks sometimes.

#### Pick Items
- Description: Checks which items were stolen, because legit players usually only take the basics.

- How to bypass it: Make the ChestStealer only steal the basics.
