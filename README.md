# uncommon-fix — Home Assistant Add-ons

A Home Assistant add-on repository. Add this repo's URL to your Supervisor to
install the add-ons below. Each add-on lives in its own repository and is
included here as a submodule.

> [!WARNING]
> These add-ons are early **public alphas** — expect breaking changes and the
> occasional need to reinstall. Please don't rely on them for anything critical
> yet. File issues in the individual add-on repositories.

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
| **Traefik** | Traefik reverse-proxy for your LAN with a built-in UI, Cloudflare DNS-01 TLS, and per-route reachability sensors. | [`ha-addon-traefik`](https://github.com/uncommon-fix/ha-addon-traefik) |

## Architectures

`aarch64` (Raspberry Pi / ARM64) and `amd64` (x86-64). Prebuilt images are
published to GitHub Container Registry.

## License

[MIT](LICENSE).
