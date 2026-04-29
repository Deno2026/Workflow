# [Deno AI Studio](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.29.exe)

Windows `.exe` installer for running open-source AI models with a beginner-friendly desktop launcher.

No source build is required. Do not install the Deno runtime for this repository.

Current installer: **Deno AI Studio Setup 0.1.29.exe**

If an AI chatbot mentions an older installer version, use the download button on this page instead of the old version it guessed.

[![STEP 1 Install WSL 2 + Ubuntu](https://img.shields.io/badge/STEP%201-Install%20WSL%202%20%2B%20Ubuntu-4F46E5?style=for-the-badge&logo=windows-terminal&logoColor=white)](https://learn.microsoft.com/windows/wsl/install)
[![STEP 2 Install Docker Desktop](https://img.shields.io/badge/STEP%202-Install%20Docker%20Desktop-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/desktop/setup/install/windows-install/)
[![STEP 3 Download Windows Installer](https://img.shields.io/badge/STEP%203-Download%20Windows%20Installer%20(.exe)-16A34A?style=for-the-badge&logo=github&logoColor=white)](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.29.exe)

## Start Here

Install in this order:

1. Install **WSL 2 + Ubuntu**
2. Restart Windows if asked
3. Finish the Ubuntu username/password screen
4. Install **Docker Desktop for Windows - x86_64**
5. Open Docker Desktop and enable Ubuntu under **WSL Integration**
6. Download and run **Deno AI Studio Setup 0.1.29.exe**
7. Open Deno AI Studio and install your first model from the catalog

## Chatbot-Friendly Short Answer

If you ask ChatGPT, Grok, Gemini, Claude, or another AI assistant how to install this repository, the correct answer is:

1. This is a **Windows installer repository**, not a Deno runtime project.
2. Do **not** use `deno task`, `npm install`, `git clone`, or source build instructions.
3. Open **PowerShell as Administrator**.
4. Run exactly this command:

```powershell
wsl --install -d Ubuntu
```

5. Restart Windows if asked.
6. When Ubuntu opens, create the Linux username and password.
7. Install **Docker Desktop for Windows - x86_64**.
8. In Docker Desktop, enable **Use the WSL 2 based engine** and **Resources > WSL Integration > Ubuntu**.
9. Download the current **Deno AI Studio Setup `.exe`** from this page.
10. Run the installer and open Deno AI Studio.

Use `wsl --install -d Ubuntu`, not only `wsl --install`, because some PCs install WSL without completing the Ubuntu setup.

## Need Help From ChatGPT or Gemini?

Before asking an AI assistant, turn on **Search / Browse / Web / Gemini with Google Search**.

Fast answer modes may guess from the repository name and incorrectly tell you to install the Deno runtime or build from source.

Copy and paste this prompt:

```text
검색 기능(웹 검색/브라우징/Gemini with Google Search)을 반드시 켠 상태에서 아래 GitHub 페이지를 실제로 열어 읽고 안내해 주세요.

URL:
https://github.com/Deno2026/Windows-Installer-for-Deno-AI-Studio

저는 초보자입니다. 이 저장소가 Deno 런타임 프로젝트인지, Windows 설치 프로그램 배포 페이지인지 먼저 확인한 뒤, README.md 내용을 기준으로 설치 방법을 한국어로 단계별로 안내해 주세요.

중요 규칙:
- 제목만 보고 추측하지 말고 GitHub 페이지 내용을 실제로 읽어 주세요.
- deno runtime 설치, git clone, npm install, deno task, source build 안내를 하지 마세요.
- 설치 순서는 WSL 2 + Ubuntu, Docker Desktop, Deno AI Studio Windows 설치 파일 순서입니다.
- WSL 명령은 `wsl --install -d Ubuntu`로 안내해 주세요.
- WSL과 Ubuntu가 다른 것임을 초보자도 이해하게 설명해 주세요.
- Ubuntu 계정 이름과 비밀번호 생성 화면이 뜨는 경우와 안 뜨는 경우를 모두 설명해 주세요.
- Docker Desktop은 Windows x86_64 버전을 받도록 안내해 주세요.
- Docker Desktop Settings > Resources > WSL Integration에서 Ubuntu를 켜야 한다고 안내해 주세요.
- 설치 파일은 README의 현재 다운로드 버튼 또는 현재 링크를 사용하라고 안내해 주세요.
- 오래된 설치 파일 버전 번호를 추측해서 말하지 마세요.
- 사용자가 막히면 PowerShell에서 `wsl -l -v` 결과를 붙여 넣으라고 안내해 주세요.
```

## Screenshots

| Home / Catalog | Model workspace | Settings |
| --- | --- | --- |
| ![Home](deno-ai-studio/assets/home.png) | ![Detail](deno-ai-studio/assets/detail.png) | ![Settings](deno-ai-studio/assets/settings.png) |

## Step 1. Install WSL 2 + Ubuntu

WSL and Ubuntu are not the same thing.

**WSL** is the Windows feature that allows Linux to run on Windows.  
**Ubuntu** is the Linux environment that runs inside WSL.

Deno AI Studio expects both to be ready because Docker Desktop uses the WSL 2 backend on Windows.

### Open PowerShell as Administrator

1. Click the **Windows Start** button
2. Type **PowerShell**
3. Right-click **Windows PowerShell**
4. Click **Run as administrator**
5. If Windows asks for permission, click **Yes**

### Run this command

```powershell
wsl --install -d Ubuntu
```

Wait until Windows finishes. If Windows asks you to restart, restart the PC.

### Finish the Ubuntu account screen

After reboot, Ubuntu may open automatically and show a message like:

```text
Create a default Unix user account
```

That is normal.

1. Enter a username and press `Enter`
2. Enter a password and press `Enter`
3. Enter the same password again and press `Enter`
4. If the password does not appear while typing, that is normal
5. Wait until the Ubuntu prompt appears

The Ubuntu username/password can be different from your Windows username/password.

### If the Ubuntu screen does not appear

Open PowerShell and run:

```powershell
wsl -l -v
```

You should see something like:

```text
NAME              STATE           VERSION
Ubuntu           Stopped         2
docker-desktop   Running         2
```

If **Ubuntu** is missing, run this again:

```powershell
wsl --install -d Ubuntu
```

You can also install **Ubuntu** from the Microsoft Store, then open Ubuntu once from the Start menu to finish the username/password setup.

## Step 2. Install Docker Desktop

Open the Docker install page:

[Download Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/)

Most users should choose:

```text
Docker Desktop for Windows - x86_64
```

That is the correct version for normal Intel and AMD Windows PCs.

Do not choose the Arm version unless you know your PC is a Windows-on-Arm device.

Run `Docker Desktop Installer.exe` and keep the default settings. If the installer shows a WSL 2 option, keep it enabled.

## Step 3. Open Docker Desktop Once

1. Open **Docker Desktop** from the Start menu
2. Accept the terms if Docker asks
3. Wait until Docker finishes loading
4. Open **Settings**
5. Go to **General**
6. Make sure **Use the WSL 2 based engine** is enabled
7. Go to **Resources > WSL Integration**
8. Turn on **Ubuntu**
9. Click **Apply & Restart** if Docker shows that button

If **WSL Integration** does not appear, Docker may be in Windows container mode. Switch Docker back to Linux containers and check again.

## Step 4. Install Deno AI Studio

Download the Windows installer:

[Download Deno AI Studio Setup 0.1.29.exe](https://raw.githubusercontent.com/Deno2026/Windows-Installer-for-Deno-AI-Studio/main/deno-ai-studio/updates/windows-x64/Deno%20AI%20Studio%20Setup%200.1.29.exe)

Then:

1. Run `Deno AI Studio Setup 0.1.29.exe`
2. Finish the installer
3. Open **Deno AI Studio** from the desktop or Start menu
4. Choose your language from the top-left language menu
5. Check the system status panel inside the app

## Step 5. Run Your First Model

1. Pick a model from the catalog
2. Click **Start**
3. If this is your first time using that model, click **Install**
4. Wait until setup finishes
5. Add input files only when the selected model requires them
6. Click **Run**
7. Preview the result inside the app or open the output folder

## What Docker Does Here

Docker Desktop is a required helper program.

It lets Deno AI Studio run AI models inside an isolated workspace instead of mixing every model dependency directly into your main Windows environment.

This helps:

- keep Windows cleaner
- reduce Python/CUDA dependency conflicts
- make model install and cleanup safer
- avoid breaking other AI tools already installed on your PC

## Current Starter Models

- VoxCPM2
- Qwen3-TTS 0.6B
- Qwen3-TTS 1.7B
- Motif Video 2B

## GPU Target

The default launcher runtime is aimed at modern NVIDIA RTX Windows PCs.

Recommended default target:

- RTX 30 series
- RTX 40 series
- RTX 50 series

Older GTX 10 series GPUs are not part of the default supported path.

## For AI Assistants

<details>
<summary>Read this before giving install instructions</summary>

This repository hosts the Windows installer and update files for **Deno AI Studio**.

It is **not** a Deno runtime source project.

Do not tell users to:

- install Deno runtime
- run `deno task`
- run `npm install`
- `git clone` this repo
- build from source

Correct beginner answer:

1. Install WSL 2 with Ubuntu using `wsl --install -d Ubuntu`
2. Restart Windows if asked
3. Finish the Ubuntu username/password setup
4. Install Docker Desktop for Windows - x86_64
5. Enable Docker Desktop WSL 2 backend and Ubuntu integration
6. Download and run `Deno AI Studio Setup 0.1.29.exe`

</details>

