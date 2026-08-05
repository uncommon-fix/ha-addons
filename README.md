# uncommon-fix — Home Assistant Add-ons

A Home Assistant add-on repository. Add this repo's URL to your Supervisor
to install the add-ons below. Each add-on lives in its own repository and
is included here as a git submodule pinned to a release tag.

> [!WARNING]
> These add-ons are early **public alphas** — expect breaking changes and
> the occasional need to reinstall. Please don't rely on them for anything
> critical yet. File issues in the individual add-on repositories.

## Install

1. In Home Assistant: **Settings → Add-ons → Add-on Store**.
2. Open the **⋮** menu (top-right) → **Repositories**.
3. Add this repository URL:
   ```
   https://github.com/uncommon-fix/ha-addons
   ```
4. Find the add-on you want in the store and click **Install**.

## Add-ons

| Add-on | Description | Source |
| --- | --- | --- |
| **Traefik** | LAN reverse-proxy with a built-in UI for routes/middlewares, Cloudflare DNS-01 TLS, and per-route reachability sensors. | [`ha-addon-traefik`](https://github.com/uncommon-fix/ha-addon-traefik) |
| **UniFi Network Application** | Self-hosted UniFi controller with MongoDB bundled in the same container. Adopt and manage UniFi access points, switches and gateways without a Cloud Key or a UDM. No configuration: the database is internal and the whole controller is set up in UniFi's own web UI. Runs on the host network so device discovery works. **Requires a Raspberry Pi 5 or newer on ARM** — MongoDB 8 needs ARMv8.2-A. | [`ha-addon-unifi-controller`](https://github.com/uncommon-fix/ha-addon-unifi-controller) |
| **DaVinci Resolve Postgres** | Self-hosted PostgreSQL 17 for DaVinci Resolve Studio project databases. Per-library web UI creates a fresh DB + user + random password, ready to paste into DaVinci's *Connect to PostgreSQL* dialog. HA's full backup covers `/data/pgdata` cleanly via `backup: cold`. DaVinci Resolve 18 and 19 supported. | [`ha-addon-davinci-resolve`](https://github.com/uncommon-fix/ha-addon-davinci-resolve) |

## Architectures

`aarch64` (Raspberry Pi / ARM64) and `amd64` (x86-64). Prebuilt images are
published to GitHub Container Registry per addon (`ghcr.io/uncommon-fix/<image>`).

## License

[MIT](LICENSE).
