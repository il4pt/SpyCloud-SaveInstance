> [!IMPORTANT]
> Independent, unofficial project. Not affiliated with, endorsed by, or officially connected to Roblox Corporation. "Luau" is a trademark of Roblox Corporation.

# SpyCloud SaveInstance

Discord: <https://discord.gg/spycloud>

## Loadstring

```lua
local Params = {
	RepoURL = "https://raw.githubusercontent.com/il4pt/SpyCloud-SaveInstance/main/",
	SSI = "saveinstance",
}
local synsaveinstance = loadstring(game:HttpGet(Params.RepoURL .. Params.SSI .. ".luau", true), Params.SSI)()
local Options = {}
synsaveinstance(Options)
```

## Progress GUI

While saving, a progress card is shown at the top of the screen with the current stage, a progress bar and percentage:

| Stage | Range |
|---|---|
| Başlatılıyor / API dump yükleniyor | 0–10% |
| Instance'lar toplanıyor | 10–35% |
| Kaydediliyor (serialize + decompile) | 35–95% |
| Dosyaya yazılıyor | 95–100% |

Set `ShowStatus = false` in `Options` to hide it.

## Credits & License

This is a modified version of **UniversalSynSaveInstance https://discord.gg/wx4ThpAsmw** by the USSI contributors (<https://github.com/luau/UniversalSynSaveInstance>).

Changes in this fork: SpyCloud branding, progress GUI, removed notification icons and docs assets.

Licensed under the GNU AGPL-3.0, see [LICENSE](LICENSE). As required by Section 7 (b) of the original license, the credit string `UniversalSynSaveInstance https://discord.gg/wx4ThpAsmw` must be kept, and authorship of the original source code is not claimed.

The original project builds on the work of [@Anaminus] & [@Dekkonot] ([Roblox Format Specifications]), [Synapse X Source 2019], [@LorekeeperZinnia], [Rojo Rbx Dom Xml], [Roblox File Format] and [Roblox Client Tracker].

## Disclaimer

This project is provided for development, debugging, archival, and research purposes within the Roblox platform. It is not intended for misuse, including violating platform rules, unauthorized access, or redistribution of content without permission. Users are responsible for ensuring their usage complies with all applicable rules, including Roblox's Terms of Use.

[@Anaminus]: https://github.com/Anaminus
[@Dekkonot]: https://github.com/Dekkonot
[@LorekeeperZinnia]: https://github.com/LorekeeperZinnia
[Rojo Rbx Dom Xml]: https://github.com/rojo-rbx/rbx-dom/blob/master/docs/xml.md
[Roblox Client Tracker]: https://github.com/MaximumADHD/Roblox-Client-Tracker
[Roblox File Format]: https://github.com/MaximumADHD/Roblox-File-Format
[Roblox Format Specifications]: https://github.com/RobloxAPI/spec/
[Synapse X Source 2019]: https://github.com/Acrillis/SynapseX
