# Website-redesigns — onderhandelingstool

Deze repo bevat verbeterde versies van bestaande websites van handelaren en
bedrijven. Het idee: een verouderde/lelijke site krijgt hier een moderne,
overzichtelijke variant die je **direct kunt laten zien** en als
onderhandelingsmiddel kunt gebruiken.

## Werkwijze

1. **Stuur een URL** van de bestaande website.
2. Ik bekijk de site — inhoud, diensten, branding en kleuren.
3. Ik kopieer het startsjabloon (`_template/`) naar `klanten/<bedrijfsnaam>/`
   en bouw daar een verbeterde versie: dezelfde kernboodschap, maar moderner,
   strakker en gericht op conversie (duidelijke call-to-action, mobielvriendelijk).
4. De verbeterde site is **losse HTML/CSS** — geen installatie nodig.

## Een site bekijken

Elke map in `klanten/` is volledig zelfstandig. Bekijken kan op twee manieren:

- **Snel:** dubbelklik op `index.html` in de betreffende map; opent in je browser.
- **Netjes (aanbevolen):** open een terminal in de mapfolder en draai een
  lokale server:

  ```bash
  cd klanten/<bedrijfsnaam>
  python3 -m http.server 8000
  ```

  Ga daarna naar <http://localhost:8000> in je browser.

## Mapindeling

```
.
├── README.md            ← dit bestand
├── _template/           ← herbruikbaar startsjabloon voor een nieuwe redesign
└── klanten/             ← één submap per bedrijf
    └── <bedrijfsnaam>/  ← bv. autobedrijf-jansen/
```

## Uitgangspunten

- **Geen build, geen dependencies** — puur HTML/CSS/vanilla JS, werkt offline.
- **Zelfstandige mappen** — elke klant-map staat volledig op zichzelf.
- **Snel aanpasbaar** — kleuren en lettertypes staan centraal in CSS-variabelen.
