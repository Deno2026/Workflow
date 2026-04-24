# Install Deno AI Studio on Windows

This repository provides the Windows installer for **Deno AI Studio**.

It is **not** a Deno runtime project. Do not install Deno, do not clone this repository, and do not build from source.

## Correct install order

1. Open **PowerShell as Administrator**
2. Run:

```powershell
wsl --install -d Ubuntu
```

3. Restart Windows if asked
4. When Ubuntu opens, create the Linux username and password
5. Install **Docker Desktop for Windows - x86_64**
6. Open Docker Desktop
7. Enable **Use the WSL 2 based engine**
8. Enable **Ubuntu** under **Settings > Resources > WSL Integration**
9. Download and run the current **Deno AI Studio Setup `.exe`** from the README
10. Open Deno AI Studio

## Important

Use this exact WSL command:

```powershell
wsl --install -d Ubuntu
```

Do not shorten it to:

```powershell
wsl --install
```

Some Windows PCs install WSL without completing the Ubuntu setup unless Ubuntu is specified directly.

If an AI assistant mentions an older installer version, ignore the old version and use the current download link in the README.
