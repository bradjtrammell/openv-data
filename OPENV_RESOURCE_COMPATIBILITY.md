# OpenV — default resources compatibility baseline

Status: **inventory only; no resources modified or executed** · 2026-10-14

This fork contains `resources/[gamemodes]`, `[gameplay]`, `[local]`, `[managers]`, `[system]`, and `[test]`. Upstream README states this source has been finalized/archived and some defaults may be bundled in the FiveM runtime now.

## Policy

Preserve original resource manifests, native names, exports, event names, ACE semantics, convars, and community-facing configuration. Preserve per-resource licenses and attribution; this repo does **not** declare a single blanket license at root. Do not include proprietary assets or bypass escrow mechanisms.

## Required verification

1. Inventory resource-level licenses and compare this historical tree with resources bundled by current FXServer.
2. Test default server startup using unchanged resources and `server.cfg`.
3. Validate built-in resources and manifests under OpenV; log exact failures.
4. Verify Lua/JS/C# runtime, NUI, voice, streamed assets and txAdmin integrations against representative community resources.
5. Treat ESX/QBCore/Qbox, pma-voice, inventories, maps, vehicles, EUP and protected resources as **separate** representative compatibility suites, subject to owner rights.
6. Preserve player identifiers, permissions and database relationships; perform backup-and-restore rehearsals before migration.

## Exclusions

Do not import or relicense arbitrary third-party community resources. Do not rewrite resource interfaces merely to replace branding. No compatibility claims until end-to-end tests have run.
