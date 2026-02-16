## Theme & Retro UI Settings

### Theme selection (System / Light / Dark)
- Open **Profile & Settings → Appearance** and use the **Theme mode** segmented control.
- `System` follows your OS/browser `prefers-color-scheme` setting.
- `Light` and `Dark` force the app theme directly.
- The selected mode is saved in `localStorage` (`ps_theme_mode`) and restored on reload.

### Where to adjust colors
- Global visual tokens live in `style.css` under the `:root` and `body.dark-mode` variable blocks.
- Main tokens to tune:
  - `--bg`, `--panel`, `--panel-strong`
  - `--text`, `--muted`, `--border`
  - `--accent`, `--glow`, `--focus-ring`
- Most core surfaces/components consume these CSS variables, so updating tokens cascades through cards, buttons, inputs, and navigation.

### Retro overlays (optional, default off)
- Open **Profile & Settings → Appearance**.
- Toggle any of these optional overlays:
  - **Retro grid overlay**
  - **Scanlines**
  - **CRT vignette**
- These are subtle visual layers and are disabled by default for clean, minimal daily use.
