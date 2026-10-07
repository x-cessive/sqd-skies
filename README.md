# SQD Skies

The player download home for **SQD Skies**, a Minecraft Java modpack with Create, airships, Big Cannons, TaCZ and proximity voice chat.

**[Downloads and release history](https://github.com/x-cessive/sqd-skies/releases)** · **[pack-v2](https://github.com/x-cessive/sqd-skies/releases/tag/pack-v2)**

## Current client: pack-v2

Minecraft **1.21.1** · **NeoForge 21.1.252** · **Java 21** · about **8 GB** allocated RAM.

Early access: the release ZIP matches the documented deployed pack-v2. A fresh launcher import and live join with these instructions have not yet been independently verified. Reported installation problems and recovery steps are below.

### Install with the CurseForge app

1. [Download SQD-Skies-pack-v2.zip](https://github.com/x-cessive/sqd-skies/releases/download/pack-v2/SQD-Skies-pack-v2.zip).
2. In the app's Minecraft section, choose **Import / Import Profile .zip** and select the ZIP.
3. Wait for **every** dependency to download. A failed download means the installation is incomplete.
4. Launch the new profile and join **play.sovranos.com**. Ask staff to whitelist your exact Minecraft Java name first.

You can import this ZIP while the CurseForge project is under review; searching Browse Modpacks is not required. Do not download GitHub's automatic **Source code** archive as your client pack.

[CurseForge project](https://www.curseforge.com/minecraft/modpacks/sqd-skies) — reported as awaiting approval as of October 7, 2026. Its preview page is not a player installation route.

### Install with Prism Launcher

**Add Instance → Import → select the release ZIP.** Use Java 21 and about 8 GB RAM. Complete all download prompts, including any browser/manual downloads.

The ZIP contains a pinned manifest and configuration. It does **not** contain every mod JAR, so importing it is not proof that every dependency downloaded.

### Missing TaCZ / Ritchie's Projectile Library?

Both mods are already required by pack-v2. If joining reports missing channels from them, close Minecraft and download the exact files below into the new profile's **mods** folder:

| Required mod | Exact file | Author download page |
|---|---|---|
| TaCZ NeoForge port 1.1.8-hotfix-r7 | `tacz-neoforge-1.21.1-1.1.8-hotfix-r7.jar` | [Download](https://www.curseforge.com/minecraft/mc-mods/tacz-1-21-1/files/9027337) |
| Ritchie's Projectile Library 2.1.2 | `ritchiesprojectilelib-2.1.2-mc.1.21.1-neoforge.jar` | [Download](https://www.curseforge.com/minecraft/mc-mods/ritchies-projectile-library/files/7587771) |

In Prism: right-click the instance → **Folder → minecraft → mods**. In CurseForge: open the profile folder → **mods**. Download the normal JAR, not a sources JAR, and keep only one version of each mod.

These repairs cover the reported errors; other failed downloads still need completing. pack-v2 also requires **aeroclaims 0.9.4** and **Walkie-Talkie Plus 1.4.0**. The full pinned list is attached as `manifest.json` on the release.

Open Parties and Claims is optional on clients and does not replace aeroclaims. Do not install the server-only SQD Radio mod or Create: Extended Factory.

## Updating

Each client update gets a numbered **pack-vN** release with its ZIP, manifest, installation guide, changes and SHA-256 checksums. Install updates as **new profiles** so obsolete mods cannot remain in the folder. Keep your old profile until the new one successfully joins. Preserve personal saves and screenshots separately; avoid overwriting release configs with old configs.

Use the pack version staff identify as supported by the running server. Server-only radio and datapack updates do not require a client reinstall. Previous releases remain available for history and rollback.

## Help

Open an issue with your launcher, pack version, exact error and relevant log excerpt. Remove account tokens and personal information before posting logs publicly.

[CurseForge ZIP import documentation](https://support.curseforge.com/support/solutions/articles/9000197912) · [Release process](RELEASING.md)
