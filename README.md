# Mission Control Index

Static index page for Stav's Second Brain / Mission Control project. Links to all key documents, data sheets, tools, and a live architecture diagram.

**Live at:** https://mission-control-index.netlify.app/

## How it works
- Single `index.html` file
- Auto-deploys to Netlify on push to `main`
- Updated by Claude Code when new docs or components are added

## Architecture diagram
The index includes a system architecture diagram where each component is marked as:
- `live` — green, solid border
- `wip` — blue, solid border
- `future` — grey, dashed border

To update a component's status, find its `<span class="nd ...">` tag and change the class. For example, to mark the Event Scout as in-progress:

```html
<!-- Before -->
<span class="nd future">Event Scout job</span>

<!-- After -->
<span class="nd wip">Event Scout job</span>
```

## Updating
Edit `index.html`, commit, push. Netlify deploys automatically within ~10 seconds.
