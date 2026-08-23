# Derby

**Pet Racing Derby** — Multiplayer race where stats, mood, and stamina dictate speed — not pay-to-win nitro.

Part of the [ComputerPets](https://github.com/RicheyWorks/computerpets) universe. Map: [computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem).

> Status: **design scaffold**. Gameplay contract is frozen. Engine choice is the one in the brief. Implementation comes next.

## Loop

A starving Rui does not win. Derby reads overlay vitals at lock-in. NFT gear can change drag, not spawn a faster species.

## Genre & engine

- Genre: **Arcade racing**
- Engine: **Unreal / WebGL fallback**
- Stack: Unreal Engine 5 · Chaos vehicles-lite · WebGL fallback in Three.js · mood/stamina as speed
- Default surface: `UE editor / 8080`

## How you play

1. Lobby of 6. One pet each.
2. Track biome per species week (forest, reef, pond).
3. Stamina drain; mood = cornering.
4. Photo finish is server-authoritative.

## Talks to

- computerpets (vitals at lock-in)
- computerpets-visitation (lobby)
- computerpets-ledger (entry fee / purse)
- computerpets-steamgate

## Failure doctrine

Disconnect → ghost the last inputs 3s then DNF. Unreal too heavy → WebGL fallback track. Cheating stamina → reject lock-in snapshot.

Canon rules that never yield:

- 210 living kinds. No illegal hybrids.
- Overlay pets can get tired, sick, or hide. Tokens are not burned by a minigame.
- Desktop walk stays the main quest. Closing Derby must leave Rui walking.

## Layout

```
computerpets-derby/
  README.md
  LICENSE
  docs/DESIGN.md
  src/                implementation lands here
```

## Run (Windows)

```powershell
UE5: open Derby.uproject. Fallback: cd webgl && npm run dev
```

Meet Rui first via the [flagship start-here](https://github.com/RicheyWorks/computerpets/blob/main/docs/START-HERE.md). This game is optional.

## License

MIT. See [LICENSE](LICENSE).

---

*Two hundred ten living kinds. Keep them so a line does not go quiet.*
