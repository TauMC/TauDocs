# TauMC Standard #002: Minecraft Version Support Status (revision 1)

This document uses many definitions and language conventions from [the TauMC Standards Specification (revision 1)](001-taumc_standards_specification-rev1.md). It is advised that you read that standard before reading this one.

## Preamble

The purpose of this standard is to provide a reliable process to determine which versions of Minecraft should receive priority for support. Projects following this standard should prioritize supporting [Mainline](#mainline-version) and [LTS](#lts-long-term-support) versions, and should not prioritize supporting [EOL](#eol-end-of-life) versions.

## Established Version Statuses

Each version not listed here should be considered [EOL](#eol-end-of-life) (or [Mainline](#mainline-version) in the case of the latest [minor version](001-taumc_standards_specification-rev1.md#majorminor-version)). Note that [non-release versions](001-taumc_standards_specification-rev1.md#non-release-version) are out of scope.

*TBD: No version's support statuses are currently defined, pending the [first establishing session](#first-establishing-session).*

## Definitions

The following definitions are used within the scope of this standard. They may differ from external sources, including internationally recognized dictionaries. For the purposes of interpreting this document, prefer our definition over external ones.

To be clear: None of the statements in this section of this document should be interpreted as an assertion of universal fact.

Additionally, the definitions in this subsection only apply in the context of a Minecraft version.

### Active Version

A Minecraft version is considered "active" if it currently has an active user-base of both players and developers. For example, as of early 2024, Minecraft 20.1 was considered active.

### LTS (**L**ong-**t**erm **S**upport)

A Minecraft version is considered LTS if it satisfies the following conditions:

- It is a [release version](001-taumc_standards_specification-rev1.md#release-version) **AND**
- It was released prior to the latest two [major releases](001-taumc_standards_specification-rev1.md#majorminor-version) **AND**
- It is [active](#active-version) **AND**
- It is likely to remain [active](#active-version)

### Mainline Version

A Minecraft version is considered mainline if it is the latest [minor update](001-taumc_standards_specification-rev1.md#majorminor-version) **OR** if it satisfies the following conditions:

- It is a [release version](001-taumc_standards_specification-rev1.md#release-version) **AND**
- It is [active](#active-version) **AND**
- It is not greater than three [major releases](001-taumc_standards_specification-rev1.md#majorminor-version) old
  - Example: Latest is `21`. `20`, `19`, and `18` (and their [minor versions](001-taumc_standards_specification-rev1.md#majorminor-version)) each fulfill this requirement, but `17` (and its [minor versions](001-taumc_standards_specification-rev1.md#majorminor-version)) and all older versions do not.

### EOL (**E**nd-**o**f-**l**ife)

A Minecraft version is considered EOL if it satisfies the following conditions:

- It is a [release version](001-taumc_standards_specification-rev1.md#release-version) **AND**
- It was released prior to the latest [minor update](001-taumc_standards_specification-rev1.md#majorminor-version) **AND**
- It is not [active](#active-version)

### Support Status

Every [release version](001-taumc_standards_specification-rev1.md#release-version) will have one and only one assigned support status. This status is one of the following:

- [Mainline](#mainline-version) **XOR**
- [LTS](#lts-long-term-support) **XOR**
- [EOL](#eol-end-of-life)

## Addressing Subjectivity

The purpose of this standard is to bring unity, not further division. As such, due to the subjectivity of these definitions, we will also define an [Establishing Process](#establishing-process).

## Establishing Process

Following every release of a new Minecraft [release version](001-taumc_standards_specification-rev1.md#release-version), the members of TauMC (herein referred to as "the council" for the context of an [Establishing Session](#establishing-session)) will review unresolved versions ("unresolved" here meaning versions which are deemed by the council to no longer satisfy the requirements for their currently assigned [support status](#support-status)) and assign each a new support status. Any [release version](001-taumc_standards_specification-rev1.md#release-version) may be considered "unresolved" regardless of its current [status](#support-status) if any council member believes its [status](#support-status) should change. [Non-release versions](001-taumc_standards_specification-rev1.md#non-release-version) are not part of this process, and no [non-release version](001-taumc_standards_specification-rev1.md#non-release-version) will be assigned a [support status](#support-status) under the current definition of this standard.

The council may also decide to hold an ad-hoc [Establishing Session](#establishing-session) at any time if deemed necessary and productive.

The steps listed in [Establishing Session](#establishing-session) will be followed in order. If the council decides to revisit a step that was already completed, then they should also re-visit all steps following that previously completed step, as each step depends on the previous one. At the moment, the way the council "decides" something is currently undefined. We hope to never have to explicitly define this, but will update this document to add a definition if necessary. At the end of this process, there should be no unresolved versions remaining.

### Establishing Session

1. The council will add or remove [PCMs](#prominent-community-members).
2. The council will review this document and make changes as needed - this would be necessary in scenarios where definitions need to be updated due to changes in the game.
3. The council will decide which versions are unresolved.
   - The second to latest [minor version](001-taumc_standards_specification-rev1.md#majorminor-version) (which was previously [mainline](#mainline-version)) is always unresolved during this step.
   - The council will ensure to verify the status of each version currently considered [mainline](#mainline-version) still meets the age requirements of a [mainline version](#mainline-version).
4. For each unresolved version, in ascending order of release date:
   1. The council will decide whether this version is an [active version](#active-version).
   2. Each council member will present their opinion as to what they think the new [support status](#support-status) of this version should be, along with their supporting argument and evidence for this opinion, adhering to the decisions of the council in the previous step.
   3. The council will decide based on previously presented arguments and evidence what the new [support status](#support-status) of this version is.
5. Once all unresolved versions are assigned a new [support status](#support-status), the results of this process will be recorded in this document.

### First Establishing Session

There are many [release versions](001-taumc_standards_specification-rev1.md#release-version) which pre-date this standard. Going through an entire [Establishing Session](#establishing-session) for all of these would take far too long. As such, TauMC will convene the first [Establishing Session](#establishing-session) with the following modifications:

- During step 3, the council will decide on a subset of all versions to assign a [support status](#support-status) to, all of which will be considered unresolved. All versions not considered unresolved during this step will be considered [EOL](#eol-end-of-life) once this session concludes.

### Prominent Community Members

In order to make the outcome of [Establishing Sessions](#establishing-session) as representative as possible of the true status of each version (according to the definitions in this standard), [Prominent Community Members (or VIPs)](#prominent-community-members) will be selected by the members of TauMC to provide input during [Establishing Sessions](#establishing-session). The role of these [PCMs](#prominent-community-members) in this process is exclusively to provide input to inform our decisions. They are not considered part of the "council" as referred to in this document, and do not hold voting powers. This power remains only with the members of TauMC.