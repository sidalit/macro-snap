<div align="center">

<img src="snap/gui/macro.png" alt="Macro logo" width="128" />

# Macro

**A workspace for documents, messages, tasks and AI agents**

[![macro](https://snapcraft.io/macro/badge.svg)](https://snapcraft.io/macro)
[![Base: core26](https://img.shields.io/badge/Base-core26-2C8C3C?logo=canonical&logoColor=white)](https://snapcraft.io/core26)
![Confinement: strict](https://img.shields.io/badge/Confinement-strict-2C8C3C)
[![Maintainer: sidaliteir](https://img.shields.io/badge/Maintainer-sidaliteir-2C8C3C?logo=snapcraft&logoColor=white)](https://snapcraft.io/publisher/sidaliteir)
![Architecture: amd64](https://img.shields.io/badge/Architecture-amd64-2C8C3C?logo=linux&logoColor=white)

[Getting Started](#getting-started) · [Configure](#configure) · [Limitations](#limitations) · [Build](#build) · [Support](#support) · [License](#license)

Unofficial snap packaging for [Macro](https://github.com/macro-inc/macro), a desktop workspace connected to Macro's hosted services.

</div>

---

## Getting Started

<a href="https://snapcraft.io/macro"><img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" width="180"></a>

```bash
sudo snap install macro
macro
```

You can also launch Macro from the application menu. Sign in through your browser and allow it to reopen Macro.

## Configure

Use the application's settings. There are no `snap set` options.

```bash
sudo snap connect macro:audio-record       # microphone for calls
sudo snap connect macro:camera             # camera for calls
sudo snap connect macro:removable-media    # optional: /media, /mnt
```

## Limitations

- Local coding-agent integration (`macrod`) is unavailable. Cloud and remote agents remain supported.
- Files must be in accessible home directories or connected removable storage. Hidden host configuration is not shared.
- Bluetooth-based WhatsApp pairing is unavailable. Application updates are managed by snapd.

## Build

```bash
git clone https://github.com/sidalit/macro-snap.git
cd macro-snap
sudo snap install snapcraft --classic
snapcraft pack
```

## Support

- **Installation or snap issues:** [open a packaging issue](https://github.com/sidalit/macro-snap/issues).
- **Application bugs:** [report them upstream](https://github.com/macro-inc/macro/issues).

## License

Snap packaging: [MIT](https://github.com/sidalit/macro-snap/blob/main/LICENSE).
