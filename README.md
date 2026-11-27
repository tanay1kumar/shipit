# ShipIt

Type in a startup idea and get a research report on it that ends in go, conditional go or no go. Built at CTRL+HACK+DEL 2.0 with [QadeerKhan06](https://github.com/QadeerKhan06). [Devpost](https://devpost.com/software/shipit-yorhxt)

## What it does

- A Gemini agent searches the web for competitors, market size and user complaints, and pulls in Google Trends data.
- The results become a dashboard covering the product, the market, the competition and the verdict.
- AI advisors, like a skeptical VC or a target customer, argue with you about the idea. You can play their replies out loud with ElevenLabs.
- You can ask questions about the report, have parts of it rewritten, or export it.

## Run it

```bash
npm install
cp .env.example .env.local   # then add your keys
npm run dev
```

The code still uses `gemini-2.0-flash`, which Google scheduled to shut down in June 2026. You'll likely need to change the model in `src/lib/gemini.ts`.

Built with Next.js, TypeScript, Gemini, Serper, MongoDB and ElevenLabs.
