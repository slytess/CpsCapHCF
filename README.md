# CPSCap - CPS Limiter for Spigot 1.8.9

CPSCap is a simple, no-nonsense plugin for Minecraft Spigot 1.8.9 servers, built to stop autoclicker abuse in PvP, especially for Hardcore Factions (HCF) servers. It tracks player clicks per second (CPS), filters out block clicks to keep things fair, and blocks hits when players go over the CPS limit.

**Made by slytes**  
📱 Telegram: [t.me/pfspovs](https://t.me/pfspovs)  
💬 Discord: drossrotzank

## What It Does
- Caps player CPS at a limit you set (default: 18 CPS).
- Ignores block clicks (like digging) so they don’t mess up CPS counts.
- Cancels hits and sends a warning message when players exceed the CPS limit.
- Lets you tweak settings like CPS limit and penalty duration in `config.yml`.
- Runs smoothly on Spigot 1.8.9 with Java 7, keeping performance tight.
- No extra fluff—just what you need for PvP control.

## See It in Action
Check out the demo:  
[🎥 CPSCap Demo Video](https://youtu.be/9GHMLDFu5BE)  
The video shows:  
- Clicking at 18-19 CPS in PvP with an autoclicker.  
- Warning message when hitting the CPS limit (18 CPS).  
- Clicking blocks to prove the filter works (no CPS inflation).

## How to Install
1. Grab `CPSCap-1.0-SNAPSHOT.jar` from the [Releases](https://github.com/slytess/CpsCap/releases/tag/CpsCap) page.
2. Drop the `.jar` into your Spigot 1.8.9 server’s `plugins/` folder.
3. Restart the server or run `/reload`.
4. Edit `plugins/CPSCap/config.yml` to customize settings (see below).

## Configuration
On first run, `config.yml` appears in `plugins/CPSCap/`. Here’s the default setup:

```yaml
max-cps: 18
warning-message: "&cYou have exceeded the server's CPS limit, please keep it below 18."
penalty-duration: 2000
