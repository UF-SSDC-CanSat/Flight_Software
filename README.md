# Flight_Software
CanSat 2027 flight software, container + PocketQube ;-;

Two build targets: `container` and `pocketqube`.

- Mission: PocketQube deployment. Container releases a 2P satellite at 90% of peak altitude.
- Radio: ESPNOW (required by X1). XBee optional backup.
- Telemetry: 4 Hz both vehicles.
- Launch: 12 June 2027

## Repo layout
- `lib/core/` — telemetry, commands, persistence, flight state machine
- `lib/drivers/` — sensor drivers (HAL + stdint only, nothing else)
- `lib/gnc/` — attitude estimation and camera pointing control
- `ground/` — ground station and simulator
- `test/` — host-side unit tests, fixtures include the 2026 flight logs
- `docs/adr/` — architecture decision records
