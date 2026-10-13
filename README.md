# lightcraft-ko-patch

Korean (한국어) interface patch for **[LightCraft](https://github.com/storytold/lightcraft)** (Lightroom-style photo editor), upstream tag `v0.6.0`.
This repository contains **only the patch**, not LightCraft's source code. See `BASE.txt` for the exact upstream commit.

## Apply
```bash
git clone --branch v0.6.0 https://github.com/storytold/lightcraft.git && cd lightcraft
git apply ../lightcraft-ko-patch/patches/lightcraft-v0.6.0-ko.patch
```
Then build as upstream documents (release builds embed fonts with `CRAFT_FONTS_DIR`).
Unofficial Windows cross-build: see [artcraft-ko-toolkit](../artcraft-ko-toolkit).

## What it changes
New Korean catalog (2,096 strings + 230 formats) with Lightroom Korean terminology (노출, 밝은 영역, 텍스처, 디헤이즈 …); Korean date/number formats.
Changed files: `CHANGED-FILES.txt`.

## Verified
63 i18n tests + 3 font tests; all 11,172 Hangul syllables covered by the bundled Noto Sans CJK; Windows headless render without tofu.

## Known limits
AI translation, not native-reviewed; What's New notes stay English.

Translations are AI-assisted (Claude Opus 5.5) and not reviewed by a professional translator.
Licence: MIT OR Apache-2.0, same as LightCraft; upstream contributions credited above.
