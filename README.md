# SousChef - Voice Cooking Companion

A simulated **Alexa+ experience** for the *Build, Ship, Shape: Amazon Developer Hackathon* (Alexa+ track, simulated-experience path).

SousChef is a hands-free kitchen assistant. You tell it what ingredients you have, it suggests recipes, then walks you through the chosen recipe step by step by voice, with built-in timers.

## Features

- **Ingredient-based suggestions**: say "I have eggs and tomato" and get the best-matching recipes, plus what you'd still need.
- **Guided cooking**: say "start Tomato Pasta", then "next", "back" or "repeat" for each step.
- **Smart timers**: steps that need timing offer a timer ("start timer"), or say "set a timer for 5 minutes". Several timers can run at once and an alarm sounds when each finishes.
- **Voice in, voice out**: uses the browser's Web Speech API for speech recognition and speech synthesis. Typing and one-tap suggestion chips work too.
- 8 built-in recipes (omelette, pasta, fried rice, aloo jeera, dal tadka, poha, grilled cheese, banana pancakes).

## Run it

No build step and no API keys.

1. Clone this repo.
2. In the repo folder, start a local server (the microphone works on `localhost`):
   ```
   python3 -m http.server 8000
   ```
3. Open `http://localhost:8000` in **Google Chrome** or Edge (best Web Speech support).
4. Click the microphone button and speak, or type in the box.

Try: "I have eggs and tomato" -> "start omelette" -> "next" -> "next" -> "next" -> "start timer".

## Project structure

- `index.html` - the entire app (UI, intent routing, recipe data, timers, speech).
- `LICENSE` - MIT.

## Built with

Plain HTML, CSS and JavaScript, plus the browser Web Speech API. Built with the help of Claude (Anthropic) as the agentic coding tool.

## License

MIT - see `LICENSE`.
