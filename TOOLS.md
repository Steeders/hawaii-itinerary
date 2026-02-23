# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup.

## Whisper (Speech-to-Text)

- **Always use:** `--device mps` to leverage the M4 GPU/Neural Engine
- **Default model:** `turbo` (good balance of speed + accuracy)
- **Full command:** `whisper <file> --model turbo --device mps --fp16 False --output_format txt --output_dir <dir>`
- `--fp16 False` is required — MPS + FP16 produces NaN errors with the turbo model
- Without `--device mps` it falls back to CPU (much slower)

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras

- living-room → Main area, 180° wide angle
- front-door → Entrance, motion-triggered

### SSH

- home-server → 192.168.1.100, user: admin

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

Add whatever helps you do your job. This is your cheat sheet.
