# flowers

## Flower Bouquet Demo

This repository contains a decorative, animated flower bouquet page: `bouquet.html`.

Features
- Animated CSS flowers with staggered "bloom" effects.
- Subtle bouquet sway animation.
- Petal "shower" effect implemented with a pooled DOM element system and GPU-friendly CSS keyframe animations for better mobile performance.
- Color-theme button to cycle petal/center colors.
- Respects the `prefers-reduced-motion` accessibility setting.

Quick start
1. Open the file directly in your browser:

```bash
xdg-open bouquet.html
```

2. Or serve locally (recommended) and open http://localhost:8000/bouquet.html:

```bash
# from the repository root
python3 -m http.server 8000
```

Accessibility & performance notes
- If a visitor has `prefers-reduced-motion` enabled, the page will not run the bloom/sway/petal animations and will show a static bouquet instead.
- On mobile devices the petal shower is capped and uses a small pooled set of elements (fewer particles and shorter durations) to reduce layout and painting work.
- For very high particle counts or advanced performance needs, consider a Canvas-based particle system as a future improvement.

Files
- `bouquet.html` — main demo with inline CSS and JavaScript.

License
This repository contains demo code; adapt and reuse as you like. If you plan to publish publicly, please add a license file.

Next steps
- I can add a small demo GIF or screenshot to the README,
- add a `LICENSE` file (suggested: MIT), or
- implement an optional Canvas fallback for ultra-low-power devices.
# flowers