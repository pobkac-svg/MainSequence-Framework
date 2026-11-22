# Changelog

## 0.3.6 ? 2026-11-22

- Avoid native TArray callback iteration in shared array reads; guard indexed reads against size changes.
- Honour Framework addon overrides, explicit mods.txt disable entries and managed-package enabled.txt markers before loading addon code.
- Add validated game inventory-total snapshots for Storage Counts.

## 0.3.5

- Cache and revalidate the WidgetSubsystem identity to avoid repeated global discovery.
- User reports smooth operation in the isolated three-mod test.
- Promoted to stable; runtime files are identical to the performance-test build.

## 0.3.4

- Fix MSCore Manager rejection by matching dependency metadata in manifest.txt and mscore.mod.
- Retains MSCore 0.8.13 dependency.
- Packaging/metadata correction; gameplay is unchanged.

## 0.3.3

- MSCore-backed release preparation.
- Existing gameplay preserved and user-tested.
- Manager-compatible ZIP and checksummed manifest prepared.
