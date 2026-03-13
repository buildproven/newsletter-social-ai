# Newsletter → Social AI

Turn any newsletter into a full week of LinkedIn + Twitter/X posts. Paste your content, get 8 ready-to-post pieces — hooks included, formatted for copy-paste, engineered from real performance data.

## How to Use

1. **Get the file** — Clone this repo or download `index.html`
2. **Open it** — Double-click `index.html`. No server, no install, no build step.
3. **Enter your API key** — Paste your [Anthropic API key](https://console.anthropic.com/settings/keys). It saves to your browser and never leaves your machine.
4. **Paste your newsletter → Generate** — Drop in your newsletter content and hit "Generate Social Posts". Posts are ready in ~10 seconds.

## What You Get

Every newsletter generates:

- **3 LinkedIn posts** — insight angle, story angle, and provocative question angle. Each with an estimated reach tier (🟢/🟡/🔴) and one-sentence "why this works" explanation.
- **5 Twitter/X posts** — 3 standalone tweets, 1 thread opener, 1 engagement tweet with a genuine question.
- **10 hook variations** — Opening lines labeled by angle (curiosity, data, confession, contrarian, specific). Use these to A/B test subject lines, post openers, and headlines.
- **Week schedule** — When to post each piece for maximum reach.
- **"Copy all as Markdown" export** — Download everything as a formatted `.md` file, ready to drop into Notion, Obsidian, or your content queue.

## Why It Works

The prompts aren't generic. They're engineered from real performance data — LinkedIn posts from a newsletter that went from 1,400 weekly reach to 38,000+ in six weeks. The AI knows why "I ran Claude Code for 40 days straight. Here's the honest scorecard." hit 24,000 impressions, and why "I've watched enough AI product builds go sideways..." hit 129. The difference is in the first line, every time.

Format rules are baked in: no "I'm excited to share", no hashtag spam, no buried insights. Specific numbers in line 1, honest tone throughout, concrete details over vague claims. The output skews toward what works — because bad patterns are explicitly ruled out in the prompt.

The app runs entirely in your browser. Your API key stays in localStorage. There's no backend, no database, no subscription. You pay Anthropic directly for the API calls (typically a few cents per generation with claude-3-5-haiku).

## Tech

Single HTML file. Tailwind CSS via CDN. Vanilla JavaScript. Zero dependencies, zero build step. Works offline after first load.

Calls the Anthropic Messages API directly from the browser using the `anthropic-dangerous-direct-browser-access` header (official CORS support).

## Built by BuildProven

[BuildProven](https://buildproven.ai) — Where experienced professionals turn expertise into AI-built products.

"Your expertise is the product. AI is just the factory."

## License

MIT. Use it, modify it, sell your own version of it. No attribution required (though appreciated).

See [LICENSE](LICENSE) for details.
