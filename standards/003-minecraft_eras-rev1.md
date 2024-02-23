# TauMC Standard #003: The Eras of Minecraft (revision 1)

This document uses many definitions and language conventions from [the TauMC Standards Specification (revision 1)](001-taumc_standards_specification-rev1.md). It is advised that you read that standard before reading this one.

Minecraft has had many large internal changes over the years. This standard groups similar versions in to named "Eras". The eras are as follows:

## The Classic Era

This era began with the very first release of Minecraft, back in 2009. It ended with the last release of "Infdev".

The very few mods that existed during this era were limited to direct modifications to the game client.

## The Primitive Era

This era began with `a0` (the first Alpha release of Minecraft), and ended with `b7.3`.

The first proper modding frameworks started in this era, but they were still very limited, and were still limited to JAR mods (if you don't know what a JAR mod is, thank the devs of your favourite mod loader).

## The Esoteric Era

This era began with `b8`, and ended with `r2.5`.

It was during this era that modding started to gain traction. JAR mods and Risugami's Mod Loader (commonly referred to as simply "Mod Loader") were the primary tools for modding the game during this era.

## The Archaic Era

This era began with `r3`, and ended with `r7.10`.

It introduced the internal server to singleplayer, which broke basically every mod in existence, but also made content mods that were only compatible with singleplayer way less common. The rise of Forge also brought an end to Risugami's Mod Loader and JAR mods (for the most part) during this era.

## The Vintage Era

This era began with `r8`, and ended with `r12.2`.

This era brought some of the most controversial 1st-party changes in Minecraft history. Microsoft acquired Mojang, PVP was revamped, the EULA changed monetization forever, and block states forever changed the way the game worked internally. The block state changes specifically created a large hurdle to mods attempting to port from `r7.10`, which resulted in many mods never making it in to the Vintage era. This took long enough that mods didn't really settle on another primary version until `r12.2`. It's a good thing that they did though, because block states were _nothing_ compared to what came next.

## The Cold Era

This era began with `r13`, and ended with `r16.5`.

This era brought a shift toward data-driven content (via datapacks), and the flattening, which forever changed modding. Forge's (understandable) delays updating for `r13` created a void which was (briefly) filled by the now defunct (yes, defunct; it took me 2 hours to get it to launch) Rift Loader, which was shortly followed by Fabric, and finally a brand-new, revamped Forge. Overall, this was not a great era for modding, but it set the stage for probably the most chaotic era in modding to date:

## The Modern Era

This is the latest era of Minecraft. It started with `r17`, and we don't yet know which version will end it. When this era ends, the following era will take the title of "The Modern Era", and this era will be renamed with the full, concluded era to reflect on to ensure a fitting name (current candidate: "The Proliferation Era").

This is the era in which TauMC was founded. So far, this era has introduced the capability for even more data-driven content, including dynamic world sizes and Y levels below 0. It also brought some more controversial changes such as chat reporting, and the Microsoft account migration. The flattening was also finally wrapped with potion/status effects getting flattened in `r20.2`.

OptiFine, and Bukkit derivatives are still around for some reason. This era has started to really show their age though.

However, the most common theme of this era has by far been proliferation. Quilt and NeoForge were both founded during this era, as was Modrinth, and more proliferation is sure to follow before this era is concluded.