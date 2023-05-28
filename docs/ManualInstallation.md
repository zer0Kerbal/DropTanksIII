---
permalink: /ManualInstallation.html
title: Manual Installation
description: the flat-pack Kiea instructions, written in Kerbalese, unusally present
tags: installation,directions,page,kerbal,ksp,zer0Kerbal,zedK
---
<!-- ManualInstallation.md v1.0.0.0
Drop Tanks III (DTIII)
created: 27 May 2023
updated: 

TEMPLATE: ManualInstallation.md v1.1.9.1
created: 01 Feb 2022
updated: 26 Apr 2023

based upon work by Lisias -->

## [Drop Tanks III (DTIII)][mod]

[Home](./index.md)

Stockalike curved wraparound Drop Tanks (conformal) with an integrated decoupler for Kerbal Space Program

## Installation Instructions

### Using CurseForge/OverWolf app or CKAN

You should be all good! (check for latest version on CurseForge)

### If Downloaded from CurseForge/OverWolf manual download

To install, place the `KerbalHacks` folder inside your Kerbal Space Program's GameData folder:

* **REMOVE ANY OLD VERSIONS OF THE PRODUCT BEFORE INSTALLING**
  * Delete `<KSP_ROOT>/GameData/KerbalHacks/DropTanksIII`
* Extract the package's `KerbalHacks` folder into your KSP's GameData folder as follows:
  * `<PACKAGE>/KerbalHacks` --> `<KSP_ROOT>/GameData`
    * Overwrite any preexisting folder/file(s).
  * you should end up with `<KSP_ROOT>/GameData/KerbalHacks/DropTanksIII`

### If Downloaded from SpaceDock / GitHub / other

To install, place the `GameData` folder inside your Kerbal Space Program folder:

* **REMOVE ANY OLD VERSIONS OF THE PRODUCT BEFORE INSTALLING**
  * Delete `<KSP_ROOT>/GameData/KerbalHacks/DropTanksIII`
* Extract the package's `GameData` folder into your KSP's root folder as follows:
  * `<PACKAGE>/GameData` --> `<KSP_ROOT>`
    * Overwrite any preexisting file.
  * you should end up with `<KSP_ROOT>/GameData/KerbalHacks/DropTanksIII`

## The following file layout must be present after installation

```markdown
<KSP_ROOT>
  + [GameData]
    + [KerbalHacks]
      + [KerbalHacksLtd]
        ...
      + [DropTanksIII]
        + [Compatibility]
          ...
        + [Config]
          ...
        + [Contracts]
          ...
        + [Localization]
          ...
        + [Parts]
          ...
          ManualInstallation.htm
        * #.#.#.#.htm
        * Attributions.htm
        * CC-BY-NC-SA-4.0.txt
        * changelog.md
        * DropTanksIII.version
        * readme.htm
        ...
      ...
    ...
    * ModuleManager.ConfigCache
  * KSP.log
  ...
```

### Dependencies

* [Kerbal Hacks Ltd. (KHL)][KHL]

THIS FILE: CC BY-ND 4.0 by [zer0Kerbal](https://github.com/zer0Kerbal)
  used with express permission from zer0Kerbal

[KHL]: https://forum.kerbalspaceprogram.com/index.php?/topic/191424-*/ "Kerbal Hacks Ltd. (KH/L)"
[mod]: https://www.curseforge.com/kerbal/ksp-mods/DropTanksIII "Drop Tanks III (DTIII)"