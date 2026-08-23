# Derby design

Implement against this file, not folklore.

## Identity

- Product: **Derby**
- Repo: `computerpets-derby`
- Idea: Pet Racing Derby
- Genre: Arcade racing
- Engine: Unreal / WebGL fallback
- Surface: `UE editor / 8080`

## Loop

A starving Rui does not win. Derby reads overlay vitals at lock-in. NFT gear can change drag, not spawn a faster species.

## Play beats

- Lobby of 6. One pet each.
- Track biome per species week (forest, reef, pond).
- Stamina drain; mood = cornering.
- Photo finish is server-authoritative.

## Neighbors

- computerpets (vitals at lock-in)
- computerpets-visitation (lobby)
- computerpets-ledger (entry fee / purse)
- computerpets-steamgate

## Failure doctrine

Disconnect → ghost the last inputs 3s then DNF. Unreal too heavy → WebGL fallback track. Cheating stamina → reject lock-in snapshot.

## Hard rules

1. Minigames cannot mint or burn NFTs by themselves (Minter is the write path).
2. Stats come from lived overlay care + Dojo caps, not cash shop.
3. Species kits stay inside Lore. Illegal hybrids never spawn.
4. Fail soft: the desktop overlay process is not this process.
