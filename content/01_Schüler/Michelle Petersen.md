---
tags: [schueler]
vorname: Michelle
nachname: Petersen
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2014-01-05
strasse: Robensteiner Straße 15
plz_ort: 12689 Berlin
eltern_name: 
eltern_telefon: 
eltern_email: Sabrina-Voigt@kabelmail.de (Pflegemutter)
status: aktiv
foto: 
besonderheiten: false
sitzplatz_hinweis: 
foerderbedarf: 
ev1_anwesend: true
pf_schulverfassung_e: true
pf_schulverfassung_s: false
pf_foto_e: true
pf_foto_s: false
pf_sporthalle_e: false
pf_sporthalle_s: false
pf_ausweis_e: true
pf_ausweis_s: false
pf_o365_e: true
pf_o365_s: false
pf_fehlzeiten_e: false
notfall_selbststaendig_nach_hause: 
notfall_chronische_krankheit: 
letzte_aktualisierung: 2026-06-29
---

# Michelle Petersen

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

Geburtsdatum und Anschrift aus dem Antrag auf Schülerausweis (Pflichtformulare-Set vom 23.06.2026) übernommen. Kontakt ist die Pflegemutter (Nachname Voigt, abweichend von Petersen). 4 von 6 Pflichtformularen eingereicht (Schulverfassung, Ausweis, O365, Foto); Sporthalle und Fehlzeiten fehlen noch.
