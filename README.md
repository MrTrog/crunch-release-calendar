# Anime Release Calendar

A weekly calendar of anime episodes, laid out by day and time like the old Crunchyroll simulcast calendar.

**Unofficial project. It is not affiliated with Crunchyroll.** The data comes from the public [AniList](https://anilist.co) API.

## Features

- Releases from Monday to Sunday, converted to your time zone.
- Available in English, Português, Español, Français, Deutsch and Italiano. The language is detected from your browser, and you can change it with the selector.
- Dates, times (12 h or 24 h) and numbers follow your computer's regional settings.
- Filters for anime on Crunchyroll, your favourites (★), episodes that are already out, and English titles. There is also a search box.
- Hover over an episode (or tap ⓘ on a phone) to see the score, season, studio, genres and synopsis. The synopsis is translated into the language you picked.
- Your favourites and settings are saved in your own browser. The site has no server and no accounts.

## How it works

The whole site is a single `index.html` with no build step and no dependencies. It runs in the visitor's browser:

- The schedule comes from the AniList GraphQL API. Each visitor makes their own requests.
- The week is cached in `localStorage` for 30 minutes and refreshed in the background.
- The synopsis is translated with the browser's built-in translator when one is available (Chrome/Edge). Otherwise it falls back to Google Translate's public endpoint and then to MyMemory.

The episode times are the Japanese broadcast times. On Crunchyroll, an episode usually comes out at the same time or up to about an hour later.

## Running locally

Open `index.html` in a browser. Nothing else is needed.

---

# Calendário de lançamentos de anime

Um calendário semanal dos episódios de anime, organizado por dia e horário, como o antigo calendário de simulcast da Crunchyroll.

**Projeto não oficial, sem ligação com a Crunchyroll.** Os dados vêm da API pública do [AniList](https://anilist.co).

Para usar, basta abrir o `index.html` no navegador.
