# [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Workflow/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe)

This repository hosts the public Windows installer and update manifest for **Deno AI Studio**.

## Direct download

- [Download Windows installer](https://raw.githubusercontent.com/Deno2026/Workflow/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe)

## What it is

Deno AI Studio is a Windows desktop launcher for open-source AI workflows.  
It is designed to make model installation, execution, input-file handling, and cleanup easier without relying on a terminal-first flow.

## Before you install

### Docker Desktop (required)

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

## Current included model support

- Qwen3-TTS 0.6B
- Qwen3-TTS 1.7B

## Notes

- Docker Desktop and WSL are required.
- Some models may require Hugging Face access approval or login.
- The app checks this repository for future installer updates.
