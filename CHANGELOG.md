# Changelog

## v1.2.1

- Seamless playback & no spinner over already-loaded reels: eliminated buffering spinner overlays during video playback and loops; added 350ms grace delay and suppressed loaders on prefetched/cached reels
- Robust cold startup & auto-retry: unconditional cached feed restoration from Hive on frame 1 so the app never shows a blank or error screen on startup; added 3-stage automatic retry loop with exponential backoff and page-1 fallback
- High-efficiency preloading: in-flight prefetch preservation across swipes, zero-delay queue execution, and `allowImplicitScrolling` on the vertical reel pager for instant swipe-to-play
- Circular progress percentage indicator: real-time buffering and progressive loading percentage inside circular loaders for video playback, vault reels, and search
- Search overhaul: submit-only search trigger (keyboard enter/tick) eliminates keystroke stutter and network congestion
- Dynamic multiline niches: search result niche categories wrap dynamically across multiple lines to fit any screen size
- Deep black background: eliminated white screen / flash on search and keyboard transitions
- Fast search response: zero debounce on submit with interactive API prioritization
- Video aspect ratio precalculation: horizontal and square videos stay in original aspect ratio without vertical stretching or snap-back
- Play Store direct links: sponsored ads directing to Google Play Store apps now open directly in the Play Store app
- Feed speed & freshness: single high-throughput batch query, page skipping, and interest-based recommendations for fast startup and non-repeating reels

## v1.2.0 (build 2013)

- Niche sorting now lives in the reel player’s More sheet, giving the video the full screen again
- AI filter moved to Settings → Content filters
- Ads render in a portrait-friendly frame, wait for a real creative before showing, and give landing pages a progress bar, back button and close control
- Profile redesigned with a frosted header and capsule tabs for Likes, History and Following
- Navbar nudged down 2 px to sit with the system navigation area

## v1.2.0 (build 2012)

- Inline sponsored page: the Adsterra native banner now renders inside the reel feed, with a large X that closes it and advances
- Niche reels sort inside the niche: Trending (default), Most viewed, Newest, Oldest, Most liked
- AI filter rebuilt: works independently of hidden topics, ignores words like “waiting”, and has a persisted Hide creator action with undo
- Explore stays responsive: background niche import pauses off-screen, interactive API priority, static thumbnails and memoized sorting
- Data Saver (Settings → Connection): no reel preloading, SD quality
- In-app update checker: silent daily check, prompt on new releases, manual check in Settings → About
- Fixes from your reports: sponsor cadence, landscape rails and sheets

## v1.1.1

- Reel preloading: while a reel plays, the next 2 preload quietly — swiping feels near-instant
- Landscape support: compact action rails, scroll-safe sheets, adaptive Insights grid, denser Profile toolbars
- Sponsor cadence tuned: first prompt a few reels after install, then every 30 reels or 10 minutes (max 10/day)

## v1.1.0 — first public release

- Vertical reel feed (Home, Search, Explore, niche reels, creator profiles)
- Likes, watch history, follows — all stored on-device
- Personal Vault: save reels and videos for offline viewing
- Downloads manager with pause-style cancel, retry and per-file progress
- Usage Insights + wellbeing controls (daily limits, hidden topics)
- GIF export with trim, A/B loop and quality options
- Tablet and DeX-friendly adaptive layouts
- Support the project via Ko-fi / UPI / PayPal, or by visiting our sponsor
