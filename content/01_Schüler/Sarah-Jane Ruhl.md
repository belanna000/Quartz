---
tags: [schueler]
vorname: Sarah-Jane
nachname: Ruhl
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2014-03-23
strasse: Blumberger Damm 219
plz_ort: 12687 Berlin-Marzahn
eltern_name: Melanie Ruhl (Mutter)
eltern_telefon: 0155 66919694
eltern_email: 
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
notfall_selbststaendig_nach_hause: ja
notfall_chronische_krankheit: 
letzte_aktualisierung: 2026-06-29
---

# Sarah-Jane Ruhl

## Bemerkungen



## Kontakt


## Notfallkontakte

Zusätzliche abholberechtigte/erreichbare Personen im Krankheits- oder Unfallfall (aus dem Kandidatenstammblatt, abweichend von den Erziehungsberechtigten):

- Binding, Stephan – 01629392554 – Blumberger Damm 219, 12687 Berlin (Anschrift nicht eigenständig angegeben, vermutlich wie Mutter)

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

Geburtsdatum, Anschrift und Erziehungsberechtigte aus dem Kandidatenstammblatt (Scan vom 2026-06-29) übernommen. Zuletzt besuchte Schule: Grundschule am Bürgerpark, Berlin-Marzahn, 1. Einschulung 01.08.2020, Fremdsprache Englisch.

4 von 6 Pflichtformularen eingereicht (Schulverfassung, Ausweis, O365, Foto), alle nur von der Mutter unterschrieben, Schülerin-Unterschrift fehlt überall (unter 14 Jahre, bei Foto entfällt das ohnehin). Beim Schülerausweis-Antrag und bei O365 steht im Datumsfeld jeweils das Geburtsdatum der Schülerin statt eines Unterschriftsdatums – wirkt wie ein Eintragungsfehler der Mutter. Sporthallenordnung und Fehlzeiten fehlen noch.
