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

## Do I need WSL too?

Yes. On Windows, Docker Desktop works best with the **WSL 2 backend**.

For most beginners, the easiest path is:

- install Docker Desktop first
- if Docker Desktop says WSL is missing, use the WSL link above
- restart Windows if needed
- then continue with Deno AI Studio

## Step-by-step setup

1. Click [Download Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/).
2. Run the Docker Desktop installer with the default settings.
3. If Docker Desktop or Windows tells you that WSL 2 is required, click the WSL link above and complete that setup.
4. Restart Windows if asked.
5. Open Docker Desktop once and wait until it is fully running.
6. Click [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Workflow/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.3.exe) to download the installer.
7. Run the installer and finish setup.
8. Open **Deno AI Studio** from the desktop or Start menu.
9. Choose your language from the top-left language menu.
10. Pick a model from the catalog and click **Start**.
11. Click **Install** the first time you use a model.
12. Add files only when a model requires them.
13. Run the model and open the output folder from inside the app.
