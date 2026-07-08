# Shorts Factory

Shorts Factory is a **personal, single-user desktop tool** that generates
short-form videos on its developer's computer and uploads them to the
developer's **own YouTube channel** via the YouTube Data API v3.

## What it does

1. Composes short vertical videos locally (text-to-speech narration over
   Creative-Commons-licensed gameplay footage, with burned-in captions).
2. Uploads the finished videos to the developer's own channel using the
   official YouTube Data API (`videos.insert`, `youtube.upload` scope).

## What it is not

- It is **not distributed**: no downloads, no app store listing, no
  website, no users other than the developer.
- It does **not** access any other person's YouTube data — no comments,
  analytics, subscriber lists, or third-party channels.
- It stores its OAuth token locally on the developer's machine only.

## API usage

- Scope: `https://www.googleapis.com/auth/youtube.upload` only
- Calls: `videos.insert`, at most a handful per day (well within the
  default 10,000-unit daily quota)

## Privacy

See [PRIVACY.md](PRIVACY.md).
