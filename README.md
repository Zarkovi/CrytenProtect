# Cryten Protect

Cryten Protect is an early-development Windows desktop tool for local file inspection, scan history, optional AES-GCM encrypted quarantine, and opt-in AI reports.

> This is not a certified antivirus and does not replace Microsoft Defender or another trusted security product. A finding is a reason to investigate, not proof that a file is malicious.

## Source and Windows builds

The source uses Python and PySide6. Run setup_and_run.bat on 64-bit Windows to install runtime dependencies and launch the app. Run BUILD_EXE.bat to run tests and package the application. Keep the entire onedir distribution together, because the executable may load adjacent runtime files.

A Windows GitHub Actions workflow is included at .github/workflows/build-windows.yml. It runs the packaging checks on a Windows runner and uploads the generated package as a workflow artifact. No prebuilt or signed executable is included in this repository.

## Privacy and quarantine

AI reporting stays disabled until an OpenRouter API key is configured and reporting is explicitly enabled. The app sends scan metadata to the selected provider, not scanned file contents or absolute file paths. Review the data and the provider's terms before enabling it.

Quarantined files require the correct encryption key to restore. Keep a backup of that key and review all findings before isolating or deleting files.

See SECURITY.md for security reporting guidance and LICENSE for licensing.
