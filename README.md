# DigiClass STEM MVP

Eerste werkende versie van een AI-ondersteunde STEM-projectengine.

## Wat werkt al?

- Projecten aanmaken voor een team en school
- Zestien begeleide ontwikkelingsstappen
- Lokale feedbackcoach zonder API-kosten
- Optionele OpenAI-feedback via de Responses API
- Voortgang per project
- Automatische productpagina
- Automatisch pitchscript in Shark Tank-stijl
- Lokale JSON-opslag voor snelle demo's
- Responsive interface voor laptop, tablet en smartphone

## Lokaal starten

Vereisten: Node.js 20.9 of nieuwer.

```bash
npm install
cp .env.example .env.local
npm run dev
```

Open daarna `http://localhost:3000`.

## AI inschakelen

De app werkt zonder API-sleutel met een lokale regelgebaseerde coach. Voor generatieve feedback:

```env
OPENAI_API_KEY=jouw_sleutel
OPENAI_MODEL=gpt-5-mini
```

Herstart daarna de ontwikkelserver.

## GitHub publiceren

```bash
git init
git add .
git commit -m "Initial DigiClass STEM MVP"
git branch -M main
git remote add origin https://github.com/JOUW-NAAM/digiclass-stem-mvp.git
git push -u origin main
```

## Belangrijke MVP-beperking

De gegevens worden lokaal in `data/store.json` bewaard. Dit is goed voor demonstraties en feedbackgesprekken, maar niet voor een nationale productieomgeving. De volgende technische stap is authenticatie, PostgreSQL, organisaties/scholen, rollen, bestandsuploads en een auditlog.

## Organisch ontwikkelprincipe

Nieuwe functies worden pas toegevoegd na aantoonbare feedback uit gesprekken met leerlingen, leerkrachten, directies of bedrijven. Bewaar feedback als GitHub Issues met labels zoals `feedback`, `school`, `bedrijf`, `pedagogiek`, `privacy` en `verdienmodel`.
