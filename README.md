# GTNH OmniOcular Configs

OmniOcular XML configs updated for GT New Horizons `2.9.0-beta-1`.

## Usage

Copy the XML files into the OmniOcular config directory, normally:

```text
config/OmniOcular/
```

OmniOcular loads every XML file from that directory, so filenames such as
`GregTech5U-GTNH.xml` are valid when installed manually.

## 2.9.0-beta-1 notes

- GregTech target version checked against `GT5-Unofficial 5.09.52.594`.
- Waila target version checked against `waila 1.19.30`.
- `GregTech5U-GTNH.xml` now handles the 2.9 maintenance NBT rename from
  `mSoftHammer` to `mSoftMallet`, while keeping fallback compatibility with
  older NBT.
- Long EU/t displays now fall back from the old `eLongEUPerTick` key to
  `mEUt` when the old key is absent.

Some machine-specific custom NBT fields are still runtime-only checks because
they depend on live machine state. Validate important machines in a 2.9.0-beta-1
client before treating every display line as fully tested.
