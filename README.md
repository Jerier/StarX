# StarX

A free all-in-one tool for gamers. Tune your screen colors on any GPU (plus NVIDIA vibrance), add a crosshair overlay, cap your volume, grab color-filtered screenshots, and set up game launch options. Everything gets put back when you turn it off or close the app.

StarX doesn't inject into games or touch game memory. It only changes settings, config files and your Windows display.

Works on Windows 10 and 11 (64-bit). NVIDIA vibrance only works on NVIDIA GPUs, everything else works on any GPU.

## Download

Grab **StarX-1.0.0-Setup.zip** from the [latest release](https://github.com/Jerier/StarX/releases/latest). That's the only file you need.

## Install

1. Download the zip and **extract it**
2. Double click `StarX-Setup.exe`
3. Follow the steps and you're done

## Windows says it's dangerous?

That's normal. StarX isn't code signed (a signing certificate costs money and this is a free app), so Windows and some antivirus programs get nervous about new unsigned apps. It's not a virus. It does change system settings, which is the whole point of it, and that can make scanners react too.

- **"Windows protected your PC"**: click **More info**, then **Run anyway**
- **Antivirus flags it**: it's most likely a false positive. You can check your download is the real one (see below)

## Get your key

StarX asks for a key the first time you open it. Join the Discord and grab it there: https://discord.gg/3zGB8NUHU3

Please don't post the key around.

## Check your download (optional)

Every release has a `SHA256SUMS.txt` next to the zip. Open PowerShell where you downloaded the zip and run:

```
Get-FileHash .\StarX-1.0.0-Setup.zip -Algorithm SHA256
```

If it doesn't match the one on the release page, don't run it. Only download StarX from this page or the Discord.

## Uninstall

Settings > Apps > StarX > Uninstall (or Start Menu > StarX > Uninstall StarX). It asks if you also want your settings deleted.

## Something broke?

- Open StarX, go to Settings > Tools > **Copy diagnostics** and paste it in the Discord. Your key and Windows name are removed from it.
- Colors stuck after a crash? Press Win+R and run `%LOCALAPPDATA%\Programs\StarX\StarX.exe --reset`.

## Other stuff

- [Terms of use](LICENSE) - free for personal use, not open source, please don't reupload it
- [Privacy](PRIVACY.txt) - the only thing StarX connects to is a tiny status file on GitHub
- [Changelog](CHANGELOG.md)