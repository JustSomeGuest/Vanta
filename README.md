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

1. Download [Vanta.rbxmx](https://github.com/JustSomeGuest/Vanta/raw/Main/Vanta.rbxmx).
2. Drag **`Vanta.rbxmx`** into **Workspace** in Roblox Studio.
3. Drag **`Vanta`** from `Workspace` into `ServerScriptService`.
4. Configure the settings if needed.
5. Done.

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
