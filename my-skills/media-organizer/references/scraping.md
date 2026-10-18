# Strict scraper matching

Optional reference. Read only when the user asks for stricter matching in a specific player, or when that player cannot identify a title with the library's normal naming. Normal organization follows `../SKILL.md`; do not rewrite a working library to these rules.

## Common rules

- One library per type: movies, TV, anime.
- One folder per title: `Title (Year)`.
- Season folders: `Season 01`; specials: `Season 00`.
- Episodes: `S01E01`; multi-episode files: `S01E01-E02`.
- One title per filename: the metadata source's primary title in the library language.
- Year: the source's primary release or first-air year.
- TV shows sit directly in the TV library; no franchise or label folders above them.
- Movies: one folder per movie; versions share the folder.

## Templates

```
Movies/
  Movie Title (Year)/
    Movie Title (Year).ext
TV/
  Show Title (Year)/
    Season 01/
      Show Title (Year) - S01E01 - Episode Title.ext
    Season 00/
      Show Title (Year) - S00E01 - Special Title.ext
```

## Plex

- Use the English word `Season` for season folders, even when the content is not English.
- Include the year with the series title in the folder and file names.
- Specials: `Season 00` or `Specials`.
- Editions: `{edition-...}`.
- Provider IDs: `{tmdb-...}`, `{tvdb-...}`, `{imdb-...}`.

## Jellyfin

- Series folder: `Series Name (Year) [tmdbid-...]`.
- Season folders: `Season 01`; specials `Season 00`.
- One folder per movie; version filenames start with the folder name.
- Multiple versions: same season folder, same `SxxExx`, suffix `- 1080p` or `- 720p`.

## Emby and Kodi

- Same core structure; provider ID syntax varies by scraper.
- Kodi: `Show/Season 01/Show - S01E01 - Title.ext`; movies `Movie (Year)/Movie (Year).ext`.

## How to use

1. First try a manual match or a provider ID.
2. Only if that fails, compare the path with these templates.
3. Change only the failing title; do not rename the whole library.
4. If the normal naming already works, leave it alone.
