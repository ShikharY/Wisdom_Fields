# TEK Grow Guide – Prototype

A small, static prototype to explore high-level Indigenous ecological practices (TEK) for growers and gardeners. Users can enter their location, season, and topic/challenge to see summarized guidance.

## Important context
- Indigenous knowledge is relational, place-based, and stewarded by communities. This prototype provides generalized, high-level practices for learning only.
- For application beyond learning, consult and partner with local Indigenous knowledge holders and follow their protocols.
- Original inspiration: the U.S. National Park Service overview of Traditional Ecological Knowledge (TEK).

## Run locally
No build step. Use any static server or open `index.html` directly.

- Quick start on macOS/Linux:
```bash
python3 -m http.server --directory "$HOME/tek-grow-guide" 8080
# then visit http://localhost:8080
```

## Accessibility
- Keyboard focusable chips and cards
- High contrast dark theme
- Reduced motion support
- ARIA live region for results

## Data model
`data/tek.json` – array of entries:
```json
{
  "title": "...",
  "region": "Great Plains; Eastern Woodlands",
  "seasons": ["Spring", "Summer"],
  "topics": ["corn", "companion planting"],
  "summary": "...",
  "practices": ["..."]
}
```

## Ethics and attribution
- This demo does not include tribe-specific knowledge. Do not treat it as comprehensive or prescriptive.
- Always attribute and seek consent for local knowledge.
