# Contributing to Lucidy Icons

## Icons
Only **official Lucide** SVG path data (https://github.com/lucide-icons/lucide). Convert to VectorDrawable — do not hand-draw replacements.

## Appfilter
Add mappings in `app/src/main/res/xml/appfilter.xml`:

```xml
<item component="ComponentInfo{package/activity}" drawable="lucidy_icon_name" />
```

## Build
```bash
./gradlew assembleRelease
```

Release signing uses env vars (same as Fern):
`RELEASE_STORE_FILE`, `RELEASE_STORE_PASSWORD`, `RELEASE_KEY_ALIAS`, `RELEASE_KEY_PASSWORD`

## PRs
Keep diffs focused. Update `RELEASE_NOTES.md` for user-visible changes.
