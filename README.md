## Movie App — Fade-in Cards

A lightweight, single-file web app that showcases a top-10 movies grid with smooth, staggered fade-in animations powered by the Intersection Observer API. Includes instant search (by title, genre, or year), a shuffle action, and thoughtful accessibility touches.

### Features
- **Fade-in reveal**: Cards animate into view as you scroll (Intersection Observer).
- **Staggered timing**: Subtle delays per card via a CSS variable for a polished look.
- **Instant search**: Filter by title, genres, or year with a single input.
- **Shuffle**: Randomize the list while preserving the animation.
- **Accessible details**: Semantic elements, ARIA labels, and a keyboard shortcut (`r`) to reveal cards.

### Tech Stack
- **HTML**: Semantic structure
- **CSS**: Modern, minimal styling with variables and responsive layout
- **JavaScript**: Vanilla JS for rendering, filtering, shuffling, and observing

### Getting Started
1. Clone or download this repo.
2. Open `index.html` directly in your browser, or serve it locally:

```bash
# Option A: Python
python3 -m http.server 5173
# then visit http://localhost:5173

# Option B: Node (serve)
npx serve . --listen 5173 --single
```

### Usage
- Type in the search box to filter by title, genre(s), or year.
- Click "Shuffle" to randomize the current list.
- Scroll to reveal cards; press `r` to reveal all cards with a staggered animation.

### File Structure
- `index.html` — Contains HTML, CSS, and JS in a single file.

### Short Project Spec
- **Goal**: Present a small, elegant movie gallery demonstrating modern front-end fundamentals without frameworks.
- **Users**: Anyone browsing top movies and testing UI interactions/animations.
- **Core Requirements**:
  - Render a list of 10 movie cards with poster, title, year, genres, and rating.
  - Animate cards into view as they enter the viewport.
  - Provide a text search that matches title, genres, or year.
  - Provide a shuffle action to randomize the list.
  - Maintain responsive layout on small screens.
- **Non-Functional Requirements**:
  - Smooth, performant animations (no jank on scroll).
  - Accessible controls with ARIA where appropriate; keyboard shortcut for reveal.
  - No build step; works by opening `index.html`.
- **Nice-to-Have Enhancements (Future)**:
  - Movie details modal on "Details" click.
  - Persist last search/shuffle state in `localStorage`.
  - Replace placeholder images with a real API (e.g., TMDB) and handle loading states.
  - Unit tests for filter and shuffle utilities.

### License
MIT


