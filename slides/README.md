# Slides

Upload journal club presentation slides here (via the GitHub web UI: **Add file → Upload files**, or `git add`/`git push` if you're working locally).

**Naming convention:** `YYYY-MM-DD-presenter.<ext>` — e.g. `2026-10-16-pedro-borges.pptx`, matching the session's date and the presenter name used on the site and in `sessions/`.

**Linking it from the website:** once a file is uploaded here, its public URL is:

```
https://github.com/cajigaslab/journal-club/raw/main/slides/<filename>
```

Set that as the `slidesUrl` for the matching session in `restorelab`'s
`LabGuide/journal-club/literature-club-website/lib/content.ts`, then rebuild and redeploy the site (see that repo's README) — a "View the slides" link will appear on that session automatically.

**Size:** slide decks are usually small enough (a few MB to tens of MB) to push directly with no compression needed. If a deck is unusually large (large embedded video/images), the same fallbacks as `recordings/` apply — see that folder's README.

Note: the lab's [journal-club README](https://github.com/cajigaslab/restorelab/blob/main/LabGuide/journal-club/README.md) also references a Box folder for slides. Uploading here in addition (or instead) is fine — Box is the original convention, this folder just makes slides linkable directly from the site.
