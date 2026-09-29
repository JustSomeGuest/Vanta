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

## Version

Newest Version: <!-- VERSION -->v1.0.1<!-- VERSION -->

## Features

- **AntiBackdoor** - Uses a honeypot `RemoteEvent` to detect backdoor scanners probing your game for exploitable remotes.
- **AntiDeletion** - Protects `LocalScripts`, `ModuleScripts`, `RemoteEvents`, and Vanta's notification UI from being deleted.
- **AntiSpeed** - Detects players moving faster than the speeds allowed in the Vanta settings and corrects abnormal movement.
- **AntiTeleport** - Detects abnormal position changes that exceed the configured teleport distance. Violations are tracked using strikes and cooldowns to reduce false detections.
- **AntiNoclip** - Detects players moving through solid objects. Violations are tracked using strikes and cooldowns.
- **AntiFly** - Detects abnormal airborne movement that may indicate flying. Players are checked against the configured maximum air time before receiving strikes.
- **AntiFling** - Prevents exploiters from flinging players by disabling character collisions. Players remain fully collidable with the game environment, so this does not enable noclip.
- **Whitelist API** - Temporarily prevents Vanta's movement checks from flagging players during legitimate game mechanics such as teleporters, portals, launchers, or cutscenes. Supports `AntiFly`, `AntiNoclip`, `AntiSpeed`, and `AntiTeleport`.
- **Automatic Version Checking** - Checks the latest version listed in Vanta's GitHub `Version.txt` and warns in the server output when the installed version is outdated.

## Installation

1. Download [Vanta.rbxmx](Vanta.rbxmx).
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

## Creator

*JustSomeGuest*
