# Beside for Windows — Changelog

## [0.3.0] — 2026-11-12
### Added & Improved
- Independent platform release tagged as `windows-v0.3.0` (build 13).
- **Zero-Lag Control Framing**: Enabled `TCP_NODELAY` across all sockets, avoiding 40–200 ms Nagle delays on file transfer control packets and yielding up to 2.63x faster inbound transfers.
- **Win32 Atomic File Finalization**: Implemented atomic non-overwriting file finalization using Win32 `MoveFileExW(..., 0)` to guarantee safe placement without data loss.
- **Physical Wi-Fi Verification**: Validated over 60 physical runs on 2.4 GHz Wi-Fi between Windows 11 PC and Android 13 smartphone.
- 100% SHA-256 integrity verification across all transferred files.
- Inno Setup Windows installer (`Beside-Setup-v0.3.0-x64.exe`) and portable archive (`Beside-v0.3.0-Windows-x64.zip`).

## [0.2.0] — 2026-11-01
### Added & Improved
- Independent platform release cycle (tagged as `windows-v0.2.0`).
- Cryptographic Ed25519 release feed signature verification.
- Windows Defender SmartScreen guidance and reputation verification.
- File Explorer context menu and WinRT toast notification resilience.
- Bounded 64 KB streaming over Mutual TLS 1.3.
