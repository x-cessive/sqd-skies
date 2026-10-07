# Publishing SQD Skies client releases

## Versioning

- Use the next `pack-vN` for changes to client mods or distributed configuration. Keep this version identical in the manifest, GitHub release and CurseForge upload.
- Do not silently replace an existing release ZIP. Correct documentation separately; changed client bytes require a new pack version.
- Server-only datapack/radio changes do not require client releases.
- Keep old releases for rollback; identify which pack the running server supports in README.

## Release assets

Attach `SQD-Skies-pack-vN.zip`, `INSTALL.md`, `manifest.json`, `RELEASE_NOTES.md` and `SHA256SUMS.txt`. Release notes identify Minecraft/NeoForge versions, additions/removals, known installation issues and testing evidence. The ZIP is a CurseForge manifest export, not a full mod-binary bundle. Refer downloads to the authors' pinned file pages; evaluate redistribution permissions before introducing bundled third-party binaries.

## Prepare and verify

1. Build from the pinned pack source and confirm every required project/file ID. Classify client-required, client-only, optional and server-only dependencies.
2. Confirm the ZIP contains no account credentials, personal saves, logs or server runtime data. Generate checksums for all attached assets except the checksum file itself.
3. Create a draft release against a commit in this repository. Use the numbered pack tag; do not copy a private server repository's commit SHA as its target.
4. Import into fresh CurseForge and Prism profiles without copying an existing mods folder. Complete all required downloads, record any manual-download prompts, launch and join the matching server. Test voice and changed client features. Record date, launcher/version and result.
5. Coordinate any server update through the server's existing backup/checkpoint procedure. Publish a tested release when the matching server is ready.
6. If sharing before clean-install verification, explicitly publish as an **early-access prerelease**, state what is unverified and include recovery instructions. Do not call it tested or promote it to stable Latest.
7. Update README's supported version and pinned download link. Upload the same manifest ZIP to CurseForge; link its exact approved file when available.

The Releases page is the stable player bookmark. For prereleases use the explicit `releases/tag/pack-vN` link; do not rely on `/releases/latest`.

## pack-v2 verification record — October 7, 2026

- OBSERVED: 74 manifest entries; TaCZ, Ritchie's Projectile Library, aeroclaims and Walkie-Talkie Plus are pinned and required.
- OBSERVED: release ZIP SHA-256 matches the existing deployed-pack hash recorded in the source pack changelog: `5212d485ed561e6e58760b58d5570aaee7a7b28ce602cc3ec600a9b78f8bd491`.
- USER_REPORTED: clients have missing mods; CurseForge review is pending.
- UNKNOWN: clean CurseForge install, clean Prism install and successful live join for these instructions. Publish as early access until verified.
