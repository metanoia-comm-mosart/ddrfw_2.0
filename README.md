# ddrfw

This directory contains LPDDR4 DDR PHY training firmware binary files
(`.bin`), organized by target platform and usage scenario.

## Directory Layout

- `evb/` — Evaluation Board (EVB) version

## Included Files

In the subdirectory contains the following firmware component:

- `mt2824_evb_lpddr4_3200.bin` - prebuilt DDR firmware for EVB board

## Usage Example

Select the appropriate directory according to the target platform:

```bash
TARGET=evb

cp ${TARGET}/mt2824_evb_lpddr4_3200.bin <your_fw_output_path>/
```

## Verification

After updating or replacing firmware files, the following command can be
used to verify file integrity and compare differences:

```bash
sha256sum evb/*
```

## Notes

- This repository currently contains binary firmware files only.
  Source code and build scripts are not included.
