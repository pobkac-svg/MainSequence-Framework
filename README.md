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

Version 0.3.5: gameplay and Manager testing confirmed by the user on 20 November 2026. Release downloads include the runtime ZIP and its checksummed MSCore manifest. Tested with the existing UE4SS 4.0.0 installation and the current installed game update; other builds are not verified.

## Credits and terms

Developed with OpenAI Codex. Uses MSCore by xxalex3xx97 and UE4SS as external dependencies. Unofficial; not affiliated with the game developer. This repository contains release documentation, with runtime files supplied as release downloads. Development source, extracted game data and saves are excluded. No third-party licence is granted; our own code is licensed under MIT (see LICENSE). Game assets and dependencies are excluded from that grant.

## Manager dependency metadata correction

Release 0.3.4 fixes matching `requires` fields in the download manifest and installed `mscore.mod`. Gameplay is unchanged. Install/update this release before feature addons.

## Performance update

Release 0.3.5: Cache and revalidate the WidgetSubsystem identity instead of repeatedly searching all objects during UI checks. Tested by the user with only MSCore, Framework and Belt Meter enabled, with no observed slowdowns. The originally affected friend PC has not retested.
