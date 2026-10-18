# DLSS-NR runtime mirrors

This repository publishes two user-supplied `nvngx_dlssnr.dll` 310.9.16 variants for HoYoShade Hub:

- `SF` is the general compatibility build. Use it on RTX 40/50 and as the fallback for unknown NVIDIA GPUs.
- `F5` is specialized for RTX 20/30 acceleration.

The release assets are ZIP files containing one normalized file named `nvngx_dlssnr.dll`. The launcher selects the F5 asset for Turing/Ampere and the SF asset for Ada/Blackwell.

These binaries are redistributed as supplied by the user. The launcher verifies each ZIP SHA256 before installation and identifies these two DLL variants by exact DLL SHA256 fingerprints; both share PE version 310.9.16.0.
