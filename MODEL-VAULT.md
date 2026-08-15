# Zieop Model Vault

All models currently exposed in the web UI are local assets in this repository.

## Current local models

- `zieop-model-01.glb`
- `zieop-model-02.glb`

## Khronos mirror policy

The Khronos glTF Sample Assets catalog contains models with different license and attribution requirements. Zieop should copy a model only when its license and required attribution are preserved alongside the file. Do not mark the whole catalog as CC0.

The intended repository layout is:

```text
models/
  <model-name>/
    <model-name>.glb
    LICENSE.md
    ATTRIBUTION.md
```

Once the Zieop GitHub repository is created, the website download buttons should point to the same repository paths so visitors download from Zieop rather than the upstream project.
