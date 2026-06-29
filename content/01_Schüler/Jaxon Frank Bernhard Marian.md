---
tags:
  - schueler
vorname: Jaxon Frank Bernhard
nachname: Marian
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2013-04-23
strasse: Ludwig-Renn-Str. 3,1
plz_ort: 12679 Berlin
eltern_name:
eltern_telefon:
eltern_email: anjamarian@web.de
status: aktiv
foto:
besonderheiten: true
sitzplatz_hinweis: vorne sitzen (ADHS/LRS)
foerderbedarf: Lernen
ev1_anwesend: true
pf_schulverfassung_e: true
pf_schulverfassung_s: false
pf_foto_e: true
pf_foto_s: false
pf_sporthalle_e: true
pf_sporthalle_s: false
pf_ausweis_e: true
pf_ausweis_s: false
pf_o365_e: true
pf_o365_s: false
pf_fehlzeiten_e: true
notfall_selbststaendig_nach_hause: 
notfall_chronische_krankheit: 
letzte_aktualisierung: 2026-06-29
---

# Jaxon Frank Bernhard Marian

⚠️ Unterschrift auf der Liste sehr schwer leserlich – Anwesenheit nach bestem Ermessen vermerkt.

## Bemerkungen

Starkes ADHS und LRS. Förderbedarf Lernen. Sollte möglichst vorne sitzen. ADHS-Medikamente sind zu Hause vorhanden.

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

Geburtsdatum und Anschrift aus dem Antrag auf Schülerausweis (Pflichtformulare-Set vom 23.06.2026) übernommen. Alle 6 Pflichtformulare eingereicht (jeweils nur Elternunterschrift).
