```
██╗   ██╗ █████╗ ███╗   ██╗████████╗ █████╗
██║   ██║██╔══██╗████╗  ██║╚══██╔══╝██╔══██╗
██║   ██║███████║██╔██╗ ██║   ██║   ███████║
╚██╗ ██╔╝██╔══██║██║╚██╗██║   ██║   ██╔══██║
 ╚████╔╝ ██║  ██║██║ ╚████║   ██║   ██║  ██║
  ╚═══╝  ╚═╝  ╚═╝╚═╝  ╚═══╝   ╚═╝   ╚═╝  ╚═╝
```

---

**Security, for free.**

Vanta is a free, server-side Roblox anticheat.

## Features

- AntiBackdoor
- AntiDeletion
- AntiSpeed
- AntiTeleport
- AntiNoclip
- AntiFly
- AntiFling
- Whitelist API
- Automatic version checking

## Installation

1. Put `Vanta` in `ServerScriptService`.
2. Configure the settings if needed.
3. Done.

## Whitelist

```lua
local Vanta = require(script.Parent.Vanta)

Vanta.Whitelist(Player, 2)

Character:PivotTo(Destination)
````

Whitelist specific modules:

```lua
Vanta.Whitelist(Player, 2, {
    "AntiTeleport",
    "AntiNoclip",
})

Character:PivotTo(Destination)
```

Supported modules:

* `AntiFly`
* `AntiNoclip`
* `AntiSpeed`
* `AntiTeleport`

## Version

Newest Version: <!-- VERSION -->v1.0.0<!-- VERSION -->

## Creator

*JustSomeGuest*
