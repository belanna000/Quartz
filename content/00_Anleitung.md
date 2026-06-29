# Anleitung zur Vault-Struktur

## Ordner

- **00_Scans** – Inbox für schnell abgelegte Scans/Fotos, die noch nicht verarbeitet/zugeordnet sind.
- **00_Dashboard** – Startseite mit Live-Übersichten.
- **00_Übersichten** – eigenständige Bases-Dateien (Datenbankansichten), auch einzeln öffenbar.
- **01_Schüler** – ein Profil pro Schüler/Schülerin.
- **02_Klassen** – ein Profil pro Klasse.
- **03_Fehlzeiten** – ein Eintrag pro Fehlzeit-Ereignis.
- **04_Dokumente** – Referenznotizen zu archivierten Dokumenten (Original liegt in der Cloud, siehe unten).
- **05_Sitzplan** – folgt im nächsten Schritt (Excalidraw).
- **06_Checklisten** – wiederkehrende Abläufe (z. B. Schuljahresbeginn).
- **07_Kurse** – OneNote-Ersatz: ein Hub pro unterrichtetem Kurs, darunter ein Unterordner mit einer (oder mehreren) Excalidraw-Leinwänden pro Unterrichtsdatum.
- **99_Vorlagen** – Vorlagen für neue Notizen.
- **_Anhänge** – Ablage für eingefügte Bilder/Dateien (z. B. Schülerfotos).

## Kurse (OneNote-Ersatz mit Excalidraw)

Aktuell angelegt: **Mathe 7.14** und **Leistungskurs Physik 12**. Weitere Kurse, die noch nicht feststehen, lassen sich jederzeit nachtragen:

1. Neue Notiz in 07_Kurse anlegen, Vorlage `99_Vorlagen/Vorlage_Kurs.md` einfügen (Cmd/Strg+N, dann „Vorlage einfügen").
2. Gleichnamigen Unterordner unter 07_Kurse anlegen (z. B. `07_Kurse/Deutsch 9a/`).
3. Pro Unterrichtstermin eine Leinwand in diesem Unterordner ablegen – Dateiname z. B. `2026-09-15 Bruchrechnung.excalidraw.md`, Vorlage `99_Vorlagen/Vorlage_Kursnotiz.excalidraw.md`. Bei Bedarf mehrere Leinwände am selben Tag (z. B. nach Thema benennen).
4. Im Frontmatter der Leinwand `kurs` auf die Kurs-Notiz verlinken (z. B. `kurs: "[[07_Kurse/Deutsch 9a]]"`) und `datum` setzen – dann taucht sie automatisch in der Tabelle der Kurs-Notiz auf.

Das Community-Plugin **Excalidraw** ist installiert und aktiviert. Eine Leinwand lässt sich damit auch direkt per Rechtsklick im Unterordner → „New drawing" erzeugen, statt die Vorlage zu kopieren – die Beispiel-Leinwände in 07_Kurse zeigen das Dateimuster.

`klassen` im Kurs-Frontmatter ist optional – sinnvoll, wenn ein Kurs einer festen Stammklasse entspricht (z. B. Mathe 7.14), aber leer lassen bei kursweise gemischten Gruppen (z. B. Leistungskurse).

## Neue Notiz anlegen

Cmd/Strg+N im jeweiligen Ordner, dann über den Befehl „Vorlage einfügen" (Templates-Plugin) die passende Vorlage aus 99_Vorlagen wählen. Die Vorlagen tragen die Grundfelder (Frontmatter) automatisch vor.

## Wie die Verknüpfung funktioniert

Schüler-, Fehlzeiten- und Dokumentnotizen sind über Wikilinks im Frontmatter verbunden (z. B. `schueler: "[[01_Schüler/Name]]"`). Die eingebetteten Bases in jeder Notiz filtern automatisch auf "gehört zu dieser Notiz" – dafür muss nur das jeweilige Feld (schueler/klasse) korrekt verlinkt sein, der Rest passiert automatisch.

## Dokumente archivieren

Diese Notizen sind **Referenzen**, keine Dateispeicher: das Originaldokument (z. B. gescannte Versäumnisanzeige) liegt im verbundenen Cloud-Speicher (SharePoint/Dateispeicher), der Link dazu steht im Feld `cloud_link`. So bleiben sensible Originaldokumente nicht zwangsläufig im lokal/mobil synchronisierten Vault, sondern nur die Verwaltungsmetadaten.

## Fehlzeiten

`art` ist eines von: offen, entschuldigt, unentschuldigt. Die Übersicht „Unentschuldigt - offen" (in der Fehlzeiten-Übersicht und im Dashboard) zeigt automatisch alle Fälle, bei denen noch keine Versäumnisanzeige verschickt wurde.

## Bemerkungen zu Schülerinnen/Schülern

Jedes Schülerprofil hat einen Abschnitt **„## Bemerkungen"** für freie Notizen (z. B. familiäre/gesundheitliche Besonderheiten, Förderbedarf, Sitzplatz-Empfehlungen). Dazu zwei Frontmatter-Felder:

- `besonderheiten: true/false` – auf `true` setzen, wenn im Abschnitt „Bemerkungen" etwas Relevantes steht. Schaltet die Notiz in die Ansicht „Mit Bemerkungen" (Schüler-Übersicht und in der Klassen-Notiz).
- `sitzplatz_hinweis` – kurzer Stichpunkt für Sitzplatz-relevante Hinweise (z. B. „vorne sitzen"), wird später für das Sitzplan-Tool nützlich sein.
- `foerderbedarf` – Stichwort zum sonderpädagogischen Förderbedarf (z. B. „Sprache", „Lernen"), falls vorhanden. Eigene Spalte/Ansicht „Förderbedarf" in der Schüler-Übersicht und in der Klassen-Notiz filtert automatisch auf alle SuS mit gesetztem Wert.

## Pflichtformulare (Schuljahresbeginn)

Sechs wiederkehrende Formulare müssen von allen Eltern und Schülerinnen/Schülern unterschrieben werden: Zustimmung Schulverfassung, Fotoerlaubnis, Zustimmung Sporthallenordnung, Antrag Schülerausweis, Datenschutzerklärung Office 365, Kenntnisnahme Fehlzeiten. Ablauf pro eingegangenem Formular-Set: Scan in 00_Scans ablegen → pro Formular eine eigene PDF heraustrennen und in _Anhänge ablegen → je eine Referenznotiz in 04_Dokumente anlegen (`typ` = Formularname, `schueler` verlinkt) → Eintrag in der passenden Checkliste in 06_Checklisten anlegen/ergänzen (ein Eintrag pro Formular, mit Bool-Haken für Eltern- bzw. Schülerunterschrift, je nachdem was das Formular vorsieht). Beispiel/erstes Set: [[06_Checklisten/Pflichtformulare Schuljahresbeginn - 7.14]].

## Checklisten-Tabelle im Klassenprofil

Damit sich Haken aus allen Checklisten an einer Stelle schnell setzen lassen, hat jedes Schülerprofil zusätzlich Bool-Felder im Frontmatter: `ev1_anwesend` (1. Elternversammlung) sowie `pf_schulverfassung_e/s`, `pf_foto_e/s`, `pf_sporthalle_e/s`, `pf_ausweis_e/s`, `pf_o365_e/s`, `pf_fehlzeiten_e` (Pflichtformulare, `_e` = Elternunterschrift, `_s` = Schülerunterschrift). Die Klassen-Notiz [[02_Klassen/7.14]] zeigt sie im Abschnitt „## Checklisten" als anklickbare Tabelle (Ansicht „Alle Haken" sowie „Offene Pflichtformulare" für alle, die noch nicht komplett sind). Ein Klick auf eine Checkbox in der Tabelle setzt direkt den Wert im jeweiligen Schülerprofil – die ausführlichen Quellen mit Anmerkungen bleiben in den einzelnen Notizen in 06_Checklisten. Kommt eine neue wiederkehrende Checkliste hinzu, am besten nach demselben Muster verfahren: neues Bool-Feld in `99_Vorlagen/Vorlage_Schüler.md` und allen Schülerprofilen ergänzen, dann Spalte in der Checklisten-Tabelle hinzufügen.

## Kandidatenstammblatt und Notfallkontakte

Manche SuS legen ihrem Pflichtformulare-Set zusätzlich ein **Kandidatenstammblatt** bei (Schulverwaltungs-Ausdruck mit Stammdaten, Vorder- und Rückseite). Vorderseite enthält i. d. R. Geburtsdatum/-ort, Anschrift, Staatsangehörigkeit sowie beide Erziehungsberechtigte (Name, Anschrift, Mobil, Rolle); Rückseite enthält das **Verhalten im Krankheits-/Unfallfall** (darf das Kind selbständig nach Hause gehen? zusätzliche abholberechtigte Personen mit Telefon/Anschrift, ggf. chronische Erkrankung).

Vorgehen, wenn ein Stammblatt im Scan auftaucht:

1. Geburtsdatum, Anschrift und (falls noch leer) `eltern_name`/`eltern_telefon` ins Schülerprofil übernehmen (bei zwei Erziehungsberechtigten beide kommagetrennt eintragen, z. B. „Mario Günther (Vater), Sylvia Günther (Mutter)").
2. Die beiden Frontmatter-Felder `notfall_selbststaendig_nach_hause` (Werte: ja / nein / wird abgeholt) und `notfall_chronische_krankheit` (Freitext, leer falls nichts angegeben) aus der Rückseite eintragen.
3. Zusätzliche, von den Erziehungsberechtigten abweichende Abhol-/Notfallkontakte (Name, Telefon, Anschrift) im Abschnitt **„## Notfallkontakte"** des Schülerprofils als Liste ergänzen.
4. Das Stammblatt selbst wie die anderen Formulare als eigenes Dokument (`typ: Kandidatenstammblatt`) in `_Anhänge`/`04_Dokumente` ablegen.

Diese Daten (Gesundheits-/Notfallbezug) fallen unter denselben Datenschutz-Hinweis wie „Bemerkungen"/Förderbedarf weiter unten – entsprechend vorsichtig behandeln.

## Datenschutz-Hinweis

Es handelt sich um personenbezogene Daten von Minderjährigen. Vor dem produktiven Einsatz lohnt sich ein kurzer Check mit dem schulischen Datenschutzbeauftragten bzw. den Berliner Vorgaben zur Schul-IT (insbesondere zur Nutzung von Cloud-Speicher und KI-Tools für diese Daten).

Die „Bemerkungen" und der Förderbedarf (Gesundheits-, sonderpädagogische und soziale Daten wie ADHS/LRS-Diagnosen, Medikation, Wohnsituation, Förderschwerpunkt) zählen zu **besonders schutzwürdigen Daten** (Art. 9 DSGVO – besondere Kategorien personenbezogener Daten) und verdienen nochmal mehr Vorsicht als reine Kontakt-/Fehlzeitendaten: Sync auf alle Geräte bedeutet, dass diese Informationen überall mitlaufen, wo der Vault offen ist (auch z. B. beim Bildschirmteilen). Auch hier gilt: vorab kurz mit dem Datenschutzbeauftragten abstimmen, ob/wie das im Vault zulässig ist.

## Nächste Schritte (offen)

- Sitzplan-Tool mit Excalidraw (Bildern, pro Klasse)
- Mail-Extraktion aus Outlook (Kontaktdaten/Fehlzeiten automatisch erfassen)
- Kalender-Aktualisierung
- OCR/Einlesen gescannter Dokumente und automatische Zuordnung zu Schülern
- Weitere Kurse nachtragen, sobald der Stundenplan feststeht
