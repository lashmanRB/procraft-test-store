# ProCraft test store

A catalogue for testing the store: add it by its address and the app lists everything below,
fetches the file it needs and checks it against the size and digest written here.

Add this address in the store's Settings, Add a source:

    https://raw.githubusercontent.com/lashmanRB/procraft-test-store/main/catalogue.json

## What it lists

Brush sets, from `assets/`:

- RSCO_Broken_Inkers.brushset
- RSCO_Dead_Pen.brushset
- RSCO_IndustryPress.brushset
- RSCO_Inferno_Ink_Spatter_Stamps.brushset
- RSCO_Ink_Bleed.brushset
- RSCO_Ink_Spray.brushset
- RSCO_MonoMagic_Line_Builders.brushset

Paper packs, from `assets/`:

- Cardstock-Cover-Stock.assetset
- Coated-Glossy-Stock-Modern.assetset
- BFK-Rives.assetset
- Bond-Paper.assetset
- Bristol-Board-Smooth.assetset
- Cartridge-Paper.assetset

## Notes

- Every `bytes` and `sha256` in `catalogue.json` was taken from the file as committed. Change a
  file and the catalogue has to change with it, or the store will refuse the download.
- The app installs brush sets into its brush library. Asset packs are listed, and installing one
  is refused while the app has no asset library to take it.
- This repository is test material: the files are here so a store can be exercised end to end,
  not for distribution.
