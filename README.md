# To-do-Liste: Miniprojekt „Namen sind doch einfach“ – Schritt für Schritt

## 1. Aufgabenstellung genau verstehen

- [ ] Lies die vollständige Aufgabenbeschreibung.
- [ ] Notiere die **Hauptziele**:
  1. Ein inklusives Kontaktformular für ein Hotel entwerfen.
  2. Automatische Antwort-E-Mails mit passender Anrede ermöglichen.
  3. Begründen, warum die gewählte Lösung Namen und Geschlecht nicht zu stark vereinfacht.
  4. Ein Cheat-Sheet für Entwickler*innen erstellen.
  5. Fünf absichtlich schlechte Formulare entwickeln und ihre Probleme erklären.
  6. Präsentation, Forschungstagebuch/Stundenliste und Reflexion erstellen.  

- [ ] Lege einen Projektordner an, z. B.:
  ```text
  miniprojekt-namen/
  ├── 01_recherche/
  ├── 02_skizzen/
  ├── 03_prototyp/
  ├── 04_schlechte_formulare/
  ├── 05_praesentation/
  ├── 06_dokumentation/
  └── abgabe/
  ```

---

## 2. Stundenliste und Forschungstagebuch von Anfang an führen

- [ ] Erstelle eine Stundenliste, etwa als Tabelle:

| Datum | Dauer | Tätigkeit | Ergebnis | Problem/Hindernis | Nächster Schritt |
|---|---:|---|---|---|---|
| 01.11. | 1 h | Aufgabenstellung und Texte gelesen | Problemfälle gesammelt | viele Sonderfälle | Formularvarianten skizzieren |

- [ ] Ergänze die Liste **nach jeder Arbeitseinheit**.
- [ ] Dokumentiere dabei Aktivitäten, Ergebnisse, Hindernisse und Erfolge. Das wird ausdrücklich verlangt. 

- [ ] Erstelle zusätzlich ein Forschungstagebuch mit:
  - Recherche-Notizen,
  - Screenshots,
  - Skizzen,
  - verworfenen Ideen,
  - Begründungen für Entscheidungen,
  - Testfällen.

---

## 3. Recherche: Namen und Geschlecht als komplexe Daten verstehen

### 3.1 Die zwei vorgegebenen Texte lesen

- [ ] Lies **„Falsehoods Programmers Believe About Names – With Examples“**.
- [ ] Lies **„Falsehoods Programmers Believe About Gender“**.
- [ ] Notiere nur die Punkte, die für ein **textbasiertes Kontaktformular und E-Mail-Anreden** wichtig sind. Genau diese Priorisierung wird gefordert. 

### 3.2 Wichtigste Problemfälle für dein Projekt notieren

#### A. Problemfälle bei Namen

- [ ] Menschen haben nicht zwingend genau einen Namen oder nur eine verwendete Namensform. Manche verwenden je nach Kontext unterschiedliche Namen, etwa einen amtlichen Namen und einen bevorzugten Namen. 
- [ ] Namen bestehen nicht immer aus „Vorname + Nachname“.
- [ ] Manche Personen haben keinen Familiennamen; andere haben mehrere Namensteile oder mehrteilige Familiennamen.  
- [ ] Namen können sehr lang sein; verwende daher keine unrealistisch kurze maximale Zeichenlänge. 
- [ ] Namen können sich ändern, z. B. durch Heirat, persönliche Entscheidung oder andere Lebensereignisse. 
- [ ] Namen dürfen nicht als eindeutige ID verwendet werden, weil viele Personen denselben Namen haben können.  
- [ ] Namen können Sonderzeichen, Apostrophe, Bindestriche, Leerzeichen, Akzente und nicht-lateinische Schriften enthalten. ASCII reicht nicht aus. 
- [ ] Groß- und Kleinschreibung darf nicht automatisch „korrigiert“ werden. Sie kann Teil der gewünschten Namensschreibweise sein.  
- [ ] Namen nicht automatisch zerlegen oder aus dem letzten Wort eine Anrede wie „Herr/Frau Nachname“ ableiten. Das kann bei Namensreihenfolge, mehrteiligen Namen, Patronymen oder Suffixen falsch sein. 

#### B. Problemfälle bei Geschlecht und Anrede

- [ ] Nicht annehmen, dass alle Menschen ausschließlich männlich oder weiblich sind. 
- [ ] Nicht annehmen, dass Geschlecht immer unveränderlich oder eindeutig ist. 
- [ ] Nicht vom Aussehen, Namen oder der Stimme auf Geschlecht schließen. 
- [ ] Nicht annehmen, dass Geschlecht automatisch vorgibt, wie jemand angesprochen werden möchte. 
- [ ] Rechtliches Geschlecht, Geschlechtsidentität, Pronomen und gewünschte Anrede sind unterschiedliche Informationen und sollten nicht gleichgesetzt werden. 

### 3.3 Ergebnis der Recherche festhalten

- [ ] Erstelle im Forschungstagebuch eine Liste:  
  **„Meine 10 wichtigsten Risiken bei Formularen für Namen und Anreden“**.
- [ ] Schreibe zu jedem Risiko:
  - Was könnte schiefgehen?
  - Welche Personen wären betroffen?
  - Wie verhindert mein Entwurf das Problem?

---

## 4. Anforderungen an das gute Kontaktformular definieren

- [ ] Formuliere eine kurze Liste funktionaler Anforderungen, z. B.:
  - Kontaktanfrage absenden können.
  - Antwort-E-Mail an die angegebene E-Mail-Adresse.
  - Persönliche Anrede ermöglichen, ohne Geschlecht zu erraten.
  - Namen möglichst unverändert speichern.
  - Formular soll einfach bleiben.
  - Nutzer*innen sollen Felder überspringen können, die für die Anfrage nicht nötig sind.

- [ ] Formuliere Datenschutz- und Datensparsamkeitsregeln:
  - Geschlecht nicht abfragen, wenn es nur zur Anrede dienen soll.
  - Nur Informationen abfragen, die wirklich benötigt werden.
  - Die gewünschte Anrede ist optional.
  - Erkläre kurz, wofür das Feld verwendet wird.

---

## 5. Mindestens fünf unterschiedliche Formularansätze skizzieren

Erstelle die ersten Entwürfe auf Papier, digital oder in Figma/Adobe XD/HTML. Es werden mindestens **fünf unterschiedliche Herangehensweisen** verlangt. 

Für **jede** Variante solltest du dokumentieren:

- [ ] Welche Felder gibt es?
- [ ] Welche Felder sind Pflichtfelder?
- [ ] Wie wird die E-Mail-Anrede erzeugt?
- [ ] Was passiert, wenn kein Name oder keine Anrede angegeben wird?
- [ ] Welche Vorteile und Nachteile hat die Variante?
- [ ] Welche Problemfälle aus deiner Recherche löst sie bzw. löst sie nicht?

### Variante 1: Klassisch, aber problematisch

```text
Anrede: [Herr / Frau]
Vorname: [              ]
Nachname: [             ]
E-Mail: [               ]
Nachricht: [            ]
```

- [ ] Bewerte kritisch:
  - schließt Menschen aus,
  - zwingt die Struktur Vorname/Nachname auf,
  - leitet Anrede direkt aus Geschlecht ab,
  - eignet sich als Vergleich oder als bewusst schlechte Variante.

### Variante 2: Vollständiger Name + neutrale Standardanrede

```text
Name: [                                ]
E-Mail: [                              ]
Nachricht: [                           ]
```

- [ ] E-Mail-Regel:
  ```text
  Guten Tag [Name],
  ```
- [ ] Vorteil: sehr einfach und inklusiver.
- [ ] Nachteil: manche Personen möchten anders angesprochen werden.

### Variante 3: Name + bevorzugter Anzeigename

```text
Name für Buchung / Kontakt: [           ]
Wie dürfen wir Sie ansprechen? [        ]  (optional)
E-Mail: [                               ]
Nachricht: [                            ]
```

- [ ] E-Mail-Regel:
  - Wenn „Wie dürfen wir Sie ansprechen?“ ausgefüllt ist:
    ```text
    Guten Tag [Ansprechname],
    ```
  - Sonst:
    ```text
    Guten Tag,
    ```

### Variante 4: Frei formulierbare gewünschte Anrede

```text
Name: [                                 ]
Gewünschte Anrede in E-Mails: [         ]  (optional)
E-Mail: [                               ]
Nachricht: [                            ]
```

- [ ] Beispiele als Platzhalter:
  ```text
  z. B. „Guten Tag Alex Kim“, „Hallo Sam“, „Sehr geehrte Dr. Rivera“
  ```
- [ ] E-Mail-Regel:
  - Wenn die Person eine Anrede eingibt, verwende diese möglichst unverändert.
  - Sonst nutze „Guten Tag,“.

### Variante 5: Strukturierte Auswahl + freie Alternative

```text
Name: [                                 ]
Anrede für E-Mails: 
( ) Guten Tag [Name]
( ) Hallo [Name]
( ) Sehr geehrte*r [Name]
( ) Andere: [                           ]
( ) Keine persönliche Anrede gewünscht

E-Mail: [                               ]
Nachricht: [                            ]
```

- [ ] Vorteil: einfach für viele Personen, aber mit Freitext-Ausweg.
- [ ] Nachteil: Die Auswahl muss sorgfältig formuliert werden und darf keine Geschlechtszuordnung erzwingen.

### Variante 6: Beste Kandidatin – empfohlen

```text
Name, wie wir ihn verwenden dürfen: [                 ]
Wie möchten Sie in unserer Antwort angesprochen werden? [optional]
Beispiel: „Hallo Alex“, „Guten Tag M. Chen“, „Sehr geehrte Dr. Okafor“

E-Mail-Adresse: [                                      ]
Betreff: [                                             ]
Nachricht: [                                           ]

[ ] Ich stimme der Verarbeitung meiner Daten zur Bearbeitung
    meiner Anfrage zu.

[Absenden]
```

- [ ] Diese Variante ist wahrscheinlich am besten, weil:
  - der Name nicht künstlich in Vor- und Nachname aufgeteilt wird,
  - keine Geschlechtsangabe notwendig ist,
  - die Person selbst bestimmt, wie sie angesprochen werden möchte,
  - eine neutrale Alternative möglich bleibt,
  - die Komplexität für die meisten Menschen gering bleibt, aber bei Bedarf sichtbar wird. 

---

## 6. Beste Formularvariante auswählen und begründen

- [ ] Wähle eine deiner Varianten als endgültigen Entwurf.
- [ ] Schreibe eine Begründung in die Stundenliste und ins Forschungstagebuch.

### Mögliche Begründungsstruktur

1. **Einfachheit:** Das Formular enthält nur wenige, verständliche Felder.
2. **Inklusion:** Es setzt keine binäre Geschlechtsangabe voraus.
3. **Namensvielfalt:** Der Name wird als vollständige Eingabe behandelt und nicht automatisch in „Vorname“ und „Nachname“ zerlegt. 
4. **Selbstbestimmung:** Nutzer*innen bestimmen selbst ihre gewünschte E-Mail-Anrede.
5. **Fehlervermeidung:** Das System rät nicht anhand des Namens, welches Geschlecht oder welche Anrede passend sein könnte.
6. **Fallback:** Wenn keine gewünschte Anrede angegeben wird, verwendet das Hotel eine respektvolle neutrale Form.

---

## 7. Regeln für die automatische E-Mail-Anrede festlegen

Dokumentiere die Logik vollständig, damit Entwickler*innen sie umsetzen können. Diese vollständige Beschreibung mit Beispielen wird verlangt. 

### Empfohlene Datenfelder

| Feld | Pflicht? | Zweck |
|---|---:|---|
| `display_name` | ja oder optional, je nach Prozess | Name, wie das Hotel die Person nennen darf |
| `email_salutation` | optional | Gewünschte vollständige Anrede |
| `email` | ja | Antwortadresse |
| `message` | ja | Anfrage |
| `consent` | ja | Zustimmung zur Verarbeitung der Anfrage |

### Empfohlene Entscheidungslogik

```text
WENN email_salutation vorhanden UND nicht leer:
    Verwende email_salutation möglichst unverändert.
SONST WENN display_name vorhanden UND nicht leer:
    Verwende: "Guten Tag " + display_name + ","
SONST:
    Verwende: "Guten Tag,"
```

### Beispiele

| Eingabe „Name“ | Eingabe „Gewünschte Anrede“ | Ausgabe in der E-Mail |
|---|---|---|
| Alex Kim | Hallo Alex | Hallo Alex, |
| Dr. María de la Cruz | leer | Guten Tag Dr. María de la Cruz, |
| 王小明 | Guten Tag 王小明 | Guten Tag 王小明, |
| e e cummings | leer | Guten Tag e e cummings, |
| leer | leer | Guten Tag, |

### Wichtige Regeln

- [ ] Die gewünschte Anrede nicht automatisch verändern.
- [ ] Namen nicht automatisch großschreiben, kürzen, übersetzen oder „korrigieren“.
- [ ] Nicht aus dem Namen auf „Herr“, „Frau“ oder Pronomen schließen.
- [ ] Nicht den letzten Namensbestandteil als Nachnamen interpretieren.
- [ ] Immer einen neutralen Fallback anbieten: **„Guten Tag,“**.
- [ ] Bei Unsicherheit ist eine neutrale Anrede besser als eine falsche geschlechtliche Zuordnung.

---

## 8. Guten Formular-Prototyp erstellen

- [ ] Suche eine passende Hotel-Website.
- [ ] Mache einen Screenshot der Website.
- [ ] Gestalte dein Formular so, dass es visuell zu dieser Website passt.
- [ ] Verwende z. B. Figma, Adobe XD, PowerPoint/Google Slides oder HTML/CSS. 
- [ ] Mache Screenshots deines fertigen Prototyps.
- [ ] Dokumentiere:
  - Desktop-Ansicht,
  - optional Mobilansicht,
  - Fehlermeldung bei fehlender E-Mail-Adresse,
  - Beispiel einer ausgefüllten Version.

### Prüfliste für den guten Prototyp

- [ ] Gut lesbare Beschriftungen.
- [ ] Keine Pflichtfelder für Geschlecht, Titel oder Anrede.
- [ ] Keine Trennung in Vor- und Nachname notwendig.
- [ ] Hinweis bei optionaler Anrede, z. B.:
  > „Optional – damit wir Sie in unserer Antwort so ansprechen können, wie Sie es wünschen.“
- [ ] Name kann Unicode/Sonderzeichen enthalten.
- [ ] Lange Namen werden nicht abgeschnitten.
- [ ] Formular funktioniert auch ohne persönliche Anrede.

---

## 9. Cheat-Sheet für Entwickler*innen erstellen

Erstelle eine Seite oder zwei Seiten mit „Best Practices“.

### Vorschlag für den Inhalt

# Cheat-Sheet: Namen und Anreden in Formularen

## Do

- [ ] Speichere Namen als Unicode-Text.
- [ ] Erlaube Sonderzeichen, Akzente, Bindestriche, Apostrophe und Leerzeichen.
- [ ] Verwende möglichst ein Feld „Name“ oder „Name, wie wir Sie ansprechen dürfen“ statt einer erzwungenen Vorname/Nachname-Struktur.
- [ ] Bewahre Eingaben möglichst unverändert auf.
- [ ] Frage nach der gewünschten Anrede, wenn eine personalisierte Anrede wirklich erforderlich ist.
- [ ] Mache dieses Feld optional.
- [ ] Biete eine neutrale Fallback-Anrede an.
- [ ] Verwende eine technisch separate interne ID statt eines Namens als Identifikator.
- [ ] Verwende parametrisierte Datenbankabfragen.
- [ ] Escape bzw. kodiere Daten korrekt für HTML- und E-Mail-Ausgaben.

## Don’t

- [ ] Nicht automatisch „Herr“ oder „Frau“ aus einem Namen ableiten.
- [ ] Nicht verlangen, dass jede Person Vor- und Nachname eingibt.
- [ ] Nicht Namen auf ASCII beschränken. 
- [ ] Nicht Namen pauschal in Groß-/Kleinschreibung umwandeln.  
- [ ] Nicht Namen anhand des letzten Wortes zerlegen. 
- [ ] Keine Geschlechtsangabe verlangen, wenn sie für die Hotelanfrage nicht notwendig ist.
- [ ] Namen nicht als eindeutige Identifikationsnummer verwenden. 
- [ ] Keine SQL-Befehle durch String-Zusammenfügen erzeugen.

---

## 10. Fünf absichtlich schlechte Formulare entwickeln

Du sollst fünf Formulare erstellen, die bewusst schlecht funktionieren, und die Schwachstellen erklären. Mindestens eines muss SQL Injection zeigen; mindestens eines muss Vorname, Nachname und Anrede in einem Datenbankfeld speichern. 

> **Wichtig:** Diese schlechten Formulare nur als Demonstration in einem lokalen, nicht produktiven Umfeld erstellen. Keine echten Daten verwenden und keine unsicheren Formulare online veröffentlichen.

### Schlechtes Formular 1: Binäre Anrede + starre Namen

```text
Anrede: [Herr / Frau]
Vorname: [Pflichtfeld]
Nachname: [Pflichtfeld]
```

**Problem erklären:**
- Schließt nichtbinäre Personen aus.
- Nimmt an, dass alle Personen Vor- und Nachname haben.
- Leitet Anrede direkt aus Geschlecht ab.
- Ignoriert gewünschte Selbstbezeichnung.

---

### Schlechtes Formular 2: Nur ASCII und kurze Feldlänge

```text
First Name: [max. 15 Zeichen, nur A–Z]
Last Name:  [max. 15 Zeichen, nur A–Z]
```

**Problem erklären:**
- Schließt Namen mit Akzenten, Apostrophen, Bindestrichen oder nicht-lateinischen Zeichen aus.
- Schneidet lange Namen ab.
- Namen sind nicht auf ASCII begrenzt; viele Namen verwenden andere Schriften. 

---

### Schlechtes Formular 3: Automatische Anrede aus Name erraten

```text
Vorname: [                ]
```

**Fehlerhafte Logik:**

```text
Wenn Vorname auf „a“ endet → „Frau“
Sonst → „Herr“
```

**Problem erklären:**
- Namen geben kein verlässliches Geschlecht an.
- Funktioniert kulturübergreifend nicht.
- Kann Personen falsch oder verletzend ansprechen.
- Das Geschlecht einer Person ist nicht zuverlässig aus Erscheinung oder Namensannahmen ableitbar. 

---

### Schlechtes Formular 4: Alles in einem Datenbankfeld speichern

```text
Eingabe:
[Herr Max Mustermann________________]
```

**Fehlerhafte Datenbankstruktur:**

```text
customer_name = "Herr Max Mustermann"
```

**Problem erklären:**
- Anrede, Name und Namensbestandteile lassen sich später nicht zuverlässig trennen.
- Bei Änderung der Anrede oder des Namens muss der gesamte Text geändert werden.
- Die Daten sind nicht sauber strukturiert.
- Trotzdem soll man Namen nicht übermäßig automatisiert zerlegen: Besser sind getrennte Felder für **optionale gewünschte Anrede** und den **vollständigen Namen als Anzeigeinformation**.

---

### Schlechtes Formular 5: SQL-Injection-Demonstration

**Unsicheres Beispielprinzip:**

```text
SELECT * FROM contacts
WHERE email = '" + userInput + "';
```

**Problem erklären:**
- Wenn Eingaben direkt in SQL-Strings eingebaut werden, können sie Datenbankabfragen verändern.
- Angreifer*innen könnten unter Umständen Daten lesen, verändern oder Sicherheitsmechanismen umgehen.

**Sichere Alternative:**

```text
SELECT * FROM contacts WHERE email = ?;
```

- [ ] Erkläre: Statt String-Verkettung werden **parametrisierte Queries / Prepared Statements** verwendet.
- [ ] Zeige die Schwachstelle nur konzeptionell oder in einer isolierten Demo-Datenbank.
- [ ] Verwende keine produktiven Zugangsdaten und keine echten personenbezogenen Daten.

---

## 11. Testfälle für das gute Formular erstellen

- [ ] Teste mindestens diese Fälle:

| Testfall | Erwartetes Ergebnis |
|---|---|
| Name mit Apostroph, z. B. O’Hara | Wird akzeptiert und unverändert angezeigt |
| Name mit Bindestrich, z. B. Jean-Pierre | Wird akzeptiert |
| Mehrteiliger Name, z. B. de la Cruz | Wird nicht automatisch zerlegt |
| Name in anderer Schrift, z. B. 王小明 | Wird gespeichert und angezeigt |
| Name mit Kleinbuchstaben, z. B. e e cummings | Keine automatische Korrektur |
| Sehr langer Name | Kein Abschneiden oder sinnvolle große Grenze |
| Keine gewünschte Anrede | E-Mail beginnt mit „Guten Tag,“ |
| Individuelle Anrede | Wird genau bzw. sicher verwendet |
| Name ohne Familienname | Formular kann trotzdem abgeschickt werden |
| Nichtbinäre Person | Keine binäre Geschlechtsauswahl notwendig |
| Eingabe mit HTML-Zeichen | Sicher ausgegeben, kein XSS/HTML-Injection |
| Eingabe mit SQL-Sonderzeichen | Keine Veränderung der Datenbankabfrage |

- [ ] Halte Testergebnisse mit Screenshots fest.

---

## 12. Präsentation für das Hotel vorbereiten

Die Präsentation soll erklären, warum die Lösung notwendig ist und wie sie funktioniert. Die Abgabe soll als PDF exportiert werden, wobei Slide und Erklärungstext gemeinsam auf einer Seite stehen. 

### Mögliche Gliederung der Präsentation

1. **Titel:** Inklusives Hotel-Kontaktformular
2. **Ausgangsproblem:** Automatische E-Mails sollen respektvoll sein.
3. **Warum Namen komplex sind:** Nicht jede Person hat Vorname + Nachname; Namen können unterschiedlich geschrieben sein.
4. **Warum Geschlecht und Anrede getrennt werden müssen:** Nicht raten, sondern nach Wunsch fragen.
5. **Anforderungen an unsere Lösung**
6. **Die fünf Formularvarianten**
7. **Unsere ausgewählte Lösung**
8. **Formular-Screenshot / Prototyp**
9. **Regeln für die automatische E-Mail-Anrede**
10. **Beispiele für generierte E-Mails**
11. **Technische Best Practices / Cheat-Sheet**
12. **Fünf schlechte Formulare und ihre Risiken**
13. **Fazit und Nutzen für das Hotel**

- [ ] Ergänze unter jeder Folie Erklärungstext bzw. Sprecher*innen-Notizen.
- [ ] Exportiere alles als PDF im verlangten Format.

---

## 13. Reflexion und Feedback schreiben

Beantworte die vorgegebenen Reflexionsfragen, zum Beispiel:

- [ ] Hat sich dein Verständnis von „Computational Thinking“ bzw. verantwortungsvoller Systemgestaltung verändert?
- [ ] Welche Teile waren schwierig?
- [ ] Welche Teile waren einfach?
- [ ] Was hat dir gefallen?
- [ ] Was würdest du an der Aufgabe ändern?
- [ ] Was hast du gelernt?
- [ ] Haben Reviews dir geholfen?
- [ ] Bist du mit deiner Arbeit zufrieden?

Diese Reflexion wird laut Aufgabenbeschreibung nicht bewertet, ist aber Teil der Endabgabe. 

---

## 14. Endkontrolle vor der Abgabe

### Inhalt

- [ ] Recherche zu Namen und Geschlecht dokumentiert.
- [ ] Wichtigste Problemfälle priorisiert.
- [ ] Mindestens fünf unterschiedliche Formularentwürfe vorhanden.
- [ ] Beste Variante nachvollziehbar begründet.
- [ ] Guter Formular-Prototyp erstellt.
- [ ] Screenshots vorhanden.
- [ ] Vollständige Regeln zur Erzeugung der E-Mail-Anrede vorhanden.
- [ ] Konkrete Beispiele für E-Mail-Anreden vorhanden.
- [ ] Cheat-Sheet für Entwickler*innen fertig.
- [ ] Fünf schlechte Formulare erstellt und erklärt.
- [ ] SQL-Injection-Beispiel enthalten.
- [ ] Beispiel mit gemeinsamer Speicherung von Anrede, Vorname und Nachname in einem DB-Feld enthalten.
- [ ] Präsentation als PDF exportiert.
- [ ] Stundenliste vollständig.
- [ ] Forschungstagebuch vollständig.
- [ ] Reflexion & Feedback geschrieben.

### Qualität

- [ ] Keine Anrede wird aus Namen oder vermutetem Geschlecht erraten.
- [ ] Keine unnötige Geschlechtsabfrage.
- [ ] Kein Zwang zu „Vorname“ und „Nachname“.
- [ ] Neutrale Fallback-Anrede ist definiert.
- [ ] Namen werden möglichst originalgetreu behandelt.
- [ ] Datenschutz und sichere Verarbeitung wurden berücksichtigt.
- [ ] Alle Dateien sind verständlich benannt und im Abgabeordner.