# Insurgency: Sandstorm — Local Play Mutator Cheat Sheet

## How to Use (Local Play)

1. Go to **Local Play > Random Map > Security/Insurgents** and load any map.
2. Open console with **`** (backtick key).
3. Enter your command using the syntax below.
4. Mutators stay active even when you load a different map afterward, as long as you keep using `Travel` (not `open`).
5. To switch maps while keeping mutators: open the **Admin Menu** (bind it under Settings > Binds > User Interface/Hud > Toggle Admin Menu) > Levels > select map.

### Command Syntax

```
Travel <Map>?Scenario=<ScenarioName>?Mutators=Mutator1,Mutator2,Mutator3
```

- Use `Travel`, not `open` — `open` will reset/override your mutator list.
- Add `?Lighting=Night` or `?Lighting=Day` to control time of day.
- Add mutators from any of the lists below, comma-separated.

### Default / Example Command

Ministry, Checkpoint Security, Day, with your locked-in defaults + Vampirism:

```
Travel Ministry?Scenario=Scenario_Ministry_Checkpoint_Security?Lighting=Day?Mutators=10E,FB8,Diff10,200S,FFOn,VOn,Vampirism,ImprovedAI,Reloads,Bolts,Quickdraw,HitIndicator,JumpShoot,DeathCam,WeaponAnimFix
```

---

## Increasing Local Bot Counts (Config File)

Path: `[User]\AppData\Local\Insurgency\Saved\Config\WindowsClient\Game.ini`

```ini
[/script/insurgency.inscoopmode]
bBots=True
FriendlyBotQuota=8
SoloEnemies=30
MinimumEnemies=15
MaximumEnemies=30
MaxPlayersToScaleEnemyCount=8
```

---

## Map & Scenario Reference

Format: `Scenario_<Map>_<Mode>`. Not every map has every mode — pick from the list under each map.

### Bab
- Checkpoint_Insurgents / Checkpoint_Security
- Domination
- Firefight_East
- Outpost
- Push_Insurgents / Push_Security
- Ambush
- Survival
- Defusal

### Crossing (Canyon)
- Ambush
- Checkpoint_Insurgents / Checkpoint_Security
- Domination
- Firefight_West
- Frontline
- Outpost
- Push_Insurgents / Push_Security
- Skirmish
- Team_Deathmatch
- Defusal
- FFA

### Farmhouse
- Ambush
- Checkpoint_Insurgents / Checkpoint_Security
- Domination
- Firefight_East / Firefight_West
- Frontline
- Push_Insurgents / Push_Security
- Skirmish
- Survival
- Team_Deathmatch
- Range
- Outpost
- Defusal

### Hideout (Town)
- Ambush / Ambush_East
- Checkpoint_Insurgents / Checkpoint_Security
- Domination
- Firefight_East / Firefight_West
- Frontline
- Push_Insurgents / Push_Security
- Skirmish
- Survival
- Team_Deathmatch
- Outpost
- Defusal

### Hillside (Sinjar)
- Ambush
- Checkpoint_Insurgents / Checkpoint_Security
- Domination
- Firefight_East / Firefight_West
- Frontline
- Outpost
- Push_Insurgents / Push_Security (INS2014 layout)
- Skirmish
- Survival
- Defusal

### Ministry
- Ambush
- Checkpoint_Insurgents / **Checkpoint_Security** ← *(default)*
- Domination
- Firefight_A
- Skirmish
- Team_Deathmatch
- Outpost
- Survival
- Defusal

### Outskirts (Compound)
- Checkpoint_Insurgents / Checkpoint_Security
- Firefight_East / Firefight_West
- Frontline
- Push_Insurgents / Push_Security
- Team_Deathmatch
- Survival
- Defusal
- Domination
- Outpost
- Ambush / Ambush_East

### Precinct
- Ambush / Ambush_East
- Checkpoint_Insurgents / Checkpoint_Security
- Firefight_East / Firefight_West
- Frontline
- Push_Insurgents / Push_Security
- Skirmish
- Team_Deathmatch
- Survival
- Defusal
- Domination_West / Domination_East
- Outpost
- FFA

### Refinery (Oilfield)
- Ambush
- Checkpoint_Insurgents / Checkpoint_Security
- Firefight_West
- Frontline
- Push_Insurgents / Push_Security
- Skirmish
- Team_Deathmatch
- Survival
- Defusal
- Domination
- Outpost

### Summit (Mountain)
- Ambush_West / Ambush_East
- Checkpoint_Insurgents / Checkpoint_Security
- Firefight_East / Firefight_West
- Frontline
- Push_Insurgents / Push_Security
- Skirmish
- Team_Deathmatch
- Survival
- Domination
- Outpost
- Defusal

### Power Plant
- Ambush
- Checkpoint_Insurgents / Checkpoint_Security
- Domination
- Firefight_East / Firefight_West
- Push_Insurgents / Push_Security
- Survival
- Frontline
- Outpost
- FFA
- Skirmish
- Defusal

### Tell
- Ambush_West / Ambush_East
- Checkpoint_Insurgents / Checkpoint_Security
- Domination_East / Domination_West
- Firefight_East / Firefight_West
- Outpost
- Push_Insurgents / Push_Security
- Survival
- Frontline
- Defusal
- FFA

### Tideway (Buhriz)
- Checkpoint_Insurgents / Checkpoint_Security
- Domination
- Firefight_West
- Frontline
- Push_Insurgents / Push_Security
- Survival
- Outpost
- Ambush
- Defusal

### Citadel
- Push_Insurgents / Push_Security
- Frontline
- Ambush
- Domination
- Firefight
- Defusal
- Checkpoint_Insurgents / Checkpoint_Security
- Outpost
- Survival

### Gap
- Push_Insurgents / Push_Security
- Frontline
- Ambush
- Domination_East / Domination_West
- Firefight_East / Firefight_West
- Defusal
- TDM
- Checkpoint_Insurgents / Checkpoint_Security
- Outpost
- Survival

### Prison
- Push_Insurgents / Push_Security
- Ambush
- Domination
- Firefight
- Defusal
- FFA
- TDM
- Skirmish
- Checkpoint_Insurgents / Checkpoint_Security
- Outpost
- Survival

### LastLight
- Push_Insurgents / Push_Security
- Frontline
- Ambush
- Domination
- Firefight
- Defusal
- TDM
- Skirmish
- Checkpoint_Insurgents / Checkpoint_Security
- Outpost
- Survival

### Trainyard
- Push_Insurgents / Push_Security
- Frontline
- Ambush_East / Ambush_West
- Domination_East / Domination_West
- Firefight_East / Firefight_West
- Defusal_East / Defusal_West
- Checkpoint_Insurgents / Checkpoint_Security
- Outpost
- Survival

### Forest
- Push_Insurgents / Push_Security
- Frontline
- Ambush
- Domination
- Firefight_East / Firefight_West
- Defusal
- FFA
- TDM
- Skirmish
- Checkpoint_Insurgents / Checkpoint_Security
- Outpost
- Survival

### Day/Night
Append to any command: `?Lighting=Day` or `?Lighting=Night`

---

## Official Mutators (Built-in)

### Movement / Combat Pace
| Mutator | Effect |
|---|---|
| `FastMovement` | Move faster |
| `SlowMovement` | Move slower |
| `LockedAim` | Weapons always point to screen center |
| `NoAim` | Aiming down sights disabled |
| `Ultralethal` | One shot kills |
| `BulletSponge` | Increased health |
| `HeadshotOnly` | Only headshots deal damage |
| `Vampirism` | Heal for damage dealt (configurable, see below) |
| `HotPotato` | Dead players drop a live grenade (configurable, see below) |

### Weapon Restrictions
| Mutator | Effect |
|---|---|
| `PistolsOnly` | Pistols + normal gear only |
| `ShotgunsOnly` | Shotguns + normal gear only |
| `BoltActionsOnly` | Bolt-actions + normal gear only |
| `LMGOnly` | Light machine guns + normal gear only |
| `AntiMaterielRiflesOnly` | Anti-materiel rifles + normal gear only |
| `GrenadeLaunchersOnly` | Grenade launchers only |
| `DesertEaglesOnly` | Desert Eagles + normal gear only |
| `MakarovsOnly` | Makarovs only |
| `WelrodsOnly` | Welrod pistols + normal gear only |
| `Welrods` | Everyone forced to use Welrod (not otherwise restricted) |
| `BudgetAntiquing` | Cheap/old weapons only |

### Supply Points (Starting Amount)
| Mutator | Starting Supply |
|---|---|
| `Broke` | 0 |
| `Strapped` | 1 |
| `Guerrillas` | 5 |
| `Warlords` | 10 |
| `SpecialOperations` | 30 |
| `AllYouCanEat` | 100 |
| `Poor` | Limited (low) |
| `SoldierOfFortune` | Gain supply as score increases |

### AI / Enemy Behavior
| Mutator | Effect |
|---|---|
| `Frenzy` | Melee-only AI enemies, with some special enemies |

### Round / Objective Pacing
| Mutator | Effect |
|---|---|
| `Hardcore` | Slower movement + longer capture times |
| `SlowCaptureTimes` | Objectives take longer to capture |
| `Competitive` | Pricier gear, shorter rounds, faster captures |
| `CompetitiveLoadouts` | Swaps player classes to Competitive's set |
| `SmallFirefight` | Adjusts Firefight for fewer players |
| `TieBreaker` | Enables overtime/replay on a draw (Firefight) |
| `ArmsRace` | Every 2 kills = new weapon; win with the final weapon (configurable, see below) |

### UI / Camera
| Mutator | Effect |
|---|---|
| `NoDeathCam` | Disables death camera for everyone |
| `NoThirdPerson` | Disables third-person spectator mode |

### Misc / Server Rules
| Mutator | Effect |
|---|---|
| `FullyLoaded` | Everything unlocked in loadout menu |
| `OfficialRules` | Forces default rules for all modes |
| `NoDrops` | Disables scavenging dropped weapons |
| `Gunslingers` | Revolver + explosives focused loadout |
| `TacticalVoiceChat` | Dead can talk to living; no proximity chat to enemy |
| `ChadTeam666Night` | Bundle: 100 supply + melee/special enemies + vampirism |

### Configurable Official Mutators (add to `Game.ini`)

**ArmsRace** — `[/Script/Insurgency.Mutator_ArmsRace]` *(exact section may vary, confirm in-game)*
```ini
bItemsDrop=False
bEnablePickupItems=False
bScorePoints=True
PenaltyPoints=2
```

**HeadshotOnly** — `[/Script/Insurgency.Mutator_HeadshotOnly]`
```ini
bCheckMeleeDamage=False
```

**HotPotato** — `[/Script/Insurgency.Mutator_HotPotato]`
```ini
bIgnoreHeadshots=False
bBotsOnly=False
```
Travel URL params: `?HotPotato_bIgnoreHeadshots=True` / `?HotPotato_bBotsOnly=True`

**Vampirism** — `[/Script/Insurgency.Mutator_Vampirism]`
```ini
bCountFriendlyFire=False
MaxHealth=1000
```
Travel URL params: `?Vampirism_bCountFriendlyFire=True` / `?Vampirism_MaxHealth=500`

---

## Custom Mod Mutators

### zCore (Framework)
Required only if a mod says it "supports zCore." Add to `Game.ini`:
```ini
[/zCore/Mutators/zCore.zCore_C]
zCoreMods=BlueprintGeneratedClass'/Mod1/Path/zCore_Settings1.zCore_Settings1_C'
```

### ImprovedAI
Mutator: `ImprovedAI` (or `ImprovedAI_2`/`_3`/`_4` for running separate configs simultaneously — not needed for normal use).
Config goes under `[/ImprovedAI/Mutators/ImprovedAI.ImprovedAI_C]` in `Game.ini`. Supports zCore since v2.9.5.

### Reloads Mod
Three independent mutators — add whichever you want active:

| Mutator | Purpose | Config File |
|---|---|---|
| `Reloads` | Faster reload speed | `Game.ini` — `SpeedChoice=Fast/Faster/Fastest` |
| `Bolts` | Faster bolt/pump cycling | `Engine.ini` |
| `Quickdraw` | Faster underbarrel/pistol switching | `Engine.ini` (+ `EnablePistols=True/False` in `Game.ini`) |

Your setup: `SpeedChoice=Faster`, with `Bolts` and `Quickdraw` both included in the mutators list.

### DeathCam
Mutator: `DeathCam`
```ini
[/DeathCam/Mutators/DeathCam.DeathCam_C]
KillerInfo=True
HoloName=True
Xray=True
DeathCamDelay=0.5
DeathCamDistance=200.0
ZoomTime=2.0
ZoomSmoothing=1.0
FreezeCam=False
FreezeTime=1.0
```

### WeaponAnimFix
Mutator: `WeaponAnimFix` (or `WeaponAnimFix_Shadows` for the version with viewmodel shadows enabled). Fixes bolt/slide animation and sight alignment issues, plus scope bump clamping for specific optics.

### CountMutators Pack (Your Defaults)

| Setting | Mutator | Value |
|---|---|---|
| Enemy count | `10E` | Min 10 / Max 20 |
| Friendly bot count | `FB8` | Max allowed (8) |
| AI Difficulty | `Diff10` | Hardest (1.0) |
| Starting supply | `200S` | Max available |
| Supply gain | *(none — default)* | — |
| Friendly fire | `FFOn` | Enabled |
| Kill feed | *(none — default)* | — |
| Vehicles | `VOn` | Enabled |

Skipped (not relevant to your local/solo setup): `Max4P–Max20P` (max players to scale), `BotsUseH/BotsUseB` (bot loadout restriction), `WG0–WG5` / `SW0–SW5` (solo wave increment/start), `Defend0–Defend240` (counterattack duration), weather/lighting mutators (require DynamicWeather mod, not installed).

### HitIndicator
Mutator: `HitIndicator`
```ini
[/HitIndicator/Mutators/HitIndicator.HitIndicator_C]
Crosshair=True
BodyStats=True
HeadShotCount=True
CriticalSoundSelect=1
HeadShotSoundSelect=1
IconColor=(R=1.0,G=1.0,B=1.0,A=1.0)
SkullColor=(R=1.0,G=1.0,B=1.0,A=1.0)
SkullIcon=True
```

### JumpShoot
Mutator: `JumpShoot` — lets you jump and shoot (including ADS) at the same time. Not compatible with mods that change free aim/ADS.

### NoRestrictPlus
Mutator: `NoRestrictPlus` — removes restricted/playable area warnings and volume collisions.
```ini
[/NoRestrictPlus/Mutators/NoRestrictPlus.NoRestrictPlus_C]
RemoveRestricted=True
RemovePlayable=True
RemoveBlockingVolumes=False
RemovePlayerCollision=False
```

### HealthModifier (One Man Army setup — Health only)
Mutator: `healthmodifier` (or `healthmodifier_2` for an alt config instance).
Vanilla player HP is 100 for reference. Your setup: player HP boosted to 350, enemy HP kept at vanilla, only self-heal enabled, bleed/shock/revive/HUD extras trimmed off.
```ini
[/healthmodifier/Mutators/healthmodifier.healthmodifier_C]
bDisplayServerInfo=False

;Health
bEnable_cHP=True
bFixed_cHP=True
f_cHP=350
bEnable_cHPAI=True
bFixed_cHPAI=True
f_cHPAI=100

;Shell Shock (off)
bEnable_shockOnHit=False

;Bleed (neutralized)
f_dmgThreshold=999999
bEnable_stemBleed=False

;Headshot modifiers (off)
bEnable_hsModifier=False
bEnable_hsAIModifier=False

;Medic — self-heal only, no revive/drag
bEnable_healing=True
bEnable_selfHeal=True
bEnable_revive=False
bEnable_drag=False
f_selfHealAmount=25
f_selfHealLimit=350
i_maxMedic=0

;Hud
bShow_HP=True
bShow_BR=False
bShow_medicHud=False
```

### HealthRegen
Mutator: `HealthRegen` — delayed health regen after combat + healing on objective capture/counterattack start. Pairs with HealthModifier above (regen scales off whatever max HP HealthModifier sets).
```ini
[/HealthRegen/Mutator/HealthRegen.HealthRegen_C]
Config=(GameMode="INSCheckpointGameMode",RegenATeam=True,RegenDTeam=True,RegenDelayTime=8.0,RegenLoopTime=1.0,RegenHealthAmount=15.0,RegenHealthLimit=1.0,ObjATeam=True,ObjDTeam=True,ObjHealMode=2,ObjHealStart=0.5,ObjHealEnd=1.0,ObjHealFinalObj=1.0,ObjHealLimit=1.0)
RegenGrunt=True
RegenOverlay=True
```
- Regens 15 HP/sec after 8 seconds without taking damage.
- Heals to 50% at the start of a counterattack, 100% after finishing an objective/counterattack, 100% on the final Checkpoint defend.
- Directly fixes the "alone and low HP when defend timer starts" problem.

### FireSupport Pack
Mutators used: `FreeRadios`, `FS_1`

| Mutator | Effect |
|---|---|
| `FreeRadios` | Every human player gets a radio — Commanders can call fire support without needing an Observer |
| `FS_1` | All fire supports +1 charge |

Other options available in the pack: `FS_2`, `FS_2x`, `FS_3x`, `FS_Inf`, `FS_Inf2`, `NoSmoke`, `NoFS`, `StripFS` (+ `bStripAI`/`bStripHuman` config), `NoDelay`, `NoLimits` (last two override the theater — incompatible with theater mutators/custom loadouts).

### Checkpoint Defend-Phase Tuning
Fixes short defend timers and friendlies not reinforcing fast enough.
```ini
[/Script/Insurgency.INSCheckpointGameMode]
DefendTimer=180
DefendTimerFinal=300
RetreatTimer=20
```

---

## Quick Copy Command (Default)

```
Travel Ministry?Scenario=Scenario_Ministry_Checkpoint_Security?Lighting=Day?Mutators=10E,FB8,Diff10,200S,FFOn,VOn,Vampirism,ImprovedAI,Reloads,Bolts,Quickdraw,HitIndicator,JumpShoot,DeathCam,WeaponAnimFix
```

**One Man Army setup** — low friendlies (4), tanky player, self-heal, objective healing, free fire support radios, still 20+ enemies:

```
Travel Ministry?Scenario=Scenario_Ministry_Checkpoint_Security?Lighting=Day?Mutators=20E,FB4,Diff10,200S,FFOn,VOn,FreeRadios,FS_1,healthmodifier,HealthRegen,Vampirism,ImprovedAI,Reloads,Bolts,Quickdraw,HitIndicator,JumpShoot,DeathCam,WeaponAnimFix,NoRestrictPlus
```

*Full War Setup*
```
Travel Ministry?Scenario=Scenario_Ministry_Checkpoint_Security?Lighting=Day?Mutators=20E,FB8,Diff10,200S,FFOn,VOn,WG5,SW5,Vampirism,ImprovedAI,Reloads,Bolts,Quickdraw,HitIndicator,JumpShoot,DeathCam,WeaponAnimFix
```

Swap `Ministry`/`Scenario_Ministry_Checkpoint_Security` for any map/scenario combo from the reference table above, and add/remove mutators as needed.
