---
tags: [schueler]
vorname: July
nachname: Ernst
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2013-11-15
strasse: Zossener Str. 165
plz_ort: 12627 Berlin-Hellersdorf
eltern_name: Nancy Ernst (Mutter), André Krause (Vater)
eltern_telefon: 
eltern_email: 
status: aktiv
foto: 
besonderheiten: false
sitzplatz_hinweis: 
foerderbedarf: 
ev1_anwesend: false
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

# July Ernst

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

Geburtsdatum, Anschrift und Erziehungsberechtigte aus dem Kandidatenstammblatt (Scan vom 2026-06-29) übernommen. Zuletzt besuchte Schule: Puerto-Grundschule Berlin-Hellersdorf, 1. Einschulung 01.08.2019, Fremdsprache Englisch. Telefonnummern der Erziehungsberechtigten auf dem Formular nicht eingetragen.

Rückseite (Notfallkontakte/Verhalten bei Krankheitsfall) ist komplett leer geblieben: kein Ankreuzen bei ja/nein/wird abgeholt, keine zusätzlichen Kontakte, kein Datum/Unterschrift. Stammblatt also nicht vollständig ausgefüllt – bei Gelegenheit nachfragen. Kein vollständiges Pflichtformulare-Set in diesem Scan enthalten (nur das Stammblatt).
