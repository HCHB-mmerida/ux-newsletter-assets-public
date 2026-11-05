# Shared Public Assets

This folder contains reusable, non-issue-specific assets for the UX newsletter.

Use this for assets that are constant across issues, including:
- Branding (for example, HCHB logo)
- Team avatars reused in multiple issues
- Outlook-safe avatar fallback variants

Folder layout:
- `shared/branding/`
- `shared/avatars/`

URL pattern:
- `https://raw.githubusercontent.com/HCHB-mmerida/ux-newsletter-assets-public/main/shared/<category>/<file>`

## Team avatar standard

- Use `avatars/<person>.png` as the canonical portrait: 116x116 with a white background, a 1px `#D8DADD` circular rim, and no soft-shadow padding.
- Use the matching `*-<size>-circle.png` file for Outlook, with `<size>` matching the rendered avatar size.
- When a portrait changes, regenerate its listed fallbacks from the same crop and sync both `email-assets/shared/avatars/` and this folder.
- In Figma and standard templates, use the canonical shared portrait rather than a separate, manually cropped copy.

Guidelines:
1. Prefer shared assets in new issue templates when applicable.
2. Keep issue-specific assets under `ux-newsletter-issueN/`.
3. Add/update entries in `shared/reusable-assets.json` whenever shared assets change.
