# Influencer Analyst Plugin

Built by Sagar for the Plix team. Gives everyone at Plix a single command to deep-dive any public Instagram account — pulling real reel data, extracting scripts, and surfacing what's actually driving engagement.

---

## What it does

Run `/influencer-analysis` followed by any Instagram handle or profile URL. Claude will:

1. **Pull the last 90–120 days of reels** via Apify's Instagram Reel Scraper
2. **Rank the top 5–10 reels** by a composite score (views + engagement rate)
3. **Extract the script** for each top reel — using Apify's built-in transcript feature for spoken content, falling back to captions where needed
4. **Break down the hook** — identifies the hook type, the exact opening line, and explains why it stops the scroll
5. **Identify engagement drivers** — what specifically made each reel outperform
6. **Synthesise cross-reel patterns** — common hook formulas, topic clusters, format signals, posting cadence
7. **Deliver strategic takeaways** — grounded in the data, specific enough to brief a creative team

---

## How to use it

```
/influencer-analysis @handle
```

Or naturally — just tell Claude what you want:

> "Analyse @beerbicleps for me — I want to understand his top hooks"
> "Reverse-engineer what @fittuber is doing in the last 3 months"
> "Pull the top reels from https://www.instagram.com/ranveerallahbadia/"

---

## Requirements

- **Apify connected** — the skill uses Apify's `instagram-reel-scraper` to pull live data. Make sure the Apify MCP is connected in your Cowork session.
- **Apify transcript add-on** — transcripts are charged per audio minute on Apify. The skill enables this by default for best results. You can disable it in the skill if needed.

---

## Output

A structured report delivered in chat or as an artifact:

- Account overview (niche, follower count, posting cadence)
- Content performance summary (aggregate stats for the window)
- Per-reel deep dives (metrics, transcript, hook breakdown, engagement drivers)
- Cross-reel pattern analysis
- Strategic takeaways

---

## Known limitations

- **Very high-volume accounts** (e.g. Gary Vaynerchuk posting 8+ reels/day) — the default 60-reel cap may only cover 7 days rather than 90. Mention this to Claude and it will adjust.
- **Accounts with heavy bot protection** — some large accounts throttle Apify's scraper during peak hours. If a scrape returns empty, ask Claude to retry.
- **Transcripts on music-heavy reels** — ambient or music-only reels won't produce clean transcripts; captions are used as fallback and clearly marked.

---

## Version history

| Version | Date | Notes |
|---------|------|-------|
| 0.1.0 | May 2026 | Initial release — influencer-analysis skill |
