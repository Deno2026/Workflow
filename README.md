# [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Workflow/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe)

This repository hosts the public Windows installer and update manifest for **Deno AI Studio**.

## Direct download

- [Download Windows installer](https://raw.githubusercontent.com/Deno2026/Workflow/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe)

## What it is

Deno AI Studio is a Windows desktop launcher for open-source AI workflows.  
It is designed to make model installation, execution, input-file handling, and cleanup easier without relying on a terminal-first flow.

## Before you install

### Required helper apps

- [Download Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/)
- [Install WSL on Windows](https://learn.microsoft.com/en-us/windows/wsl/install)

### Why this is needed

Deno AI Studio runs AI models inside an isolated container environment.

That means:

- it helps keep your main Windows environment cleaner
- it avoids many dependency conflicts between AI projects
- it reduces the chance of breaking your existing PC setup
- it makes install, update, and cleanup much safer

If you are new to Docker, the easiest way to think about it is:

**Docker Desktop is a required helper app that lets Deno AI Studio run models safely in a separate workspace without directly mixing everything into your main PC environment.**

### Do I need WSL too?

Yes, Deno AI Studio uses Docker Desktop on Windows, and Docker Desktop works best with the **WSL 2 backend**.

The good news is:

- most beginners can start with **Docker Desktop first**
- if WSL is missing, Docker Desktop or Windows usually tells you what to do next
- if that happens, just use the WSL link above, finish that step, and continue

## Step-by-step for first-time users

1. Click [Download Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/).
2. Run the Docker Desktop installer and keep the default settings.
3. If Docker Desktop or Windows says WSL 2 is required, click the WSL link above and complete that setup first.
4. Restart Windows if Docker Desktop or WSL asks you to restart.
5. Open Docker Desktop once and wait until it finishes loading normally.
6. Click [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Workflow/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe) to download the installer.
7. Run `Deno AI Studio Setup 0.1.3.exe`.
8. Finish the installer.
9. Open **Deno AI Studio** from the desktop or Start menu.
10. Choose your language from the top-left language menu.
11. Pick a model from the catalog and click **Start**.
12. If this is your first time with that model, click **Install** and wait for the setup to finish.
13. Add input files only if the selected model requires them.
14. Run the model and open the output folder from inside the app.

## Current included model support

- Qwen3-TTS 0.6B
- Qwen3-TTS 1.7B

## Notes

- Docker Desktop and WSL are required.
- Some models may require Hugging Face access approval or login.
- The app checks this repository for future installer updates.
