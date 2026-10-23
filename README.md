# Vårgärdsvägen 73 – 3D-modell (statisk sajt)

`index.html` är hela viewern i en fil (three.js och modellen inbakade, ~3,6 MB). Inga beroenden, inget byggsteg.

## Engångs-setup (ca 5 min)
1. GitHub → New repository, t.ex. `v73-modell` (Private går bra).
2. Ladda upp `index.html`, `vercel.json` och den här README:n (Add file → Upload files → Commit).
3. vercel.com → Add New → Project → Import `v73-modell` → Framework preset: **Other**, Build command: tomt, Output directory: tomt → Deploy.
4. Klart. Varje ny commit till `main` publiceras automatiskt. Vill du begränsa åtkomst: Project → Settings → Deployment Protection.

## Uppdatera
Byt ut `index.html` i repot (Upload files → Commit) – Vercel publicerar inom ~30 s.
Snabbast: klona repot till en mapp på datorn, koppla mappen till Claude, så skriver Claude in nya `index.html` direkt och du trycker bara Push i GitHub Desktop.

## Skillnad mot claude.ai-versionen
Kameraknappen skickar bara till Figma när modellen öppnas i claude.ai (Figma-kopplingen). På Vercel laddas skärmdumpen ner som JPEG i stället – dra in den i ramen SKISS UPPDATERINGAR.
`vercel.json` sätter `noindex` så sidan inte hamnar i sökmotorer.
