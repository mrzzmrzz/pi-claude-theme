# pi-claude-theme

Claude Code's look for the [pi](https://pi.dev) TUI. Two themes, faithful to the original palette:

- **claude-dark** — clay accent `#d77757`, periwinkle links, the signature pink bash mode
- **claude-light** — the same identity, tuned for light terminals

The palette is taken from Claude Code's built-in Dark/Light modes: clay for accents and headings,
periwinkle (`permission`/`suggestion`) for links and labels, Claude's own success/error/warning
greens and reds, its exact user-message and memory backgrounds, and `bashBorder` pink for bash mode.
Text stays on your terminal's default color, as both tools intend.

## Install

From a local checkout:

```bash
pi install /path/to/pi-claude-theme
```

Or, once published to GitHub:

```bash
pi install git:github.com/mrzzmrzz/pi-claude-theme
```

Then pick `claude-dark` or `claude-light` in `/settings`, or set it directly:

```json
{ "theme": "claude-light" }
```

## Try without installing

```bash
pi --theme ./themes/claude-dark.json --use-theme claude-dark
```

To follow terminal appearance:

```bash
pi --theme ./themes/claude-light.json --theme ./themes/claude-dark.json --use-theme claude-light/claude-dark
```

## Notes

- Thinking-level borders ramp from gray through teal, blue, and periwinkle up to clay — max thinking is full Claude.
- Both theme files hot-reload while active, so edits show up immediately.

## License

MIT
