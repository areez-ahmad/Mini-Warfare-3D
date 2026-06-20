# Sprint 5 — Scripting
**Date:** June 18, 2026 (Thursday) | **Course:** Game Programming (GP) | **Instructor:** Dr. Amna Lodhi

## What was done
This sprint covers the gameplay/network programming layer of the Boss Room multiplayer project — the C# scripts that drive player control, networked connection state, server/client gameplay logic, AI, UI, and infrastructure systems.

### Script breakdown (`Assets/Scripts/`)
| Folder | Files | Responsibility |
|---|---|---|
| `Gameplay/` | 138 | Core gameplay: characters, actions/abilities, AI states, projectiles, UI, game state machine (char select, boss room, post-game), debug cheats |
| `ConnectionManagement/` | 11 | Client/host connection state machine (offline, connecting, hosting, reconnecting) |
| `Utils/` | 13 | Network overlay/stats, lerpers, prefab spawner, client prefs, profile manager |
| `Infrastructure/` | 16 | Pub/Sub messaging (MessageChannel), ScriptableObject event architecture, network object pooling |
| `UnityServices/` | 8 | Authentication and multiplayer session/lobby service facades |
| `VisualEffects/` | 3 | Special FX graphics, randomized lighting, scrolling material UVs |
| `Editor/` | 3 | Editor tooling (baking menu, build helpers, scene bootstrapper) |
| `Audio/` | 2 | Audio mixer config, client music player |
| `ApplicationLifecycle/` | 2 | App-level startup/quit handling |
| `Navigation/` | 2 | Dynamic nav-path system |
| `CameraUtils/` | 1 | Camera controller |

### Additional
- `Assets/Tests/Runtime/` — 4 automated test scripts (connection management, message channels, host/disconnect flow)
- `Assets/Editor/Tutorials/` — in-editor tutorial callback script

**Note for documentation:** this codebase is derived from Unity Technologies' official **Boss Room** multiplayer sample project (`Unity.BossRoom` namespace), adapted for this project's multiplayer gameplay. Original authorship/source is credited here for academic integrity — any custom modifications made for this assignment should be called out separately in commit messages.

## GitHub upload notes
- All 472 files in this sprint are plain-text C#/`.meta`/`.asmdef` files — **largest file is ~28 KB**, total folder size ~2.5 MB.
- ✅ Well under GitHub's 100 MB per-file hard limit (and the 50 MB soft-warning threshold) — safe to push directly, no Git LFS needed.
- No binary assets, textures, or LFS pointer files are included in this folder.

## Deliverable
Script files (`/Sprint5_Scripting/Assets/Scripts`, `/Assets/Tests`, `/Assets/Editor`) pushed to GitHub with documented structure.

## Status
✅ Complete
