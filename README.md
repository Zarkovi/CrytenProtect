# Cryten Protect — repository setup in progress

This public repository is currently a **README-only seed**. The Cryten Protect v0.0.4 source tree and a Windows executable have **not** been published here yet. Do not expect the source files or a release artifact to be available in this repository at this time.

The complete source package is prepared separately as `CrytenProtect-v0.0.4-source.zip`. To publish it, extract the archive on Windows, install Git for Windows, authenticate with write access to `Zarkovi/CrytenProtect`, and run the package's `PUSH_TO_GITHUB.bat`. That helper clones this repository first to preserve the existing README commit, copies the source while excluding common local caches and secrets, then asks before pushing.

Once the complete source has been pushed, the included GitHub Actions workflow can run on a Windows runner, execute the tests, build the application, and upload its package as an Actions artifact. No Windows build has run yet.

Cryten Protect is an early-development file-inspection tool, not a certified antivirus or replacement for Microsoft Defender. Review all findings before taking action on files.
