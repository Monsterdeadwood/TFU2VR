# Star Wars: The Force Unleashed II VR — project status

[← Project page](../README.md) · [Flat2VR testing & discussion](https://discord.gg/P4q9zt7ek)

Reviewed **14 November 2026**. Documented branch: **OpenXR R44**.

## What has been checked

- R44 checks used the actual supported game with XR Sim and two rendered eyes. Recorded cases cover blade rendering, native enemy reactions, nonzero grip calibration, held-platform movement and audio API routing, with save/configuration restoration after the checked runs.
- A tester has reported Virtual Desktop working on GOG. The current R44 image, enemy-response and audio changes still need their own physical-headset assessment.
- The R44 archive passed cold extraction and launcher checks, with the previous R43 package preserved.

## Current limits

- The tested game-code path is GOG. The supplied Steam EXE is recognized under guarded checks, but real licensed Steam startup and dependency compatibility still require a tester run.
- RND_1 (opening Kamino), DAG_1 and REB_1 have supported paths; the whole campaign is not qualified. The package documents a test launch with -noSaving.
- Physical Air Link audio, headset comfort/weight perception and broad controller coverage remain open. R44 makes no general FPS-improvement claim.

## Build access

Ask for the current complete test package in the game’s Flat2VR thread. A local build record does not by itself mean a file has been uploaded to this repository’s Releases.

## Documentation basis

This overview was reconciled against the project’s recorded package notes and validation records. The following names identify the records reviewed; they are not download links:

- `TFU2_OPENXR_R44/README_RU.txt`
- `TFU2_OPENXR_R44/DISCORD_POST_EN.txt`
- `TFU2_OPENXR_R44/evidence/R44_VERIFICATION.json`
- `TFU2_OPENXR_R44_RECEIPT.json`

Game execution, simulator validation and physical-headset feedback are reported separately above. Features from a separate experimental branch are identified explicitly.

## Кратко по-русски

VR-мод Star Wars: The Force Unleashed II: световые мечи от контроллеров, независимый телекинез рук и управление Силой. R44 объединяет пять форм клинка, настройку хвата, родные реакции врагов и проверенный VR-маршрут начала Камино.

- Проверенный игровой код — GOG. Присланный Steam EXE распознаётся с защитными проверками, но настоящий лицензионный Steam-запуск и совместимость его зависимостей ещё требуют теста.
- Есть поддерживаемые маршруты RND_1 (начало Камино), DAG_1 и REB_1; вся кампания ещё не проверена. В пакете описан тестовый запуск с -noSaving.
- Физическое прослушивание Air Link, удобство/ощущение веса в шлеме и широкий набор контроллеров ещё требуют проверки. Общий прирост FPS в R44 не заявляется.
