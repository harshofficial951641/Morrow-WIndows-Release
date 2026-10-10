# Morrow for Windows: releases

This repository only holds Morrow for Windows release files. No source code.

Each release `vX.Y.Z` carries:

- `Jarvis-X.Y.Z.exe`: the Morrow installer that Morrow downloads to update itself.
- `Jarvis-X.Y.Z.exe.sig`: its update signature. Morrow for Windows installs an
  update only if this signature matches the Windows update key built into it.

Morrow learns about a release from Morrow's own update service, which records the
file's SHA-256 and signature and only switches a release on after checking that
the file published here is byte-for-byte the one that was signed.
