---
tags: [schueler]
vorname: Sophia
nachname: Baumann
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 
strasse: 
plz_ort: 
eltern_name: 
eltern_telefon: 
eltern_email: kathinka@familienbandeberlin.de (Wohngruppe, kein Elternteil)
status: aktiv
foto: 
besonderheiten: true
sitzplatz_hinweis: 
foerderbedarf: Sprache
ev1_anwesend: true
pf_schulverfassung_e: false
pf_schulverfassung_s: false
pf_foto_e: false
pf_foto_s: false
pf_sporthalle_e: false
pf_sporthalle_s: false
pf_ausweis_e: false
pf_ausweis_s: false
pf_o365_e: false
pf_o365_s: false
pf_fehlzeiten_e: false
notfall_selbststaendig_nach_hause: 
notfall_chronische_krankheit: 
letzte_aktualisierung: 2026-06-29
---

# Sophia Baumann

## Bemerkungen

Lebt in einer Wohngruppe. Förderbedarf Sprache.

## Kontakt


## Notfallkontakte


## Fehlzeiten
```base
filters:
  and:
    - file.hasTag("fehlzeit")
    - note.schueler == this
views:
  - type: table
    name: Fehlzeiten
    order:
      - note.datum_von
      - note.art
      - note.dauer_tage
      - note.versaeumnisanzeige_verschickt
```

## Dokumente
```base
filters:
  and:
    - file.hasTag("dokument")
    - note.schueler == this
views:
  - type: table
    name: Dokumente
    order:
      - note.datum
      - note.typ
      - note.status
```

## Notizen

Erfasst aus Klassenliste 7.14 (Anwesenheitsliste 1. Elternversammlung).
