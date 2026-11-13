# GitHub Profile Refresh

This package contains a GitHub profile README and five original SVG visuals.

## Install

Upload `README.md` and the whole `assets/` directory into the root of the public `Sabstar71/Sabstar71` repository. GitHub's **Add file → Upload files** accepts multiple files, or use Git from a local clone:

```powershell
Copy-Item .\README.md -Destination "<profile-repo>\README.md" -Force
Copy-Item .\assets -Destination "<profile-repo>\assets" -Recurse -Force
```

Replace `<profile-repo>` with the path to a local clone of `https://github.com/Sabstar71/Sabstar71`. Commit and push. Avoid copying the files into the separate private `sabeeh-portfolio` website repository.

## Design notes

- One animated typing caption from `readme-typing-svg.demolab.com` (third-party service; unavailable if blocked or down)
- Original gradient SVG header and project covers (static art, no JavaScript, no user photo)
- One collapsible activity graph (third-party service)
- No fabricated project statistics; featured project URLs are chosen from known public repos or the user's site
- GitHub profile README does not execute JavaScript, and native SVG animation is not reliably supported by GitHub, so the supplied SVG assets are deliberately static.

The GitHub connector rejected the previous write attempt with HTTP 403; local files are provided for manual publishing. No GitHub content was changed by this package.
