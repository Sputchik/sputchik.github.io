# 0.16.0
- Adapt to twitch's v2 HLS API

# 0.15.0
- Tweaked chart generation (grid/outline w/ colors)
- Titles and Games are now clickable in archive.org description (to player with offset)

# 0.14.1, 2025-10-18
- Fixed offset for first chat messages

# 0.14.0, 2025-09-29
- Added game slug parsing for stream metadata
- Moved Predictions & Polls below charts

# 0.13.7, 2025-09-10
- Revised recording to un-breakingly handle unstable streamers (since a long time ago)
- More aggressive ad segment handling (test)
- pre-0.14.0

# 0.13.6, 2025-09-09
- Better stat chart downscaling

# 0.13.5, 2025-09-07
- Video recording can now "blazingly" fast handle short streams (< 3-5s)
- 2K (1440p60) recording support
- Faster session boot

# 0.13.4, 2025-09-06
- fMP4 segments support - making available 2k and higher resolution recording
- Video recording now starts without a need of wait for metadata response via GQL
- Bits messages key trim
- Fixed TOP-chart generation
- WiP: 1. Cleaner fMP4 handling, 2. resolve issue with offset for long streams (twitch eventually breaks it), 3. streamer poll manager

# 0.13.3
- Robust fuckass video recording m3u8 playlist parsing

# 0.13.2
- Rewrote stream video recording function to skip ad segments (enhanced < 0.10.0 version)

### Technical details
- Simultaneous recording user limit (ignoring download bandwidth limit / no video recording) per IP: 5,000 (200 * 25)

- Simultaneous minimal recording limit (stream up/down & title/game changes) per IP: 15,000 (200 * 75)