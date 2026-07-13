# Recordings

Upload journal club session recordings here (via the GitHub web UI: **Add file → Upload files**, or `git add`/`git push` if you're working locally).

**Naming convention:** `YYYY-MM-DD-presenter.<ext>` — e.g. `2026-07-08-kamren-khan.mp4`, matching the session's date and the presenter name used on the site and in `sessions/`.

**Linking it from the website:** once a file is uploaded here, its public URL is:

```
https://github.com/cajigaslab/journal-club/raw/main/recordings/<filename>
```

Set that as the `recordingUrl` for the matching session in `restorelab`'s
`LabGuide/journal-club/literature-club-website/lib/content.ts`, then rebuild and redeploy the site (see that repo's README) — the "Recording not posted yet" text will switch to a "Watch the recording" link automatically.

**Size limit:** GitHub blocks any single file over 100 MB pushed via plain git. Most screen recordings of a journal club session will exceed that. If a recording is too large:
- Compress it first (e.g. `ffmpeg -i in.mp4 -vcodec libx264 -crf 28 out.mp4` gets most screen recordings well under 100 MB), or
- Use [Git LFS](https://git-lfs.com) for this repo (free tier: 1 GB storage / 1 GB bandwidth per month — fine for a few recordings, not for a large archive), or
- Host the video elsewhere (Zoom cloud, Google Drive, YouTube unlisted) and just put that URL in `recordingUrl` instead — it doesn't have to be a file in this folder, that's just the convenient default for a fully self-contained setup.
