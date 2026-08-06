<h3 align="center">
	<img src="https://avatars.githubusercontent.com/u/257101280?s=200&v=4" width="100" alt="Logo"/><br/>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
	Colony
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<h6 align="center">
  <a href="#-the-apps">Apps</a>
  ·
  <a href="#-philosophy">Philosophy</a>
  ·
  <a href="#-tech-stack">Tech Stack</a>
  ·
  <a href="#-theming">Theming</a>
  ·
  <a href="#-contributing">Contributing</a>
</h6>

<p align="center">
	<a href="https://github.com/Project-Colony"><img src="https://img.shields.io/badge/organization-Project--Colony-b4befe?style=for-the-badge&logo=github&logoColor=cdd6f4&labelColor=1e1e2e" alt="Organization"></a>
	<a href="https://github.com/Project-Colony/Colony"><img src="https://img.shields.io/badge/built%20with-Rust-fab387?style=for-the-badge&logo=rust&logoColor=cdd6f4&labelColor=1e1e2e" alt="Built with Rust"></a>
	<a href="https://github.com/Project-Colony/Colony/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-GPL--3.0--or--later-a6e3a1?style=for-the-badge&logoColor=cdd6f4&labelColor=1e1e2e" alt="License"></a>
</p>

&nbsp;

<p align="center">
Colony is an ecosystem of small, focused desktop utilities built with Rust.<br/>
Instead of one monolithic tool that does everything poorly, Colony offers a curated set of apps —<br/>
each designed to do one thing exceptionally well, with native performance and beautiful, themeable interfaces.
</p>

<p align="center">
The <a href="https://github.com/Project-Colony/Colony">Colony launcher</a> ties them together: it installs, updates and launches<br/>
every app in this organization, and lists the apps already on your system alongside them.
</p>

&nbsp;

<h3 align="center">🧩 The Apps</h3>

<div align="center">

| App | What it does | Platforms |
|:---|:---|:---:|
| **[Colony](https://github.com/Project-Colony/Colony)** | Launcher and app store for the whole ecosystem | Linux · Windows · macOS |
| **[Eidos](https://github.com/Project-Colony/Eidos)** | Mod manager for Bethesda games — merges mods into a FUSE union at launch, so the game directory is never touched | Linux |
| **[SphereCord](https://github.com/Project-Colony/SphereCord)** | Discord client with Equicord preinstalled and the Colony palettes bundled in | Linux · Windows |
| **[Spotter](https://github.com/Project-Colony/Spotter)** | Game library tracker — imports Steam, GOG, Epic, Xbox and PlayStation, follows playtime and achievements | Linux · Windows · macOS |
| **[Grape](https://github.com/Project-Colony/Grape)** | Music player for a local library, with tag and cover reading and a built-in equalizer | Linux · Windows · macOS |
| **[D1Gg2r](https://github.com/Project-Colony/D1Gg2r)** | System monitor — live CPU, memory, disk, network, temperature and GPU, with persistent history | Linux · Windows · macOS |
| **[orCAL](https://github.com/Project-Colony/orCAL)** | Desktop calculator, in a phone-shaped window or a tablet one with a scientific keypad | Linux · Windows · macOS |
| **[SAM · Colony Edition](https://github.com/Project-Colony/SAM-Colony-Edition)** | Steam achievement manager — browse, unlock and edit the stats of games you own | Linux · Windows · macOS |

</div>

&nbsp;

<h3 align="center">🧠 Philosophy</h3>

<p align="center">
<b>One app, one purpose</b> — each Colony tool solves a single problem with clarity and precision.<br/>
No feature bloat, no hidden complexity.
</p>

<p align="center">
<b>Native performance matters</b> — nearly everything is built in Rust.<br/>
Startup is instant, memory usage is minimal, and your CPU stays cool.
</p>

<p align="center">
<b>Beauty is not optional</b> — the apps share one theming system<br/>
and adapt to your system's dark mode.<br/>
Tools should look as good as they work.
</p>

<p align="center">
<b>Cross-platform by default</b> — most apps target Linux, Windows and macOS<br/>
from the same source, on Apple Silicon and Intel alike.<br/>
Only Eidos is Linux-only, because it is built on Linux mount namespaces.
</p>

&nbsp;

<h3 align="center">🛠 Tech Stack</h3>

<div align="center">

| Layer | Technology |
|:-----:|:----------:|
| **Language** | Rust · TypeScript |
| **GUI frameworks** | Iced, Tauri, Electron |
| **Data** | SQLite (via rusqlite), TOML and JSON on disk |
| **Secrets** | OS keyring (Secret Service, Credential Manager, Keychain) |
| **System access** | FUSE and mount namespaces, NVML (NVIDIA), sysfs (AMD/Intel) |
| **Platforms** | Linux, Windows, macOS |
| **Release** | GitHub Actions, release-please, AUR |

</div>

&nbsp;

<h3 align="center">🎨 Theming</h3>

<p align="center">
The launcher ships <b>57 palettes across 25 families</b>, compiled into the binary —<br/>
no theme files to download, no runtime parsing.
</p>

<table align="center">
<tr>
<td align="center">🐱 <b>Catppuccin</b><br/><sub>Latte · Frappé · Macchiato · Mocha</sub></td>
<td align="center">🪵 <b>Gruvbox</b><br/><sub>Light · Dark</sub></td>
<td align="center">❄️ <b>Nord</b><br/><sub>Dark · Light</sub></td>
<td align="center">🌊 <b>Kanagawa</b><br/><sub>Wave · Dragon · Lotus</sub></td>
</tr>
<tr>
<td align="center">🌃 <b>Tokyo Night</b><br/><sub>Night · Day</sub></td>
<td align="center">🌹 <b>Rosé Pine</b><br/><sub>Main · Moon · Dawn</sub></td>
<td align="center">🌲 <b>Everforest</b><br/><sub>Dark · Light</sub></td>
<td align="center">🧛 <b>Dracula</b><br/><sub>Dark · Light</sub></td>
</tr>
</table>

<p align="center">
<sub>…and Everblush, Solarized, One Dark, Monokai, Ayu, Material, Flexoki, Nightfox, Sonokai,<br/>
Oxocarbon, Night Owl, Iceberg, Horizon, Melange, Synthwave '84, Modus, and a fan-made Stellar Blade set.</sub>
</p>

<p align="center">
Each theme combines with <b>8 accent colors</b>, and the same palettes are bundled into SphereCord,<br/>
so your Discord client matches the rest of the desktop. A high-contrast mode<br/>
and an OpenDyslexic option ship alongside them.
</p>

&nbsp;

<h3 align="center">🔏 Signed Releases</h3>

<p align="center">
Colony verifies its own updates against an <b>ed25519 public key compiled into the binary</b>,<br/>
and refuses to install anything that fails: a missing, malformed or invalid signature<br/>
aborts the update instead of trusting it.
</p>

<p align="center">
The apps in the store publish detached signatures against that same key.<br/>
Once an app has been installed with a verified signature, the launcher will<br/>
refuse a later unsigned build of it — a repository cannot quietly stop signing.
</p>

&nbsp;

<h3 align="center">🌍 Internationalization</h3>

<p align="center">
Interface translations are static string tables compiled into each binary —<br/>
no runtime overhead, no external files, and fonts adapt to the active language.
</p>

<p align="center">
D1Gg2r offers <b>50 selectable languages</b> (falling back to English where a translation is incomplete),<br/>
while Colony and Grape are fully bilingual in <b>English and French</b>.
</p>

&nbsp;

<h3 align="center">🗺 Roadmap</h3>

<p align="center">Here's what's ahead:</p>

<p align="center">
◇ Lilypad, a local-first password manager, as the next app in the catalog<br/>
◇ Wider translation coverage across the ecosystem<br/>
◇ More packaging targets beyond the AUR<br/>
◇ Community-contributed apps and themes
</p>

&nbsp;

<h3 align="center">👐 Contributing</h3>

<p align="center">
Colony is open to contributions!<br/>
Whether it's bug fixes, new utilities, theme additions, or translations — all help is welcome.
</p>

<p align="center">
Each app lives in its own repository under the <a href="https://github.com/Project-Colony">Project-Colony</a> organization.<br/>
Pick one, open an issue or submit a PR.
</p>

&nbsp;

<h3 align="center">📄 License</h3>

<p align="center">
Colony and its applications are released under the <b>GNU General Public License v3.0 or later</b>.<br/>
This is copyleft: you are free to use, study, share and modify them, provided<br/>
derivative works keep the same freedoms. See the LICENSE file in each repository.
</p>

&nbsp;

<p align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="60" width="0px"/>
</p>

<p align="center">
	<sub>Built with 🦀 and ❤️</sub>
</p>
