---
tags: [klasse]
kuerzel: 
klassenstufe: 
klassenlehrer: 
schuljahr: 2026/2027
---

# {{title}}

## Schülerliste
```base
filters:
  and:
    - file.hasTag("schueler")
    - note.klasse == this
views:
  - type: table
    name: Schüler
    order:
      - note.nachname
      - note.vorname
      - note.status
      - note.eltern_telefon
```

## Fehlzeiten dieser Klasse
```base
filters:
  and:
    - file.hasTag("fehlzeit")
    - note.klasse == this
views:
  - type: table
    name: Fehlzeiten
    groupBy:
      property: note.schueler
      direction: ASC
    summaries:
      note.dauer_tage: Sum
    order:
      - note.datum_von
      - note.art
      - note.dauer_tage
```

## Notizen

