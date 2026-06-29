---
tags: [kurs]
fach: 
kursbezeichnung: {{title}}
klassen: 
schuljahr: 2026/2027
---

# {{title}}

## Leinwände / Notizen
```base
filters:
  and:
    - file.hasTag("kursnotiz")
    - note.kurs == this
views:
  - type: table
    name: Leinwände
    order:
      - note.datum
      - note.thema
```

## Material

## Notizen

Unterordner mit gleichem Namen wie diese Notiz anlegen ({{title}}/) und dort pro Unterrichtsdatum eine Leinwand (Vorlage_Kursnotiz.excalidraw.md) ablegen.
