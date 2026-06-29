---
tags: [schueler]
vorname: Luis
nachname: Henckel
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2014-09-13
strasse: Landsberger Allee 54A
plz_ort: 12679 Berlin
eltern_name: 
eltern_telefon: 
eltern_email: frjahn378@gmail.com
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
pf_ausweis_e: true
pf_ausweis_s: false
pf_o365_e: true
pf_o365_s: false
pf_fehlzeiten_e: false
notfall_selbststaendig_nach_hause: 
notfall_chronische_krankheit: 
letzte_aktualisierung: 2026-06-29
---

# Luis Henckel

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

Geburtsdatum und Anschrift aus dem Antrag auf Schülerausweis (Scan vom 2026-06-29) übernommen. Name auf dem Formular schwer leserlich ("Heuckel" vs. "Henckel") – als Henckel, Luis interpretiert, da dieser Name in der Klassenliste existiert und kein anderer passender Eintrag vorhanden ist. Im Original ggf. gegenprüfen.

3 von 6 Pflichtformularen eingereicht (Ausweis, O365, Foto); Schulverfassung, Sporthallenordnung und Fehlzeiten fehlen noch. Bei der Fotoerlaubnis ist die gesamte Medien-Ankreuztabelle leer geblieben, obwohl die Unterschrift vorhanden ist – rechtlich daher keine erteilte Erlaubnis, nachfragen.
