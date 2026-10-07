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
Colony is an ecosystem of small, focused desktop utilities, nearly all of them built with Rust.<br/>
Instead of one monolithic tool that does everything poorly, Colony offers a curated set of apps,<br/>
each designed to do one thing well, with native performance and themeable interfaces.
</p>

<p align="center">
The <a href="https://github.com/Project-Colony/Colony">Colony launcher</a> ties them together: it installs, updates and launches<br/>
every app that publishes a <code>colony.json</code> manifest, and lists the apps already on your system alongside them.
</p>

&nbsp;

<h3 align="center">🧩 The Apps</h3>

<div align="center">

| App | What it does | Builds | In Colony |
|:---|:---|:---:|:---:|
| **[Colony](https://github.com/Project-Colony/Colony)** | Launcher and app store for the whole ecosystem | Linux · Windows · macOS | it *is* the store |
| **[Eidos](https://github.com/Project-Colony/Eidos)** | Native Linux mod manager for Bethesda games: mods are merged into a private, per-launch FUSE view, so the game directory is never touched | Linux | ✅ |
| **[Colony Firewall Control](https://github.com/Project-Colony/Colony-Firewall-Control)** | Application-aware outbound firewall, a Rust port of opensnitch with per-app prompts, a CLI and a tray companion | Linux | not yet |
| **[Raven](https://github.com/Project-Colony/Raven)** | Experimental: runs Windows programs from Linux against a real Windows installation mounted as C:, with Wine kept only at the syscall boundary | Linux | ✅ |
| **[Grape](https://github.com/Project-Colony/Grape)** | Music player for the music you already own: your folder is the library, with tag and cover art reading | Linux · Windows · macOS | ✅ |
| **[SphereCord](https://github.com/Project-Colony/SphereCord)** | Discord client (a fork of Equibop) with Equicord preinstalled and the Colony palettes bundled in | Linux · Windows | ✅ Linux |
| **[Spotter](https://github.com/Project-Colony/Spotter)** | Game library tracker: imports Steam, GOG, Epic, Xbox and PlayStation, follows playtime and achievements | Linux · Windows · macOS | ✅ |
| **[D1Gg2r](https://github.com/Project-Colony/D1Gg2r)** | System monitor: live CPU, memory, disk, network, temperature, GPU and processes, with persistent history | Linux · Windows · macOS | ✅ |
| **[orCAL](https://github.com/Project-Colony/orCAL)** | Desktop calculator, in a phone-shaped window or a tablet one with a scientific keypad | Linux · Windows · macOS | ✅ |
| **[SAM · Colony Edition](https://github.com/Project-Colony/SAM-Colony-Edition)** | Steam achievement manager: browse, unlock and edit the stats of games you own | Linux · Windows · macOS | ✅ |
| **[Lilypad](https://github.com/Project-Colony/Lilypad-Vault)** | Local-first password manager written in Rust. No release yet: it is listed in Colony, but the source and downloads arrive with its first release | none yet | listed only |

</div>

<p align="center">
<sub>Linux is the supported platform: every app is developed and tested there.<br/>
Windows and macOS builds are best-effort and are not code-signed, so expect SmartScreen and Gatekeeper warnings.</sub>
</p>

&nbsp;

<h3 align="center">🧱 Infrastructure</h3>

<div align="center">

| Repository | What it is |
|:---|:---|
| **[Project-Colony-Resources](https://github.com/Project-Colony/Project-Colony-Resources)** | Shared design tokens and UI conventions, the `colony-ui` crate, the `colony.json` schema and the release workflow templates |
| **[nix](https://github.com/Project-Colony/nix)** | Nix flake that packages Colony apps and tracks their releases automatically (SphereCord today) |
| **[Arch-Colony](https://github.com/Project-Colony/Arch-Colony)** | Arch-derived Linux distribution (not a fork) with the Colony programs, a signed `[colony]` repository and a hardened base; early, with an installable ISO |

</div>

&nbsp;

<h3 align="center">🧠 Philosophy</h3>

<p align="center">
<b>One app, one purpose</b>: each Colony tool solves a single problem with clarity and precision.<br/>
No feature bloat, no hidden complexity.
</p>

<p align="center">
<b>Native performance matters</b>: nearly everything is built in Rust.<br/>
Startup is instant, memory usage is minimal, and your CPU stays cool.
</p>

<p align="center">
<b>Beauty is not optional</b>: Colony, Eidos, Raven, Grape, D1Gg2r and Colony Firewall Control<br/>
share one theme library, <code>colony-ui</code>, so a palette looks the same wherever you meet it.<br/>
Tools should look as good as they work.
</p>

<p align="center">
<b>Linux first, honestly</b>: Linux is where the apps are built, used daily and tested.<br/>
Several apps also ship Windows and macOS builds from the same source, on Apple Silicon and Intel alike;<br/>
those are best-effort, and bug reports from them are welcome.
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
| **System access** | FUSE and mount namespaces, NFQUEUE and eBPF, NVML (NVIDIA), sysfs (AMD/Intel) |
| **Platforms** | Linux (supported), Windows and macOS (best-effort) |
| **Release** | GitHub Actions, release-please, AUR, Nix |

</div>

&nbsp;

<h3 align="center">🎨 Theming</h3>

<p align="center">
The launcher ships <b>59 palettes across 26 families</b> from <code>colony-ui</code>, compiled into the binary:<br/>
no theme files to download, no runtime parsing.
</p>

<table align="center">
<tr>
<td align="center">🐱 <b>Catppuccin</b><br/><sub>Latte · Frappé · Macchiato · Mocha</sub></td>
<td align="center">🪵 <b>Gruvbox</b><br/><sub>Light · Dark</sub></td>
<td align="center">❄️ <b>Nord</b><br/><sub>Dark · Light</sub></td>
<td align="center">🌊 <b>Kanagawa</b><br/><sub>Light · Dark · Journal · Dragon</sub></td>
</tr>
<tr>
<td align="center">🌃 <b>Tokyo Night</b><br/><sub>Night · Day</sub></td>
<td align="center">🌹 <b>Rosé Pine</b><br/><sub>Main · Moon · Dawn</sub></td>
<td align="center">🌲 <b>Everforest</b><br/><sub>Dark · Light</sub></td>
<td align="center">🧛 <b>Dracula</b><br/><sub>Dark · Light</sub></td>
</tr>
</table>

<p align="center">
<sub>...and Everblush, Solarized, One Dark, Monokai, Ayu, Material, Flexoki, Nightfox, Sonokai,<br/>
Oxocarbon, Night Owl, Iceberg, Horizon, Melange, Synthwave '84, Modus, Parchment, and a fan-made Stellar Blade set.</sub>
</p>

<p align="center">
Each theme combines with <b>8 accent colors</b>, and the same palettes are bundled into SphereCord,<br/>
so your Discord client matches the rest of the desktop. The launcher also offers<br/>
a high-contrast mode and an OpenDyslexic font option.
</p>

&nbsp;

<h3 align="center">🔏 Signed Releases</h3>

<p align="center">
Colony verifies its own updates against an <b>ed25519 public key compiled into the binary</b>,<br/>
and refuses to install anything that fails: a missing, malformed or invalid signature<br/>
aborts the update instead of trusting it.
</p>

<p align="center">
Store apps that declare <code>"signed": true</code> in their manifest publish detached signatures against that same key.<br/>
Once an app has been installed with a verified signature, the launcher will<br/>
refuse a later unsigned build of it: a repository cannot quietly stop signing.
</p>

&nbsp;

<h3 align="center">🌍 Internationalization</h3>

<p align="center">
Interface translations are static string tables compiled into each binary:<br/>
no runtime overhead and no external files.
</p>

<p align="center">
D1Gg2r offers <b>50 selectable languages</b> (falling back to English where a translation is incomplete),<br/>
while Colony and Grape are bilingual in <b>English and French</b>.
</p>

&nbsp;

<h3 align="center">🗺 Roadmap</h3>

<p align="center">Here's what's ahead:</p>

<p align="center">
◇ Lilypad's first release, with its source<br/>
◇ Colony Firewall Control in the Colony store<br/>
◇ Wider translation coverage across the ecosystem<br/>
◇ More packages in the Nix flake and the Arch Colony repository<br/>
◇ Community-contributed apps and themes
</p>

&nbsp;

<h3 align="center">👐 Contributing</h3>

<p align="center">
Colony is open to contributions!<br/>
Whether it's bug fixes, new utilities, theme additions, or translations, all help is welcome.
</p>

<p align="center">
Each app lives in its own repository under the <a href="https://github.com/Project-Colony">Project-Colony</a> organization.<br/>
Pick one, open an issue or submit a PR. Themes live in <a href="https://github.com/Project-Colony/Project-Colony-Resources">Project-Colony-Resources</a>.
</p>

<p align="center">
Found a security problem? Please report it privately, as described in our <a href="https://github.com/Project-Colony/.github/blob/main/SECURITY.md">security policy</a>.
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
