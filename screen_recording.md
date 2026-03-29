# Learn about screen recording tools #47
## What are the best free and paid screen recording tools for Windows/macOS?
windows:
free- OBS sudio
paid- EaseUS, RecExperts

macOS:
free- Built-in screenshot, OBS studio
paid- CleanShotX

## How do you record a specific part of the screen instead of the entire display?
Windows: Use OBS or EaseUS—select "Region" mode, drag to crop app window or area.

macOS: Press Shift+Cmd+5, choose "Selected Portion," drag rectangle; or OBS for precise window capture.

## What are best practices for including screen recordings in bug reports?
best practices should include:
1.Start video with environment, show steps to reproduce slowly, highlight error, explain expected vs. actual.
2.Add text summary: title, frequency, impact on users
3.Embed/link video

## How can you reduce video file sizes while maintaining good quality?
Use H.264/HEVC codecs at 1080p/30-60fps; trim clips to 30-60 seconds.
Free compressors like Handbrake reduce size 70-90% by lowering bitrate (5-10 Mbps), removing audio if silent

## What key information should you include when submitting a screen recording of a bug?
key info include:
1.Steps to reproduce, environment, expected vs. actual, frequency/impact.
2.Timestamp bug moment in video
3.Attach logs/DevTools for context.

## How can you ensure sensitive information is not accidentally shared in a recording?
1.Pre-record: Close tabs/apps, use incognito, cover notifications.
2.Post-edit: Blur faces/emails/URLs with Camtasia or Vmaker tools; crop regions.
3.Review full playback; use secure links 

## If a bug only happens during fast interactions, how would you record and describe it effectively?
I would record at 60fps; perform actions deliberately but at normal speed, repeat 2-3x.
 