# EvaSenDesign Microstock Manager — Cloud Build

This package is designed so you do NOT need Rust, Node.js, or Visual Studio installed locally.

## Exact workflow
1. Create a GitHub account/repository.
2. Create a new repository, e.g. `evasendesign-microstock-manager`.
3. Upload ALL files and folders from this package to the repository root.
4. Commit to the `main` branch.
5. Open the repository's **Actions** tab.
6. Open **Build Windows Installer**.
7. Click **Run workflow**.
8. Wait for the green check.
9. Open the workflow run and download the artifact named:
   `EvaSenDesign-Microstock-Manager-Windows`
10. Inside it are the `.exe` and `.msi` installers.

The included workflow builds on a hosted Windows runner, so the user's own PC does not need the Rust/Node/Visual Studio toolchain.

Important: this starter contains the desktop shell and modular agency UI. Actual agency submission connectors must be implemented using each platform's permitted API/FTP/official mechanism. It intentionally does not bypass CAPTCHA, authentication, rate limits, or other platform controls.
