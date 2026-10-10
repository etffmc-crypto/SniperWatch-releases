# SniperWatch (beta)

SniperWatch puts a "CURRENT STREAM SNIPER" callout on your stream when you or a mod types `!sniper <name>` in your Twitch, Kick or YouTube chat. It can also post the callout line in your Twitch chat. It runs on your PC; your chat is read directly from the platforms.

## Download
Get `SniperWatch-win-Setup.exe` from the latest entry on the [Releases page](../../releases). Windows 10 or 11, 64-bit. No admin rights needed; it installs for your user only.

## "Windows protected your PC"
The beta installer is not yet code-signed, so Windows SmartScreen shows a blue warning the first time. Click **More info**, then **Run anyway**. (Screenshots: `docs/smartscreen-1.png`, `docs/smartscreen-2.png`.)

## First run
1. SniperWatch opens its dashboard at http://localhost:17890/ and starts a short setup: your channel, the overlay link for OBS, a connection check and your commands.
2. In OBS add a **Browser** source with the overlay link from the wizard (`http://localhost:17890/overlay`), 1920×1080, and place it over your game.
3. In your chat type `!sniper TestSniper`. The callout shows on the overlay for 7 seconds.
4. Optional: Settings → Chat posting → Connect Twitch to post the callout line in Twitch chat.

SniperWatch lives in the tray (near the clock). Double-click the icon for the dashboard; right-click for the menu.

## What data is sent
- Nothing, unless you turn on **Send anonymous usage statistics** (setup wizard or Settings). Then small event records (app started, a callout fired on which platform, a command ignored, an error type) go to the authors. Never names, channel names, chat text or settings. Full list in Settings → the privacy policy link.
- **Send a report** on the About tab sends the diagnostics text, your note and, only if you tick it, today's log file.
- Updates: the app asks this repo's Releases page for newer versions and installs one only when you click "Restart to update".

## Known limits (beta)
- Twitch chat posting only; Kick and YouTube posting come later.
- One Twitch account at a time; the sign-in lasts about 30 days.
- Unsigned installer (SmartScreen prompt once).

## Feedback
Open an [issue](../../issues), or use **Send a report** in the app.
