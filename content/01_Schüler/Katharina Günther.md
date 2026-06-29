---
tags: [schueler]
vorname: Katharina
nachname: Günther
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2014-04-22
strasse: Wittenberger Str. 47
plz_ort: 12689 Berlin-Marzahn
eltern_name: Mario Günther (Vater), Sylvia Günther (Mutter)
eltern_telefon: 01721757790 (Vater), 01721757910 (Mutter)
eltern_email: 
status: aktiv
foto: 
besonderheiten: false
sitzplatz_hinweis: 
foerderbedarf: 
ev1_anwesend: true
pf_schulverfassung_e: false
pf_schulverfassung_s: false
pf_foto_e: false
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

# Katharina Günther

## Bemerkungen



## Kontakt


## Notfallkontakte

Zusätzliche abholberechtigte/erreichbare Personen im Krankheits- oder Unfallfall (aus dem Kandidatenstammblatt, abweichend von den Erziehungsberechtigten):

- Dietze, Michaela – 0176/55019092 – Wittenberger Str. 75, 12689 Berlin
- Dietze, Jürgen – 0155/166175106 – wie oben

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

Geburtsdatum, Anschrift und Erziehungsberechtigte aus dem Kandidatenstammblatt (Pflichtformulare-Set vom 23.06.2026) übernommen. Zuletzt besuchte Schule: Selma-Lagerlöf-Grundschule Berlin-Marzahn, 1. Einschulung 09.09.2020, Fremdsprache Englisch.
