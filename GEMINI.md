# ProPost

ProPost drafts, schedules and publishes social media posts for the signed-in
user (LinkedIn, X, Bluesky, Threads, Mastodon, Instagram, Facebook, TikTok,
Pinterest, Google Business, YouTube, Telegram), in their own voice.

- Start with `get_account` (plan, drafts left, time zone, this connection's
  autonomy) and `list_channels` (ids, character limits).
- Each channel belongs to a brand: read `get_brand_brief` before writing a
  post yourself with `create_draft`, and never mix brands.
- `generate_draft` has ProPost write in the user's voice (one monthly draft).
- Times are ISO 8601 with an offset, in the user's time zone.
- `publish_now` and scheduled posts go public on the user's real accounts:
  confirm with the user first.
- The AI team: `get_team_status`, `ask_teammate` (talk to Maestro, Scout or a
  specialist about their work), `list_needs_you` / `resolve_needs_you`.

Sign-in is OAuth: the first call opens ProPost in the browser.
