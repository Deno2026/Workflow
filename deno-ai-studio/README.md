# [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Workflow/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe)

## Direct download

- [Download Windows installer](https://raw.githubusercontent.com/Deno2026/Workflow/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe)

## Install Docker Desktop first

- [Download Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/)
- [Install WSL on Windows](https://learn.microsoft.com/en-us/windows/wsl/install)

## Why Docker is required

Deno AI Studio uses Docker to run AI models in an isolated environment.

This helps:

- keep your main Windows environment cleaner
- reduce dependency conflicts
- avoid breaking other AI tools already installed on your PC
- make uninstall and cleanup safer later

If you do not know Docker yet, you can think of it like this:

**It is a required helper program that lets Deno AI Studio run models in a separate and safer workspace instead of directly changing your main PC environment.**

## First launch checklist

1. Install Docker Desktop if it is not already installed.
2. Make sure WSL is available and Docker Desktop can start successfully.
3. Run the installer.
4. Open **Deno AI Studio** from the desktop or Start menu.
5. Install a supported model from the catalog.
6. Add an input file only when the selected model requires one.
7. Run the model and check the output folder from inside the app.
