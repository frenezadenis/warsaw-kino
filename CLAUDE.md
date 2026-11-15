# CLAUDE.md

## Project goal

- Build a public website listing all movie screenings in Warsaw for today and the next 2 weeks. Later, expand to other Polish cities.
- Second goal: the owner is learning to work with AI tools through this project.

## Owner

- Not a developer; has very little web development knowledge.
- Uses macOS.

## Stack (do not change without discussion)

- Python scrapers → `screenings.json` → static HTML/JS site → hosted on Cloudflare Pages.
- Daily runs via GitHub Actions.

## Data collection rules

- Collect facts only: film, time, cinema, language, format, ticket purchase link.
- Request each site no more than once a day.
- Use an honest User-Agent that identifies the project.
- Respect `robots.txt`.
- Never copy posters or film descriptions.
- Do not use Filmweb as a source.

## Working rules

- Always reply to the owner in Russian. Code, comments, commit messages and files stay in English.
- Before each action, briefly explain to the owner what you are doing and why, in plain words.
- Never delete files without explicit confirmation.
- Add files to commits by name only; never use `git add .` or `git add -A`.
- Every working session ends with a commit and `git push`.
- Secrets (passwords, keys, tokens) never go into the repository.

## Documentation

- `docs/schema.md` — format of one screening.
- `docs/sources.md` — list of cinemas and how data is collected.
- `docs/decisions.md` — decision log (date, decision, why).
