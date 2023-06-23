---
permalink: /Changelog.html
title: The Change Log
description: The Opening Credits, and the closing credits, plus the first of two (or is three) end credit scenes
tags: changes,changelog,change-log,page,kerbal,ksp,zer0Kerbal,zedK
---
<!-- 
hdr-changelog.md v1.0.0.0
Drop Tanks III (DTIII)
created: 13 May 2022
updated:
CC BY-ND 4.0 by zer0Kerbal
--># Changelog  
  
| modName    | Drop Tanks III (DTIII)                                            |
| ---------- | ----------------------------------------------------------------- |
| license    | CC-BY-NC-SA-4.0                                                   |
| author     | Enceos and zer0Kerbal                                             |
| forum      | (https://forum.kerbalspaceprogram.com/index.php?/topic/209332-*/) |
| github     | (https://github.com/zer0Kerbal/zer0Kerbal/DropTanksIII)           |
| curseforge | (https://www.curseforge.com/kerbal/ksp-mods/DropTanksIII)         |

## Version 0.9.99.1-prerelease - `<Спасибо evanisrael>` edition

* Released
  * 22 Jun 2023
  * for Kerbal Space Program 1.12.5
  * by [zer0Kerbal](http://github.com/zer0Kerbal)

* 📌 Pinned
  * Dependencies:
    * [Kerbal Hacks Limited(KHL)](https://www.curseforge.com/kerbal/ksp-mods/kerbalhacksltd)
  * search for `dt3` or `dtiii` in editors

### Change Summary 0.9.99.1

* Fixed
  * [BUG] B9PartSwitch throws errors and crashes
  * needed to move the variable cleanup statement into own patch
* Localize
  * ![Russian (Русский)](https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/master/img/RU.png) Russian (Русский)
  * Спасибо [evanisrael](https://github/evanisrael)

### Changes 0.9.99.1

#### Compatibility 0.9.99.1

* [BUG] B9PartSwitch throws errors and crashes
  * needed to move the variable cleanup statement into own patch
* closes #33 - [BUG] B9PartSwitch throws errors and crashes

#### Localization 0.9.99.1

* Add
  * Russian (Русский)
    * [ru.cfg] v1.0.0.0
    * Спасибо [evanisrael](https://github/evanisrael)
  * Translation guides
    * [readme-ru.md] v1.0.1.0
    * [quickstart-ru.md] v1.0.0.0
    * Спасибо [evanisrael](https://github/evanisrael)
* Update
  * [ru.cfg] v1.0.1.0
  * add header, give credit
* closes #10 - Localization - Master
* closes #18 - Russian (Русский) <ru.cfg>

#### Documentation 0.9.99.1

* Update
  * [Attributions.md] v1.0.1.0
  * [Localizations.md] v1.0.1.0
  * [readme.md] v0.9.99.1
  * [ReleaseLayout.md] 0.9.99.1

### Issues 0.9.99.1

* closes #31 - 0.9.99.1 Additional Tasks
* closes #30 - Drop Tanks III (DTIII) 0.9.99.1-prerelease `<Спасибо evanisrael>` edition

---

## Version 0.9.99.0-prerelease - `<Enceos Inspired>` edition

* Released
  * 07 Apr 2023
  * for Kerbal Space Program 1.12.5
  * by [zer0Kerbal](http://github.com/zer0Kerbal)

### Creation by [zer0Kerbal](http://github.com/zer0Kerbal)

* 📌 Pinned
  * Dependencies:
    * [Kerbal Hacks Limited (KHL)](https://www.curseforge.com/kerbal/ksp-mods/kerbalhacksltd)
  * search for `dt3` or `dtiii` in editors

### Change Summary 0.9.99.0

* NEW 3.75m (inner diameter) drop tanks
  * TechRequired = advFuelSystems
* English and Dutch localizations
* Compatibility
  * [B9FuelSwitch.cfg]
  * [InterstellarFuelSwitch.cfg]
  * [TweakScale.cfg]
* Subject to change (K5 need input!!!)
  * mass
  * cost/entryCost
  * capacity
  * Decoupler: explosiveForce (eF)

#### Specifications

| 3.75      | mass (mt) | cost  | LF    | OX    | eF   |
| --------- | --------- | ----- | ----- | ----- | ---- |
| cap       | 0.625     | 10800 | 2673  | 3267  | 1250 |
| bracelet  | 1.25      | 6000  | 5589  | 6831  | 1250 |
| wristband | 2.25      | 35100 | 11178 | 13662 | 1250 |
| wrapper   | 4.5       | 35100 | 22599 | 27621 | 1250 |
| sleeve    | 9.0       | 8100  | 29160 | 35640 | 1250 |

### Changes 0.9.99.0

### Parts

* Create five new parts (scaled)
* DONE:
  * inventory
  * DRAG_CUBES

### Compatibility 0.9.99.0

* Create
  * [InterstellarFuelSwitch.cfg] v1.0.0.0
  * [B9FuelSwitch.cfg] v1.0.0.0

### docs/ 0.9.99.0

* Add
  * [`_config.yml`]
  * [Attribution.md] v1.0.7.1
  * [ManualInstallation.md] v1.1.8.0
  * [404.md] v1.0.3.2
  * [LegalMumboJumbo.md] v1.0.5.1
  * [Localizations.md] v1.1.7.0
  * [Marketing.md] v1.0.1.0
  * [Notices.md] v1.0.1.0
  * [Parts-Catalog.md] v1.1.4.1
  * [Why.md] v1.1.0.0
* closes #5 - Create GitHub Pages

### Hero Logo 0.9.99.0

* Create
* closes #6 - Create HeroLogo.png

### Localization 1.0.99.0

* Add
  * [DropTanksIII.cfg] v1.0.0.0
    * adds localized tags to parts
* Create
  * Localization/
    * <en-us.cfg> v1.0.0.0
    * <nl-nl.cfg> v1.0.0.0 -bedankt! [renejant](https://github.com/renejant)
    * [readme.md] v2.1.2.0
    * [quickstart.md] v1.0.1.1
* closes #7 - Create Localization directory and contents
* closes #9 - Create <DropTanksIII.cfg>
* closes #11 - English <en-us.cfg>
* closes #22 - Dutch (Nederlands) <nl-nl.cfg>
* updates #10 - Localization - Master

### Issues 0.9.99.0

* closes #1 - DropTanksIII (DTIII) 0.9.99.0-prerelease `<Enceos Inspired>` edition
* closes #2 - 1.1.99.0 Create Legal Mumbo Jumbo
* closes #3 - 1.1.99.0 Create Documentation
* closes #4 - 1.1.99.0 Create Social Media Presence
* closes #8 - Part Asset Updates

---
