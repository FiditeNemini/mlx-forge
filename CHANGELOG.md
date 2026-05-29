# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.4.0](https://github.com/FiditeNemini/mlx-forge/compare/v0.3.0...v0.4.0) (2026-05-29)


### ⚠ BREAKING CHANGES

* the convert/validate recipe names change from `vjepa2-vitl` / `vjepa2-vit-l-rope` to `vjepa-2.0-vitl` / `vjepa-2.1-vitl`.

### Features

* add --dry-run to convert command ([855b38c](https://github.com/FiditeNemini/mlx-forge/commit/855b38cc15441e221a88fd374186c9b2ea82184d))
* add CogVideoX-Fun conversion recipe ([cda2c01](https://github.com/FiditeNemini/mlx-forge/commit/cda2c0149acbff3c801090c062a2297d088b6dc2))
* add error handling, upload validation, and test coverage ([38c4e83](https://github.com/FiditeNemini/mlx-forge/commit/38c4e8354d1f8c96d6e03bcc22bf468a2937b3c8))
* add Fish S2 Pro recipe (Phase 1 — transformers only) ([ac72daf](https://github.com/FiditeNemini/mlx-forge/commit/ac72daf7e9bcaedd131268a83bac794b18a7d811))
* add Matrix-Game-3 conversion recipe ([91431e7](https://github.com/FiditeNemini/mlx-forge/commit/91431e70dc20ae72061d0cd4cd8962f52d92d108))
* add Matrix-Game-mlx implementation link to model card ([a581bb7](https://github.com/FiditeNemini/mlx-forge/commit/a581bb7a8a499a9fb09a5c9acfdb486e80cc65c5))
* add Mistral Small 3.1 24B recipe (language + vision + projector) ([4ab0376](https://github.com/FiditeNemini/mlx-forge/commit/4ab0376cd59fcad1bf2e949d6fe55cbcd3b1e4bf))
* add Qwen-Image-2512 recipe (57B text-to-image MMDiT) ([1991dfc](https://github.com/FiditeNemini/mlx-forge/commit/1991dfcd54f585c984a56df884a95e41dc96bb84))
* add spatial/temporal upscaler support to LTX-2.3 recipe ([e48ab7f](https://github.com/FiditeNemini/mlx-forge/commit/e48ab7f4943eb1d60a35316f92793e6557174926))
* add upload command — push converted models to HuggingFace Hub ([d9bebea](https://github.com/FiditeNemini/mlx-forge/commit/d9bebea3c3bafb16741f705c1abd153cda43c571))
* add void-model recipe for Netflix VOID weight conversion ([dbef988](https://github.com/FiditeNemini/mlx-forge/commit/dbef988eea27eda0874644b6ee2ce33363efd0b7))
* codec DAC, integration tests, CI smoke tests ([1d357e1](https://github.com/FiditeNemini/mlx-forge/commit/1d357e14053b338be7acfddea8dbf1fa5109aacc))
* complete CogVideoX-Fun recipe + add mlx-recipe skill ([a9c5ee5](https://github.com/FiditeNemini/mlx-forge/commit/a9c5ee551be38cf2f5d11de995b2753188437b6f))
* convert all Matrix-Game-3.0 variants (distilled DiT + LightVAE) ([fe87952](https://github.com/FiditeNemini/mlx-forge/commit/fe8795204babac1bbcebcbe2bb372daf4d3898c2))
* download HF checkpoints to ./models/ instead of HF cache ([4f7ee5c](https://github.com/FiditeNemini/mlx-forge/commit/4f7ee5c54b0b922b68428fdc3e8e3e25c8b6c947))
* initial mlx-forge — convert, quantize, split, validate ML models for MLX ([75dd047](https://github.com/FiditeNemini/mlx-forge/commit/75dd0476c2cc2782e65483a940c8885c09f24f2a))
* **ltx-2.3:** add --skip-shared flag (argparse only) ([3eda189](https://github.com/FiditeNemini/mlx-forge/commit/3eda1897e67b5ab199a877211623967074e25b0d))
* **ltx-2.3:** add distilled-1.1 variant + LoRA 1.1 ([7c0bd38](https://github.com/FiditeNemini/mlx-forge/commit/7c0bd38a097fa0a237952d4421898cf594ec378d))
* **ltx-2.3:** extract audio VAE encoder weights ([ef6e0ec](https://github.com/FiditeNemini/mlx-forge/commit/ef6e0ec96ab8ba4b0acdfa927e8bfd99bf6d5765))
* **ltx-2.3:** honor --skip-shared in convert flow + emit delta in split_model.json ([0336d6c](https://github.com/FiditeNemini/mlx-forge/commit/0336d6cabc64826cbd7998b98c3bb3a947172f86))
* **ltx-2.3:** unify dev/distilled variants in single repo ([aba53b8](https://github.com/FiditeNemini/mlx-forge/commit/aba53b876d5ab3685d885f10a85fd886b643265c))
* **ltx-2.3:** validate auto-detects delta mode (skips shared checks) ([1e41513](https://github.com/FiditeNemini/mlx-forge/commit/1e415139a77bb2b834d11a23e5028ea1a925d057))
* **recipe:** add ernie-image-pe for Baidu Prompt Enhancer ([7581f03](https://github.com/FiditeNemini/mlx-forge/commit/7581f03f797872b12816b0dcf3396ff4a6fd62c2))
* **recipe:** add Hunyuan3D-2.1 shape generation conversion recipe ([bf93205](https://github.com/FiditeNemini/mlx-forge/commit/bf932057f29b1b3b0bf5d2c1b9b8ffff1980827c))
* **recipe:** add paint stage to hunyuan3d-2.1 recipe ([9097f21](https://github.com/FiditeNemini/mlx-forge/commit/9097f21d782c609a70b82dff69f0f20b044bb2ca))
* **recipes:** add vjepa2-vit-l-rope conversion recipe ([#8](https://github.com/FiditeNemini/mlx-forge/issues/8)) ([5fdb51c](https://github.com/FiditeNemini/mlx-forge/commit/5fdb51c4b5df24b6853e501e9882e3348336e6a1))
* **recipes:** add vjepa2-vitl (V-JEPA 2.0 ViT-L + attentive probes) ([#9](https://github.com/FiditeNemini/mlx-forge/issues/9)) ([be2b5de](https://github.com/FiditeNemini/mlx-forge/commit/be2b5de3d25fbdaddd1f1aa3e9bcd78713529167))
* **upload:** --card-only + --cli-snippet for Usage section ([4900264](https://github.com/FiditeNemini/mlx-forge/commit/4900264b323023edeeee9498fed7920be5eebad5))
* **upload:** --card-only derives variants from remote repo ([c2b512c](https://github.com/FiditeNemini/mlx-forge/commit/c2b512ccccd68e7c767d8b01ba31d159b6d3b174))
* **upload:** add --link flag for related projects in model card ([a7adf91](https://github.com/FiditeNemini/mlx-forge/commit/a7adf9187b6ca130f25b978f68729c43994cb140))
* **upload:** add --usage-url flag for model card ([c292961](https://github.com/FiditeNemini/mlx-forge/commit/c2929611e265359626b216fabc8890f713058356))
* **upload:** implement --add-only (skip files present on remote) ([7e12de4](https://github.com/FiditeNemini/mlx-forge/commit/7e12de425859411580f52fce976baccd877e7e5e))
* **upload:** wire --add-only flag through CLI (no-op behavior) ([baf7735](https://github.com/FiditeNemini/mlx-forge/commit/baf77358a5fb2fbe7a84262c81067f3fe25ff915))
* use ./models/ as default output directory ([f2a7728](https://github.com/FiditeNemini/mlx-forge/commit/f2a772817f039574c8a0eee1f6b7cd8952b6a4bd))
* warn when tensors are skipped during quantization ([b7a7f28](https://github.com/FiditeNemini/mlx-forge/commit/b7a7f2860f3d103118969c8fb657d87e0b7e6e48))


### Bug Fixes

* add model version to recipe naming (cogvideo-fun-v1.5-5b-inp) ([ef9195f](https://github.com/FiditeNemini/mlx-forge/commit/ef9195ffc05465dd538197f03b1212a80c802f2a))
* auto-download VOID weights from HuggingFace when --source not specified ([c726606](https://github.com/FiditeNemini/mlx-forge/commit/c7266060ad25a5de0f3db7a7c316cf50b53cc187))
* **ci:** use uvx for lint, --extra dev for test dependencies ([ebd8831](https://github.com/FiditeNemini/mlx-forge/commit/ebd883111e7c09492cf1958783978cf4a2a15640))
* codec.pth loading (torch + bfloat16) and audio_decoder validation ([4529053](https://github.com/FiditeNemini/mlx-forge/commit/452905342562b8f2a3f407cdb607a2d5ddd7e833))
* correct Mistral Small 3.1 key prefixes and validation ([03cd41c](https://github.com/FiditeNemini/mlx-forge/commit/03cd41cf74235d0f792b3b148500c705c6b86faf))
* correct weight conversion for matrix-game-3.0 ([5010312](https://github.com/FiditeNemini/mlx-forge/commit/50103121457450e0676c667ac871b0cdedeee55a))
* **delta-workflow:** address final-review findings (components inventory, README, mutex, validate test) ([d1cd4eb](https://github.com/FiditeNemini/mlx-forge/commit/d1cd4eb78b628aa1a528e5b6a0609d45be19a64e))
* detect forward_basis/inverse_basis as conv buffers needing transpose ([c398b07](https://github.com/FiditeNemini/mlx-forge/commit/c398b07b96d43507486f848ac19296632fd2fd63))
* download to per-model subdirectories to avoid file conflicts ([35e3cbc](https://github.com/FiditeNemini/mlx-forge/commit/35e3cbc84dbb09e6dfed11d6ac625409b0a08220))
* **hunyuan3d:** write 'source' field to split_model.json ([3cc33f2](https://github.com/FiditeNemini/mlx-forge/commit/3cc33f2a88f585c4daad7aad7d4a62c7663f71ec))
* include version in upscaler filenames (v1.0, v1.1) ([9df0755](https://github.com/FiditeNemini/mlx-forge/commit/9df07556490428244c4c5128e911bfa5c95d3bbc))
* lint — remove unused import, fix formatting ([c10f33c](https://github.com/FiditeNemini/mlx-forge/commit/c10f33c2666aa5a2cb722e73db384ed4bfe23e0d))
* **ltx-2.3:** update validation for audio VAE encoder keys ([3e90557](https://github.com/FiditeNemini/mlx-forge/commit/3e9055787ceb04376a398a0893ca76eb1c4ba28f))
* never quantize T5 text_encoder (keep bf16 for all quant levels) ([8e06eb2](https://github.com/FiditeNemini/mlx-forge/commit/8e06eb20c89830ed83ab74018602de1e57bb5dba))
* pass block_key to validate_quantization in qwen-image-2512 ([05feea9](https://github.com/FiditeNemini/mlx-forge/commit/05feea9ff5352080af01e8074f0343f5b9146742))
* pre-convert ConvTranspose1d weights in LTX-2.3 vocoder ([553284a](https://github.com/FiditeNemini/mlx-forge/commit/553284a19b6ef2139a84ccec732cadaab68cb50c))
* **recipe:** remove fourier_embedder validation check ([17d53de](https://github.com/FiditeNemini/mlx-forge/commit/17d53de30fcca103814d44c1524467011abd6a8c))
* **recipes:** version the V-JEPA 2 default output dirs to match HF naming ([#12](https://github.com/FiditeNemini/mlx-forge/issues/12)) ([40d8130](https://github.com/FiditeNemini/mlx-forge/commit/40d81300e6c0628364c9bc1f5a9074def0074d9e))
* rename matrix-game-3 recipe to matrix-game-3.0 ([030c837](https://github.com/FiditeNemini/mlx-forge/commit/030c837f18e7fac25dc23fe370e1ff7c95b34b0f))
* replace deprecated hf_transfer with hf-xet high performance mode ([b795822](https://github.com/FiditeNemini/mlx-forge/commit/b7958226bc4e77528685b24c286fec62a0c1b948))
* scale_shift_table validation for distilled variant ([c13a883](https://github.com/FiditeNemini/mlx-forge/commit/c13a883ca5dd257c8ee636e073fbe667c9609068))
* skip T5 text_encoder quantization at 4-bit ([172eeb7](https://github.com/FiditeNemini/mlx-forge/commit/172eeb791e3b97334b91fc57f35a4bc86dc4ed86))
* skip txt_in from quantization in qwen-image-2512 ([740ebb8](https://github.com/FiditeNemini/mlx-forge/commit/740ebb84efe2c2db869d68f9d3e4f8e8f7c11122))
* squeeze VAE RMS_norm gamma to 1D for MLX channels-last ([829e6b2](https://github.com/FiditeNemini/mlx-forge/commit/829e6b2deb14a0b1b89d50efc08d05ffe8e28ed2))
* store DiT distilled weights in bfloat16 instead of float32 ([7bffb14](https://github.com/FiditeNemini/mlx-forge/commit/7bffb14ea27ba1b6bb28fb7d25f4ec9dfa76c173))
* support multiple block_keys in validate_quantization ([60bdf1e](https://github.com/FiditeNemini/mlx-forge/commit/60bdf1ea5c3679d86838c8e9f1881e23887d2c98))
* transpose conv-like buffers (filter, basis, kernel) in vocoder and upscaler ([faf5170](https://github.com/FiditeNemini/mlx-forge/commit/faf5170943584fda58fe22070e62e85e3bb9da48))
* **upload:** clearer error when --add-only is given a missing model_dir ([67d62fb](https://github.com/FiditeNemini/mlx-forge/commit/67d62fb0a58a0bced35c2388b462e883c5863a8d))
* **upload:** filter empty variants + test --card-only network fallback ([4388f11](https://github.com/FiditeNemini/mlx-forge/commit/4388f11b495d982ff4cf3f9edda2676a92e6ece7))
* **upload:** keep dir-name -q{bits} in derive_repo_id when split omits it ([#11](https://github.com/FiditeNemini/mlx-forge/issues/11)) ([0afd51c](https://github.com/FiditeNemini/mlx-forge/commit/0afd51cce3c5c26e767a2c815621eedf3e3bec68))
* **upload:** strip existing -mlx suffix in derive_repo_id ([#10](https://github.com/FiditeNemini/mlx-forge/issues/10)) ([b15ef28](https://github.com/FiditeNemini/mlx-forge/commit/b15ef2826191d820964a84c0a4270d0fc3b1c085))
* use torch.load for .pth files in matrix-game-3.0 recipe ([83514a0](https://github.com/FiditeNemini/mlx-forge/commit/83514a0ce652d44263e3e6a2a67f22d493160d64))
* validation skips T5 quantization checks when text_encoder is in skip_components ([7dd90db](https://github.com/FiditeNemini/mlx-forge/commit/7dd90db0e49632e8078bc5df03c63be8894b0830))


### Documentation

* add all known LTX-2.3 conversion/quantization gotchas ([cb80046](https://github.com/FiditeNemini/mlx-forge/commit/cb80046ec51037cc3d92715d0d04d96a9a0fbc67))
* add conversion, quantization, and splitting guides ([a894798](https://github.com/FiditeNemini/mlx-forge/commit/a8947985577a276ca1bb3249e02923054a517738))
* add docs/models/vjepa-2.md model guide ([#17](https://github.com/FiditeNemini/mlx-forge/issues/17)) ([e5a7bb3](https://github.com/FiditeNemini/mlx-forge/commit/e5a7bb31a8d0e81ffdbdfab43ddb79baf856bb3d))
* add Fish S2 Pro model guide and usage examples ([d26f295](https://github.com/FiditeNemini/mlx-forge/commit/d26f29586da80aee9c9dc2749bc1f025885fab97))
* add Mistral Small 3.1 model guide and update all references ([9d8f98e](https://github.com/FiditeNemini/mlx-forge/commit/9d8f98e2c7ff000ca5f2be6c565e843afb024f6c))
* add the V-JEPA 2 recipes to the README ([#15](https://github.com/FiditeNemini/mlx-forge/issues/15)) ([f8cc8fc](https://github.com/FiditeNemini/mlx-forge/commit/f8cc8fcdbb90ee8213a8943938dde571833c7379))
* **changelog:** release notes for v0.1.0 ([#3](https://github.com/FiditeNemini/mlx-forge/issues/3)) ([b1a1b71](https://github.com/FiditeNemini/mlx-forge/commit/b1a1b71b45e1f57c1b5e382dc034815c97387cc0))
* cross-link the porting-pytorch-to-mlx Claude Code skill ([36b8de4](https://github.com/FiditeNemini/mlx-forge/commit/36b8de4bb7e8257bdcda5244d0a8d166610967dd))
* delta workflow (CLAUDE.md) + model card template (mlx-recipe skill) ([774307c](https://github.com/FiditeNemini/mlx-forge/commit/774307ccdb46278b11b5e5165d2e380768bfccbf))
* document --dry-run flag and add test ([dec4366](https://github.com/FiditeNemini/mlx-forge/commit/dec4366b3974cddce31462be4924d6cf830da70b))
* document conv-like buffer transposition and temporal-upscaler scale args ([efb12d6](https://github.com/FiditeNemini/mlx-forge/commit/efb12d68f9044ad8f69716b9481f4ba864574288))
* move LTX-specific content from README to model doc ([250bcae](https://github.com/FiditeNemini/mlx-forge/commit/250bcae00f9417c15ee2dfbc54acd8007aad2dcb))
* **plan:** delta-workflow improvements implementation plan ([4c794e2](https://github.com/FiditeNemini/mlx-forge/commit/4c794e2874f9d76dd241481ca0fa2d694748fdff))
* separate generic concepts from LTX-2.3 specifics ([8952be1](https://github.com/FiditeNemini/mlx-forge/commit/8952be166d604da286ccf29c32d7130ab7c9e617))
* skill must auto-download from HuggingFace when --source not given ([6107aea](https://github.com/FiditeNemini/mlx-forge/commit/6107aeadc7dd005ae824b88e459526b4d99ee3b6))
* **spec:** delta-workflow improvements design ([5ef5aed](https://github.com/FiditeNemini/mlx-forge/commit/5ef5aede96809c3d92b19fb4baaa3eaa3c3b7ca0))
* update all docs for codec DAC, convert.py, and torch dependency ([55839fd](https://github.com/FiditeNemini/mlx-forge/commit/55839fd744f7d9fc6d0152081c0c695542ac09af))
* update README with Fish S2 Pro stable status and codec ([e698e72](https://github.com/FiditeNemini/mlx-forge/commit/e698e7223f896225cc4be2a5bf365e5a6fb358bd))
* update README with ltx-2.3 recipe name and --key-prefix flag ([2f477ed](https://github.com/FiditeNemini/mlx-forge/commit/2f477ed66f187b5a1f50e87abea017b0052c68be))
* update skill cross-link name (porting-pytorch-to-mlx -&gt; mlx-porting) ([69f5f16](https://github.com/FiditeNemini/mlx-forge/commit/69f5f16d8750d357a793e9eecbe65a65231e9f98))


### Code Refactoring

* rename V-JEPA 2 recipes to the versioned scheme ([#18](https://github.com/FiditeNemini/mlx-forge/issues/18)) ([2cd2bb5](https://github.com/FiditeNemini/mlx-forge/commit/2cd2bb50ddb11031173dfac5f74353c45f716b18))

## [0.3.0](https://github.com/dgrauet/mlx-forge/compare/v0.2.1...v0.3.0) (2026-05-27)


### ⚠ BREAKING CHANGES

* the convert/validate recipe names change from `vjepa2-vitl` / `vjepa2-vit-l-rope` to `vjepa-2.0-vitl` / `vjepa-2.1-vitl`.

### Documentation

* add docs/models/vjepa-2.md model guide ([#17](https://github.com/dgrauet/mlx-forge/issues/17)) ([e5a7bb3](https://github.com/dgrauet/mlx-forge/commit/e5a7bb31a8d0e81ffdbdfab43ddb79baf856bb3d))
* add the V-JEPA 2 recipes to the README ([#15](https://github.com/dgrauet/mlx-forge/issues/15)) ([f8cc8fc](https://github.com/dgrauet/mlx-forge/commit/f8cc8fcdbb90ee8213a8943938dde571833c7379))


### Code Refactoring

* rename V-JEPA 2 recipes to the versioned scheme ([#18](https://github.com/dgrauet/mlx-forge/issues/18)) ([2cd2bb5](https://github.com/dgrauet/mlx-forge/commit/2cd2bb50ddb11031173dfac5f74353c45f716b18))

## [0.2.1](https://github.com/dgrauet/mlx-forge/compare/v0.2.0...v0.2.1) (2026-05-27)


### Features

* **recipes:** add vjepa2-vit-l-rope conversion recipe ([#8](https://github.com/dgrauet/mlx-forge/issues/8)) ([5fdb51c](https://github.com/dgrauet/mlx-forge/commit/5fdb51c4b5df24b6853e501e9882e3348336e6a1))
* **recipes:** add vjepa2-vitl (V-JEPA 2.0 ViT-L + attentive probes) ([#9](https://github.com/dgrauet/mlx-forge/issues/9)) ([be2b5de](https://github.com/dgrauet/mlx-forge/commit/be2b5de3d25fbdaddd1f1aa3e9bcd78713529167))


### Bug Fixes

* **recipes:** version the V-JEPA 2 default output dirs to match HF naming ([#12](https://github.com/dgrauet/mlx-forge/issues/12)) ([40d8130](https://github.com/dgrauet/mlx-forge/commit/40d81300e6c0628364c9bc1f5a9074def0074d9e))
* **upload:** keep dir-name -q{bits} in derive_repo_id when split omits it ([#11](https://github.com/dgrauet/mlx-forge/issues/11)) ([0afd51c](https://github.com/dgrauet/mlx-forge/commit/0afd51cce3c5c26e767a2c815621eedf3e3bec68))
* **upload:** strip existing -mlx suffix in derive_repo_id ([#10](https://github.com/dgrauet/mlx-forge/issues/10)) ([b15ef28](https://github.com/dgrauet/mlx-forge/commit/b15ef2826191d820964a84c0a4270d0fc3b1c085))

## [Unreleased]

## [0.2.0] - 2026-05-05

### Removed

- **Breaking:** `mistral-small-3.1` recipe and associated docs/tests
- **Breaking:** `qwen-image-2512` recipe and associated docs/tests

### Changed

- Refreshed `CLAUDE.md`: list current recipes, add Quick Start and Dev workflow sections

## [0.1.0] - 2026-05-05

### Added

- CLI with `convert`, `validate`, `split`, `quantize`, and `upload` subcommands
- Generic conversion framework (lazy loading, component-by-component processing, conv weight transposition, materialization-aware quantization)
- Recipes:
  - **LTX-2.3** — 22B video DiT (transformer + VAE + text encoders)
  - **Fish S2 Pro** — Dual-AR TTS + DAC codec
  - **Mistral Small 3.1** — 24B VLM (Pixtral vision + dense LLM)
  - **Qwen-Image** — text-to-image MMDiT (Flux-style)
- Delta workflow for adding transformer/LoRA variants to existing repos (`--skip-shared`, `--add-only`, `--card-only`)
- Validation framework (pass/fail/warn)
- HuggingFace Hub upload with auto-generated model cards

[0.2.0]: https://github.com/dgrauet/mlx-forge/releases/tag/v0.2.0
[0.1.0]: https://github.com/dgrauet/mlx-forge/releases/tag/v0.1.0
