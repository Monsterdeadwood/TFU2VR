> [!IMPORTANT]
> **[TEST BUILDS & DISCUSSION · FLAT2VR DISCORD](https://discord.gg/P4q9zt7ek)**
> Testing, build requests, feedback and discussion happen in the **Flat2VR Modding Discord**. Join the server and find the **The Force Unleashed II** thread.

<p align="center">
  <img src="assets/vr-banner.png" alt="Star Wars: The Force Unleashed II VR — VR" width="500">
</p>

# Star Wars: The Force Unleashed II VR

[Flat2VR Discord](https://discord.gg/P4q9zt7ek) · [All projects](PORTFOLIO.md)

![Project status](assets/vr-status.svg)

Bring Star Wars: The Force Unleashed II into VR with tracked lightsabers, independent hand telekinesis and controller-driven Force powers. R47 fixes how the mod uses blade contact for the game’s original cut joints and keeps impact effects consistent across both eyes.

**Package baseline on this page: OpenXR R47 test package.**

## Installation

1. Ask for **TFU2_OPENXR_R47** in the **The Force Unleashed II** thread on Flat2VR. Install the supported PC game separately.
2. Extract the complete **TFU2_OPENXR_R47** folder. Connect your headset, select the active OpenXR runtime in your PC VR software, then run **RUN.bat** from that folder.
3. If the game is not detected, set **game_directory** in **app/settings.json** to your game folder. For the Steam test path, start Steam before RUN.bat and read the compatibility limits below.
4. Keep the launcher open. For a Flat2VR report, include the headset, XR runtime, game edition and scene. Attach the text-only TELEMETRY ZIP if created, or include the console error if the game fails to start.

Current test-package availability is coordinated in Discord. Use the complete package for your supported game build; this project page is separate from a release download.

## What this project brings to VR

- OpenXR stereo and tracked hand/saber integration in the supported game scenes.
- A saber in each hand, separate trigger toggles and five switchable blade forms. Form one uses the original game blade effect in red with the new hilt; the other forms retain session-random dual colors.
- Independent telekinetic grip for props and enemies: hand reach changes distance, wrist twist rotates the target and release motion throws it.
- Per-hand lightning, shared Force input and a tested way to ride your own held support.
- Editable left/right grip position and rotation, with shared alignment for the palm, hilt, blade and contact.
- Tuned original enemy reactions while retaining stock damage and crystal actions.
- Both blades can sever the game’s prepared enemy parts at supported joints. R47 uses the actual blade pose at impact to select the joint and cut plane.
- A curved screen for menus and movies, controller menu input and updated native audio routing.

<details>
<summary><b>Controller quick reference</b></summary>

| Input | Action |
| --- | --- |
| Each hand’s trigger | Toggle that hand’s saber |
| Each hand’s Grip | Hold a prop/enemy with telekinesis; reach/twist to position it; release motion throws |
| Y left / B right | Lightning from the corresponding hand |
| X left | Shared Force action for both hands; preserves your ridden platform |
| A right | Jump / double jump; exit a ridden support |
| Left stick | Move; while gripping, horizontal input moves held targets sideways and vertical input retains walking |
| Right stick horizontal / vertical | Turn / adjust held-target height; without a grip, vertical input retains separate reverse-grip control |
| Right stick click | Cycle five blade forms |
| Left Menu tap / hold | Recenter / pause |
| Menus and movies: A / B | Confirm / back; release then hold right B at least 0.7 seconds to skip a movie |

The complete package control sheet takes precedence for its version and interaction profile.

</details>

## Features in newer test builds

- **A saber can cut an arm during combat.** In R48, a damaging swing could sever the nearest intact prepared arm while the enemy was still alive. Head and leg cuts use the supported joints after the game's own death event.
- **Hold an enemy with one hand and fight with the other.** In R49, Grip lifted an original hostile Stormtrooper. The same grip survived the brief pause after a saber hit. In a separate test, a gripped crate kept supporting the player through that pause.
- The R49 checks used the GOG game with XR Sim in Cato Neimoidia and Dagobah. Physical-headset testing remains open.

## Current status

**Experimental preview.** R47 tests in the game with XR Sim covered cuts with either controller, the five prepared Stormtrooper parts, physical separation, world-space impact effects in both eyes and recovery after hit-stop.

- The tested game-code path is GOG. The supplied Steam EXE is recognized under guarded checks, but real licensed Steam startup and dependency compatibility still require a tester run.
- R45 tested entry into all nine default campaign worlds and completed the ship-crash QTE. Full campaign and boss playthroughs still need testing. The launcher runs with -noSaving.
- Physical Air Link audio, headset comfort and controller coverage still need testing.

[Detailed status and validation scope](docs/PROJECT_STATUS.md)

## Testing & feedback

Post in the game’s [Flat2VR thread](https://discord.gg/P4q9zt7ek) with your **mod version, game/store version, headset, OpenXR runtime, GPU, reproduction steps and the package’s diagnostic ZIP**. A short video is helpful for visual or handling problems.

<!-- COMMUNITY_TESTERS_START -->
## ❤️ Community testers — thank you!

These VR projects improve thanks to the people sharing test reports, logs, videos and practical feedback across the portfolio.

alvaro · Arkturus [CODA] · Arkturus Primacronus [HD2M] · Arthur G [ORE] · Bestgamer3 · Chtiblue · creative name [SC℧M] · Derp Dog · DNana51 [R1Δ] · Gritt [F2VR] · headbangerle. · huligan01 · jeremiasadasmki · Kerin\_Serica [1984] · kilo · Lawyer [WYRD] · little\_boxbr · Lord Beardsteak · MeWhenINameMyself · MetalikSix · neoz\_1980 · Notagameaddict · Pelmeschka · Potato Pancake Person · ReseTV · Rusty Gere · SilentBang [LTS] · SilentVortigaunt · Terry · ThE LaNd GuLl · Thomas-3D-VR · Uruz [F2VR] · Willthethrill · wxorys\_ · Xavier H. G.

[Full community credits, games, feedback contributors and testing volunteers](TESTERS.md).

The linked list shows which games each person helped with. Thank you as well to everyone whose reports arrived without a public display name.

<!-- COMMUNITY_TESTERS_END -->

## Other VR mods by Monsterdeadwood

| Game / project | Focus | Visibility |
| --- | --- | --- |
| [Assassin’s Creed VR](https://github.com/Monsterdeadwood/AC1VR) | First-person exploration, climbing and sword interaction | Private |
| [Crysis 2: VRevamp](https://github.com/Monsterdeadwood/C2VR) | Nanosuit combat, physical interaction and spatial UI | Public |
| [NOVA · CS:GO Legacy VR](https://github.com/Monsterdeadwood/CSGOVR) | CS:GO Legacy local matches with motion controls | Public |
| [TimeShift VR](https://github.com/Monsterdeadwood/TimeShiftVR) | Time powers, nine weapons and roomscale posture | Public |
| [You Are Empty: Absolute Edition VR](https://github.com/Monsterdeadwood/YouAreEmptyAEVR) | Absolute Edition VR, weapons and hand interaction | Public |
| [Alone in the Dark 2008 VR](https://github.com/Monsterdeadwood/AloneInTheDark2008VR) | Survival-horror VR and held-item interaction | Public |
| [Rainbow Six Siege VR](https://github.com/Monsterdeadwood/SiegeVR) | Legacy Siege stereo and tracked weapon handling | Public |
| [Burnout Paradise Remastered VR](https://github.com/Monsterdeadwood/BUrnOutPvr) | Stereo driving, vehicle menus and native effects | Public |
| [Titanfall 1 VR](https://github.com/Monsterdeadwood/Titanfall1VR) | Pilot combat and Titan cockpit VR | Public |
| [Metro 2033 VR](https://github.com/Monsterdeadwood/Metro2033VR) | Original Metro VR and native physics experiments | Public |
| [Insurgency VR](https://github.com/Monsterdeadwood/InsurgencyVR) | Early VR integration research | Private |
| [Counter-Strike: Source VR](https://github.com/Monsterdeadwood/CSSVR) | Counter-Strike: Source VR development | Private |

Private repository links are available to invited collaborators. Public project pages are marked above.

## Credits & development notes

Project maintained by [Monsterdeadwood](https://github.com/Monsterdeadwood). This is an independent fan VR project; you need your own supported copy of the original game.

Documentation reviewed: **15 November 2026**.
