# Changelog

## 0.4.0 — beta 1
- First public beta.
- Twitch chat posting works out of the box.
- Optional anonymous usage statistics and "Send a report".
- Updates from this repository's Releases, applied when you choose.

## 0.4.1 — update check
- No functional change: proves the in-app update from 0.4.0.

## 0.4.2 — Show on screen switch
- New "Show on screen" switch (Status tab button, tray menu item, hotkey Ctrl+Alt+Shift+O, Settings → Overlay). Off: the OBS overlay stays blank while `!sniper` keeps working; every callout still shows on the dashboard and under Recent callouts, so you and your mods can use it without viewers knowing. Flip it on at any time; a callout that is up appears for its remaining seconds. The choice is remembered across restarts.
- A warning appears if the overlay is hidden while "Post callouts in Twitch chat" is on, since chat would still tell viewers.
- Diagnostics report the switch; the optional usage statistics gain one event (`overlay.visibility`: shown/hidden and where from).
