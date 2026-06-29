---
tags: [schueler]
vorname: Jasper Carlisle Ray
nachname: Pätzold
klasse: "[[02_Klassen/7.14]]"
geburtsdatum: 2013-08-06
strasse: Pöhlbergstr. 18
plz_ort: 12685 Berlin-Marzahn
eltern_name: Julia Pätzold (Mutter); Jeffrey Böhm (Vater)
eltern_telefon: "017682112545 (Mutter), 01762900361 (Vater)"
eltern_email: crazyjulchen92@yahoo.de (Mutter); jeffrey1990@web.de (Vater)
status: aktiv
foto: 
besonderheiten: false
sitzplatz_hinweis: 
foerderbedarf: 
ev1_anwesend: false
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
notfall_selbststaendig_nach_hause: "widersprüchlich: sowohl „nein“ als auch „wird abgeholt“ angekreuzt"
notfall_chronische_krankheit: keine Angabe
letzte_aktualisierung: 2026-06-29
---

# Jasper Carlisle Ray Pätzold

## Bemerkungen



## Kontakt


## Notfallkontakte

- Pätzold, Alice (Notfallkontakt) – 017620230524 – Pöhlbergstr. 18, 12685 Berlin

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

Geburtsdaten, Anschrift und Elternkontakte aus dem Kandidatenstammblatt (Scan vom 2026-06-29) übernommen. Eltern leben getrennt (Mutter Julia Pätzold, Vater Jeffrey Böhm), beide mit eigener Telefonnummer/E-Mail erfasst. Notfallkontakt Alice Pätzold (vermutlich Großmutter/Verwandte, gleiche Anschrift) von der Rückseite übernommen. Alle 6 Pflichtformulare eingereicht (Schulverfassung, Foto, Sporthalle, Ausweis, O365, Fehlzeiten), jeweils nur mit Elternunterschrift, Schülerunterschriften durchgängig leer.

Zwei Anomalien: (1) Auf der Stammblatt-Rückseite ist bei der Frage zur selbstständigen Heimkehr widersprüchlich sowohl „nein" als auch „wird abgeholt" angekreuzt/durchgestrichen – nicht eindeutig auflösbar. (2) Bei der Fotoerlaubnis ist die Tabelle uneinheitlich befüllt (anders als bei den meisten anderen SuS mit durchgängig ja/nein): Homepage nein/nein, Social Media nein/widersprüchlich (sowohl ja als auch nein markiert), Printpublikationen nein/ja, Aushänge nein/ja, Tagespresse nein/nein. Details siehe Dokument-Notiz zur Fotoerlaubnis.
