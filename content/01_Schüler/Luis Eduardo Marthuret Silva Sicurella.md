---
tags: [schueler]
vorname: Luis Eduardo Marthuret
nachname: Silva Sicurella
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2013-05-02
strasse: Lea-Grundig-Str. 76
plz_ort: 12687 Berlin-Marzahn
eltern_name: Monica Dubraska Sicurella Rodriguez (Mutter)
eltern_telefon: 01632822405 (Festnetz), +4915758505073 (Mobil)
eltern_email: monicasicurella85@gmail.com
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
notfall_selbststaendig_nach_hause: nein, wird abgeholt
notfall_chronische_krankheit: keine Angabe
letzte_aktualisierung: 2026-06-29
---

# Luis Eduardo Marthuret Silva Sicurella

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

Stammdaten, Anschrift und Kontaktdaten aus dem Kandidatenstammblatt (Scan vom 2026-06-29) übernommen: geboren in Caracas/Venezuela, Zuzug in die BRD am 01.09.2022, zuletzt Grundschule am Bürgerpark (Berlin-Marzahn) besucht, 1. Einschulung dort am 07.11.2022, Fremdsprache Englisch. Die auf der Stammblatt-Rückseite als Notfallkontakt eingetragene Mobilnummer (+4915758505073) gehört zur selben Mutter, die bereits als Erziehungsberechtigte mit Festnetznummer erfasst ist – daher als zweite Telefonnummer unter `eltern_telefon` ergänzt statt als eigener Eintrag unter „Notfallkontakte". Siehe [[04_Dokumente/2026-06-29 Kandidatenstammblatt - Luis Silva Sicurella]].

3 von 6 Pflichtformularen eingereicht (Ausweis, O365, Foto). Ausweis vollständig (nur Elternunterschrift, kein Passbild). Bei O365 zusätzlich Datum im eigentlich entfallenden Schülerfeld eingetragen, aber ohne Unterschrift. Bei der Fotoerlaubnis ist die Medien-Ankreuztabelle vollständig mit „ja" ausgefüllt, auf der Unterschriftenseite fehlt aber jede Unterschrift (weder Eltern noch Schüler) – damit formal keine wirksame Einwilligung trotz ausgefüllter Tabelle; nachfragen. Schulverfassung, Sporthalle und Fehlzeiten fehlen noch.

Zusätzlich lag eine Schulbescheinigung bei (kein Pflichtformular), siehe [[04_Dokumente/2026-06-29 Schulbescheinigung - Luis Silva Sicurella]].
