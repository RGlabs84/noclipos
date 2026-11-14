# NoClipOS

**Built by a game dev. For gamers and game devs.**

NoClipOS is an Arch-based gaming OS from Raven Iron Games and RG://LABS: it boots like a console (Duka mode: gamescope with Steam Big Picture), works like a studio (KDE Plasma 6 with the island taskbar), and talks back (Duka, the voice-first assistant).

Website: https://noclip.rossgilsonlabs.dev

## Download

**[NoClipOS 0.1, M1 prototype](https://github.com/RGlabs84/noclipos/releases/tag/v0.1.0-m1)**: a 1.3 GB network installer.

It is a prototype: installed start to finish in virtual machines, not yet proven on real hardware. **The installer erases the whole disk you install to; NoClipOS does not dual boot.** The release notes list what you need, how to install and the known gaps.

## What is here

- **Releases → `v0.1.0-m1`**: the installer ISO, its checksum and signature.
- **Releases → `repo-x86_64`**: the signed pacman repository `[noclip]` (NoClipOS's own packages and the AUR packages it ships prebuilt). It is not a download: the installer and every installed system read it through pacman. A copy is served from `https://noclip-repo.rossgilsonlabs.dev/noclip/os/x86_64/`, which pacman uses when GitHub does not answer.

```ini
[noclip]
SigLevel = Required DatabaseRequired
Server = https://github.com/RGlabs84/noclipos/releases/download/repo-$arch
Server = https://noclip-repo.rossgilsonlabs.dev/noclip/os/$arch
```

Everything is signed with the NoClipOS signing key, fingerprint `A517 2474 B0AB 096C 18D9  62C2 9D76 BBB4 3CCB B5B6`.
