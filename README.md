# Music Generator

Real-time browser-based music generator with interactive controls.

## Idea

Web app for generating ambient/lo-fi music in real-time with customizable parameters. Perfect for vibe coding sessions.

## Tech Stack

- **Frontend:** React + TypeScript + Vite
- **Audio:** Tone.js (Web Audio API wrapper)
- **Styling:** CSS Modules or Tailwind

## Features

### MVP
- [ ] Basic synth engine with Tone.js
- [ ] Play/Pause controls
- [ ] Real-time parameter controls:
  - Tempo (BPM)
  - Key/Scale selection
  - Reverb amount
  - Filter cutoff
  - Volume

### Phase 2
- [ ] Multiple instrument layers (pads, bass, arpeggios, percussion)
- [ ] Preset configurations (lo-fi, ambient, chillhop)
- [ ] Randomize button for happy accidents

### Phase 3
- [ ] Audio visualization (waveform, spectrum)
- [ ] Save/Load configurations (localStorage)
- [ ] Export to audio file

### Future Ideas
- [ ] Share configs via URL
- [ ] User presets gallery
- [ ] MIDI input support

## Architecture

```
src/
├── components/
│   ├── Controls/
│   │   ├── Slider.tsx
│   │   ├── Knob.tsx
│   │   └── Select.tsx
│   ├── Player/
│   │   └── Player.tsx
│   └── Visualizer/
│       └── Visualizer.tsx
├── audio/
│   ├── engine.ts        # Main Tone.js setup
│   ├── synths.ts        # Synth configurations
│   ├── sequences.ts     # Note patterns
│   └── effects.ts       # Reverb, delay, filter
├── hooks/
│   └── useAudioEngine.ts
├── types/
│   └── index.ts
├── App.tsx
└── main.tsx
```

## Getting Started

```bash
# Install Node.js first: https://nodejs.org/

# Clone and setup
git clone https://github.com/AndyIshch/music-generator.git
cd music-generator

# Install dependencies
npm install

# Run dev server
npm run dev
```

## Dependencies

```json
{
  "dependencies": {
    "react": "^18.x",
    "react-dom": "^18.x",
    "tone": "^14.x"
  },
  "devDependencies": {
    "@types/react": "^18.x",
    "@vitejs/plugin-react": "^4.x",
    "typescript": "^5.x",
    "vite": "^5.x"
  }
}
```

## References

- [Tone.js Docs](https://tonejs.github.io/)
- [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- [Music theory for generative music](https://learningmusic.ableton.com/)

## License

MIT
