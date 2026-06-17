# w3w-dispatch

**911 CAD Training Console** — what3words geofence mapping, ANI/ALI parsing, and mock dispatch testing.

## Files

| File | Purpose |
|---|---|
| `index.html` | Main CAD console — map, geofence draw, ANI/ALI parser, w3w lookup, incident log |
| `trigger.html` | Mock ANI/ALI sender — inject test calls into the console |

## Usage

1. Open `index.html` in one browser tab (the console)
2. Open `trigger.html` in a second tab (the trigger)
3. Enter your [what3words API key](https://developer.what3words.com/) in the console settings panel
4. Draw a geofence on the map using the rectangle or polygon tools
5. Fire a mock call from the trigger tab — the console parses the payload, drops a pin, looks up the w3w address, and flags whether the pin is inside the fence

## Deploying to Vercel

1. Import this repo at [vercel.com/new](https://vercel.com/new)
2. Select the repo and click **Deploy** — no build config needed
3. Your console will be live at `https://your-project.vercel.app/`
4. Trigger page at `https://your-project.vercel.app/trigger.html`

## what3words API Key

Get a free API key at [developer.what3words.com](https://developer.what3words.com/). Enter it in the console's Settings panel at runtime — no environment variables needed.
