# MainSequence-Framework

Shared MSCore-backed world lifetime, input ownership and addon support.

## Requirements

Main Sequence, single-player; MSCore 0.8.13 and a compatible UE4SS installation. Install this support package before its feature addons.

## Install and update

Add `pobkac-svg/MainSequence-Framework` in MSCore Manager. Save and fully restart after installation or updates. Do not enable the old standalone mods alongside these addons. Keep saves, Designs and underground companion files.

## Controls

This is shared support; it has no gameplay key bindings.

## Troubleshooting and removal

Check `ue4ss/UE4SS.log` and `Mods/MSCore/selfcheck.log`. Close the game before Manager removal. Remove dependent feature addons before removing this shared support package.

## Release status

Version 0.3.6: the clean combined build was functionally confirmed by the user on 22 November 2026. An earlier diagnostic with the array corrections ran for over an hour with eleven saves on the affected large save without a crash. The final clean-build long-run duration was not separately measured. Tested with UE4SS 4.0.0; no claim that this resolves every native crash or the severe large-save FPS drop.

## Credits and terms

Developed with OpenAI Codex. Uses MSCore by xxalex3xx97 and UE4SS as external dependencies. Unofficial; not affiliated with the game developer. This repository contains release documentation, with runtime files supplied as release downloads. Development source, extracted game data and saves are excluded. No third-party licence is granted; our own code is licensed under MIT (see LICENSE). Game assets and dependencies are excluded from that grant.

## Manager dependency metadata correction

Release 0.3.4 fixes matching `requires` fields in the download manifest and installed `mscore.mod`. Gameplay is unchanged. Install/update this release before feature addons.

## Performance update

Release 0.3.5: Cache and revalidate the WidgetSubsystem identity instead of repeatedly searching all objects during UI checks. Tested by the user with only MSCore, Framework and Belt Meter enabled, with no observed slowdowns. The originally affected friend PC has not retested.

## 0.3.6 update

- Avoid native TArray callback iteration in shared array reads; guard indexed reads against size changes.
- Honour Framework addon overrides, explicit mods.txt disable entries and managed-package enabled.txt markers before loading addon code.
- Add validated game inventory-total snapshots for Storage Counts.

Save, fully close the game and update Framework first, then the installed feature addons. Fully restart after updating.
