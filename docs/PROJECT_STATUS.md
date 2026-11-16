# Star Wars: The Force Unleashed II VR — project status

[← Project page](../README.md) · [Flat2VR testing & discussion](https://discord.gg/P4q9zt7ek)

Reviewed **15 November 2026**. Documented branch: **OpenXR R47 test package**.

## What has been checked

- R47 tests in the game with XR Sim covered cuts with either controller, the five prepared Stormtrooper parts, physical separation, world-space impact effects in both eyes and recovery after hit-stop.
- A tester previously reported Virtual Desktop working on GOG. R47 visuals and audio still need physical-headset testing.
- The R47 archive passed its launcher check after fresh extraction. R46 is the rollback package.

## Follow-up tests reviewed 16 November 2026

R48 extended prepared-arm cuts to native damaging swings against a live target. R49 exercised lifting an original hostile Stormtrooper, holding through saber hit-stop, original release and riding a held crate in two GOG scenes with XR Sim. The original Quit route exited cleanly. R47 remains the earlier test package described above.

Verification records used for this section

- `TFU2_OPENXR_R49/README.txt`
- `TFU2_OPENXR_R49/evidence/VERIFICATION_R49.json`

## Current limits

- The tested game-code path is GOG. The supplied Steam EXE is recognized under guarded checks, but real licensed Steam startup and dependency compatibility still require a tester run.
- R45 tested entry into all nine default campaign worlds and completed the ship-crash QTE. Full campaign and boss playthroughs still need testing. The launcher runs with -noSaving.
- Physical Air Link audio, headset comfort and controller coverage still need testing.

## Build access

Ask for the current complete test package in the game’s Flat2VR thread. A local build record does not by itself mean a file has been uploaded to this repository’s Releases.

## Documentation basis

This overview was reconciled against the project’s recorded package notes and validation records. The following names identify the records reviewed; they are not download links:

- `TFU2_OPENXR_R47/README.txt`
- `TFU2_OPENXR_R47/evidence/VERIFICATION_R47.json`
- `TFU2_OPENXR_R47_RECEIPT.json`

Game execution, simulator validation and physical-headset feedback are reported separately above. Features from a separate experimental branch are identified explicitly.
