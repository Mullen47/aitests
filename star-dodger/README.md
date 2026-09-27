# Star Dodger

A tiny arcade game in a single HTML file. No build step and no dependencies.

## Play

Open `index.html` in any browser, or serve the folder:

```sh
python3 -m http.server -d star-dodger 8000   # then visit http://localhost:8000
```

- **Move:** ← → or A / D (on a touchscreen, drag with your finger)
- **Start / restart:** Space, Enter, or tap
- **Pause:** P

Dodge the red meteors and grab the yellow stars for +50 points. The game speeds up
the longer you survive. Your best score is saved in the browser's localStorage.

## Tweak it

All of the game lives in the `<script>` block in `index.html`:

- `speed = 1 + elapsed / 25` sets how fast the difficulty ramps up
- `spawnTimer` sets how often meteors appear
- `score += 50` is the bonus for a star
