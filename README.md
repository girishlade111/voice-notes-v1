# Voice Notes v1

A voice-to-text quick-notes UI component — jot down ideas using speech-to-text, then organize and search them with tags.

## Features

- **Voice input** — hands-free note capture (designed around Google ML Kit / Apple Speech speech-to-text).
- **Tag organization** — attach tags to every note; duplicate tags are deduplicated case-insensitively.
- **Full-text search** — instantly find notes by content.
- **No auth needed** — notes live in local component state; nothing leaves the browser.

## Tech stack

- React (functional components + hooks)
- TypeScript
- Tailwind CSS / shadcn-style UI components (`button`, `card`, `input`, `textarea`)
- lucide-react icons
- Planned: Firebase ML for offline voice processing

## Quick start

This is a drop-in React component. Copy the `voice-notes v1` component file into your project and adapt the imports to your component library:

```tsx
import VoiceNotes from './voice-notes-v1'

export default function App() {
  return <VoiceNotes />
}
```

Requirements: a React + Tailwind project with shadcn-style UI primitives (`@/components/ui/*`) and `lucide-react` installed.

## Project structure

```
voice-notes-v1/
├── voice-notes v1   # VoiceNotes React component (notes + tags + search UI)
├── README.md
└── LICENSE
```

## Deploy notes

No build or deployment step — this is a source component meant to be integrated into an existing React app, not a standalone site.

## Roadmap

- Wire the Mic button to the Web Speech API / ML Kit recognizer
- Persist notes to localStorage / IndexedDB (Dexie)
- Export notes as Markdown / share sheet

---

Built by [Girish Lade](https://ladestack.in) — part of the [LadeStack](https://ladestack.in) free-tools ecosystem.
