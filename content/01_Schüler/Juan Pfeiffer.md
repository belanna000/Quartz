---
tags: [schueler]
vorname: Juan
nachname: Pfeiffer
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2012-01-16
strasse: Märkische Allee 244 A
plz_ort: 12679 Berlin-Marzahn
eltern_name: Sheila Pfeiffer (Mutter)
eltern_telefon: 0163/6744424
eltern_email: sheilapfeiffer@gmail.com
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
notfall_selbststaendig_nach_hause: ja
notfall_chronische_krankheit: keine Angabe
letzte_aktualisierung: 2026-06-29
---

# Juan Pfeiffer

## Bemerkungen



## Kontakt


## Notfallkontakte

- Schwarzkopf, Mirden (Vater) – 0172 2311776
- Pfeiffer, Maria (Oma) – 0176 57380220

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

Stammdaten aus dem Kandidatenstammblatt (Scan vom 2026-06-29) übernommen: geb. 16.01.2012 in Flensburg, Geburtsland Deutschland, Familiensprache Deutsch, zuletzt Paavo-Nurmi-Grundschule Berlin-Marzahn besucht, 1. Einschulung dort am 06.09.2024, Fremdsprache Englisch. Der auf der Stammblatt-Rückseite zusätzlich eingetragene Notfallkontakt mit identischer Telefonnummer (Pfeiffer, Sheila, 0163/6744424) ist dieselbe Mutter, die bereits oben als Erziehungsberechtigte erfasst ist. Siehe [[04_Dokumente/2026-06-29 Kandidatenstammblatt - Juan Pfeiffer]].

3 von 6 Pflichtformularen mit Elternunterschrift eingereicht (Ausweis, O365, Foto), Schülerunterschrift fehlt jeweils. Bei der Fotoerlaubnis fällt auf, dass Juan mit 14 Jahren bereits selbst hätte unterschreiben sollen (Formular sieht das „ab 14 Jahren" vor), hat aber nicht unterschrieben. Schulverfassung, Sporthalle und Fehlzeiten fehlen noch.
