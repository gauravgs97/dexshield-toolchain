# 🛡️ DexShield Toolchain

Self-contained Clang/LLVM 21 toolchain for **on-device Android native compilation**, used by the DexShield DEX-to-C++ protection app.

No Termux installation required — extracted from Termux packages with fixed portable RPATH.

## Downloads

See **[Releases](../../releases)** for the latest toolchain archive.

## Features

- Clang 21.1.8 (NDK r29 based)
- lld linker + llvm-ar / llvm-strip / llvm-nm
- Targets:
  - ✅ `aarch64-linux-android` (arm64-v8a)
  - ✅ `armv7a-linux-androideabi` (armeabi-v7a)
- libc++, libunwind, compiler-rt builtins
- Fixed relative RPATH (`$ORIGIN/../lib`) — runs standalone
- Android NDK headers + multi-arch sysroot
- Binaries stripped (smaller size)

## Version

- v2.0 — multi-arch (arm64 + armv7), fixed RPATH, stripped binaries