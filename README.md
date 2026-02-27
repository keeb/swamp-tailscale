# @keeb/tailscale

[Swamp](https://github.com/systeminit/swamp) extension for Tailscale installation and tailnet machine inventory.

## Models

### `tailscale/node`

Install and authenticate Tailscale on a remote host over SSH.

| Method | Description |
|--------|-------------|
| `install` | Install Tailscale, authenticate with an auth key, and enable the service |

### `tailscale/net`

Discover and sync machines from a Tailscale tailnet.

| Method | Description |
|--------|-------------|
| `sync` | Sync all machines from the tailnet into named resources |
| `discover` | Discover a specific machine by name |

## Workflows

| Workflow | Description |
|----------|-------------|
| `setup-tailscale` | Install Tailscale and authenticate on a running VM |

## Dependencies

- [@keeb/ssh](https://github.com/keeb/swamp-ssh) — SSH helpers (`lib/ssh.ts`)

## Install

```bash
swamp extension pull @keeb/tailscale
```

## License

MIT
