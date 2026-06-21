# ux-consultant.be → 301 redirect naar uxconsultant.be

Dit is GEEN aparte website, maar een permanente (301) doorverwijzing.
`ux-consultant.be` en `uxconsultant.be` zijn bijna identiek; twee losse sites zouden
duplicaten zijn en elkaar wegconcurreren. De hoofdsite staat op `uxconsultant.be`
(die heb je al in Vercel opgezet); dit domein stuurt er met een 301 naartoe, zodat alle
autoriteit en links op één plek terechtkomen.

## Deployen op Vercel
1. Maak een nieuwe, lege repo met alleen deze `vercel.json` (en deze README).
2. Importeer de repo in Vercel.
3. Voeg in Vercel het domein `ux-consultant.be` toe (Project → Settings → Domains).
4. Zet bij je registrar de DNS zoals Vercel aangeeft (meestal A-record naar `76.76.21.21`
   of een CNAME naar `cname.vercel-dns.com`).

Resultaat: elke bezoeker van `ux-consultant.be/...` wordt met een 301 doorgestuurd naar
`https://uxconsultant.be/...`. Google volgt de 301 en bundelt de waarde op uxconsultant.be.
