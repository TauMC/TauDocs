# TauMC Standard #001: TauMC Standards Specification (revision 1)

This standard sets the specification for all following TauMC standards. It currently primarily consists of shared definitions and language conventions that allow us to treat written word more like a programming language (and by extension write our standards in a less ambiguous way).

## Logic Gates

Logic gates (such as **AND**, **OR**, **XOR**) may be used within referencing standards, **bolded** and CAPITALIZED to avoid ambiguity. Read more about logic gates [here](https://en.wikipedia.org/wiki/Logic_gate).

## Braces & Bulleted Lists

Within referencing standards, some parts of sentences may be surrounded by **bolded** braces (`{}`). These braces should be considered to function the same way brackets (`()`) do in mathematics and computer science; interpret logic gates and other contained statements within these first and group them together. Bulleted lists should be implicitly considered to be within braces unless otherwise explicitly stated.

## Concise Minecraft Versions

Every [release version of Minecraft](#release-version) (according to this standard's definition), excluding the prefix (that being "Alpha" or "Beta", if one is present), starts with `1.`. This is something we do not expect to change within the lifetime of Minecraft: Java Edition. As such, referencing standards may leave out the `1.` when referring to a [Minecraft release version](#release-version).

Additionally, Alpha versions (those starting with "Alpha") may be abbreviated further by referencing standards by replacing the "Alpha" with an `a`. The same applies to Beta versions, which should instead be abbreviated with a `b`. For clarity (such as when **{** Alpha **OR** Beta **}** versions are being referred to in the same context), versions with no prefix can be given the prefix `mc` or `r` applied to them. 

Examples:

- `1.20.1` -> **{** `20.1` **OR** `mc20.1` **OR** `r20.1` **}**
- `1.0` -> **{** `0` **OR** `mc0` **OR** `r0` **}**
- `Beta 1.7.3` -> `b7.3`

## Minecraft

TauMC (as of writing) only does work relating to Minecraft: Java Edition. Other editions, such as Minecraft: Bedrock Edition, are out of TauMC's scope. As such, when any referencing standards refer to "Minecraft" without explicitly stating which edition it is referring to, it should be assumed that it is referring to Minecraft: Java Edition.

## Release Version

The versions of Minecraft listed [on this page](https://minecraft.wiki/w/Java_Edition_version_history) under the "Full Release", "Beta", and "Alpha" sections are considered to be "release versions" for referencing standards.

## Non-release Version

The versions of Minecraft listed [on this page](https://minecraft.wiki/w/Java_Edition_version_history/Development_versions) are considered to be "non-release versions" for referencing standards.

## Major/Minor Version

Each [release version](#release-version) has a "major" and a "minor" component. After applying the logic defined in [Concise Minecraft Versions](#concise-minecraft-versions) and stripping the prefix, the first number is the major version. If there is nothing after this number, the minor version for this version is `0`. If there is a `.`, followed by another number, this following number is the minor version.

Examples:

- `20.1` - Major: `20`, Minor: `1`
- `18` - Major: `18`, Minor: `0`
- `16.5` - Major: `16`, Minor: `5`

When referring to the latest major update, this is simply to disregard the minor component. The latest minor update may be the same as the latest major release.

Examples:

- The latest [release version](#release-version) is `20.4`, so the latest major update is `20`, and the latest minor update is `20.4`
- The latest [release version](#release-version) is `21`, so the latest major and minor updates are both `21`