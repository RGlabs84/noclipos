# NoClipOS

**Built by a game dev. For gamers and game devs.**

NoClipOS is an Arch-based gaming OS from Raven Iron Games and RG://LABS: it boots like a console (Duka mode: gamescope with Steam Big Picture), works like a studio (KDE Plasma 6 with the island taskbar), and talks back (Duka, the voice-first assistant).

Website: https://noclip.rossgilsonlabs.dev

## What is here

- **Releases → `repo-x86_64`**: the signed pacman repository `[noclip]` (NoClipOS's own packages and the AUR packages it ships prebuilt). It is not a download: NoClipOS's installer and every installed system read it through pacman. A copy is served from `https://noclip-repo.rossgilsonlabs.dev/noclip/os/x86_64/`, which pacman uses when GitHub does not answer.
  Signing key: `A5172474B0AB096C18D962C29D76BBB43CCBB5B6` (NoClipOS Repo Signing Key).
- **ISO releases** will appear here when NoClipOS goes public. It is an M1 prototype today.

```ini
[noclip]
SigLevel = Required DatabaseRequired
Server = https://github.com/RGlabs84/noclipos/releases/download/repo-$arch
Server = https://noclip-repo.rossgilsonlabs.dev/noclip/os/$arch
```
