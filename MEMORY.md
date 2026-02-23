# MEMORY.md - Long-Term Memory

## Identity
- My name is Kevin. Russell named me on 2026-02-23, first session.
- Running on Kevin's Mac mini (M4 chip, Apple Silicon), America/Denver timezone.

## Russell
- Fractional CMO, ~10 years marketing + ops experience
- Physics degree, former co-founder (warranty software, sold to Corso)
- Got fired from Corso after strategy conflict — good story
- Direct, wants to learn, hates AI yes-man behavior, wants Socratic pushback
- Careful with token spend — be smart with model selection

## Channels
- **Primary:** Webchat dashboard (http://127.0.0.1:18789)
- **Slack:** Connected and working as of 2026-02-23. Russell's Slack ID: U091VCDLREJ

## Tools & Config
- **Whisper:** `whisper <file> --model turbo --device mps --fp16 False --output_format txt --output_dir <dir>`
  - Must use --fp16 False (MPS + FP16 = NaN crash)
  - TODO: switch to mlx-whisper for much faster M4 transcription
- **OpenClaw config:** ~/.openclaw/openclaw.json
- **Restart gateway:** `launchctl bootout gui/$(id -u) ~/Library/LaunchAgents/ai.openclaw.gateway.plist` then `launchctl bootstrap gui/$(id -u) ~/Library/LaunchAgents/ai.openclaw.gateway.plist`

## Projects (Priority Order)
1. **Podcast pipeline** — The Fundamental Edge: research → validate → quiz → script → record → AI-edit → Captivate
2. **Business database** — Forbes/HBR/blog links + summaries for podcast research
3. **Weekly podcast briefs** — auto-pull from Founders, HTTTW, Marketing Against the Grain, etc.
4. **Campaign brief system** — competitor ad analysis + creative briefs for clients
5. **Personal story database** — Russell's experiences for podcast material

## Immediate Backlog
- Episode 4 of The Fundamental Edge: unedited, 2+ weeks delayed
- Aubrey Live needs 15-20 ad creatives/month — currently at 3
- Treads Plus needs lots of content

## Key Clients
- Zip String (kid's toy, Kickstarter)
- Amped Bikes (e-commerce, embedded ops role)
- Aubrey Live (fitness influencers, digital products)
- Treads Plus (stair nose flooring, DTC)
- Kivu (consumer AI software)
