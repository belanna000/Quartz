---
tags: [schueler]
vorname: Jayden Jeremy Jacob
nachname: Back
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2013-11-24
strasse: 
plz_ort: 
eltern_name: 
eltern_telefon: 
eltern_email: mback91@gmail.com
status: aktiv
foto: 
besonderheiten: false
sitzplatz_hinweis: 
foerderbedarf: 
ev1_anwesend: true
pf_schulverfassung_e: false
pf_schulverfassung_s: false
pf_foto_e: true
pf_foto_s: false
pf_sporthalle_e: false
pf_sporthalle_s: false
pf_ausweis_e: false
pf_ausweis_s: false
pf_o365_e: true
pf_o365_s: false
pf_fehlzeiten_e: false
notfall_selbststaendig_nach_hause: 
notfall_chronische_krankheit: 
letzte_aktualisierung: 2026-06-29
---

# Jayden Jeremy Jacob Back

## Bemerkungen



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

Geburtsdatum aus dem O365-Formular übernommen. 2 von 6 Pflichtformularen eingereicht (O365, Foto), beide vollständig ausgefüllt und unterschrieben (Berlin, 23.6.26). Schulverfassung, Sporthalle, Ausweis und Fehlzeiten fehlen noch (keine Anschrift verfügbar, da bisher kein Antrag auf Schülerausweis vorliegt).
