This is Semiblock Type Code documentation repo

Type Code is a Semiblock educational module that trains coding fluency by having users type real, useful source code snippets instead of random text.

## What is Type Code?

- Practice typing actual runnable programs in Python and JavaScript
- Lessons range from simple "Hello World" to classes, loops, array methods, and async/await
- Real-time feedback: errors are highlighted as you type
- Metrics: live timer, error count, WPM (words per minute), and accuracy %
- Only your personal bests are saved (faster time, or same time with fewer errors)
- Global rankings and per-lesson leaderboards (privacy-friendly display names)
- Dark/light themes, adjustable font size, full session persistence (refresh-safe)
- "Rankings" floating action button + in-app ranking dialogs

## How it works in the platform

- Feature-flagged module (slug: `typeCode`)
- React + TypeScript + MUI standalone app
- Dev server (localhost:8088) with automatic fallback to pre-built bundle at `/typeCode-build/bundle.js`
- Laravel backend (TypeCodeController) handles auth, score submission, stats, and leaderboards
- Follows the same sideloading / hot-reload pattern used by other modules (e.g. the model for TeensDB)

See the main platform dashboard card under Education for access.