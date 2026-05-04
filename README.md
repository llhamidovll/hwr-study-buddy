# HWR Study Buddy

## 1. Projektüberblick

**HWR Study Buddy** ist eine zweiseitige Web-Plattform für Studierende der HWR Berlin.

Die Plattform verbindet Studierende, die Unterstützung in bestimmten Modulen benötigen, mit Studierenden, die Nachhilfe oder Lernunterstützung anbieten möchten.

Studierende können nach passenden Tutorinnen und Tutoren suchen, Tutorprofile ansehen und Lernanfragen senden. Tutorinnen und Tutoren können ein eigenes Profil erstellen, unterstützte Module angeben und eingehende Anfragen verwalten.

Das Projekt wird als Solo-Projekt umgesetzt.

---

## 2. Team Composition

**Teamname:** HWR Study Buddy  
**Projektart:** Solo-Projekt / Ein-Personen-Team

| Name | Rolle | Beitrag |
|---|---|---|
| Abdulhamid Suliman | Full Project Responsibility | Projektidee, Value Proposition, Target Scope, UI-Wireframes, Implementierung und Dokumentation |

**Repository:**  
https://github.com/llhamidovll/hwr-study-buddy.git

Das Repository kann vom Prüfer mit folgendem Befehl geklont werden:

```bash
gh repo clone llhamidovll/hwr-study-buddy
```

Alternativ:

```bash
git clone https://github.com/llhamidovll/hwr-study-buddy.git
```

---

## 3. Meta-Goals per Contributor

| Name | Zielnote | Persönliche Ziele |
|---|---|---|
| Abdulhamid Suliman | 2.0 | Ich möchte den vollständigen Entwicklungsprozess einer Flask-basierten Webanwendung verstehen. Dabei möchte ich insbesondere Flask, Jinja2, SQLite, Login/Registrierung, User Roles, Authorization und eine saubere Projektstruktur praktisch anwenden. Da ich das Projekt alleine bearbeite, ist mein Ziel, den Umfang realistisch zu halten und einen klaren Happy Path von der Registrierung bis zur Verwaltung von Lernanfragen umzusetzen. |

---

## 4. Value Proposition

### Zielnutzer

Die Zielnutzer sind Studierende der HWR Berlin.

Die Plattform richtet sich an zwei Nutzergruppen:

1. Studierende, die Unterstützung in bestimmten Modulen benötigen.
2. Studierende, die als Tutorinnen oder Tutoren Lernunterstützung anbieten möchten.

Beispielhafte Module sind:

- Programming
- Databases
- Accounting
- Statistics
- Web Development

---

### Problem

Viele Studierende haben Schwierigkeiten in einzelnen Modulen und suchen gezielte Unterstützung. Die Suche nach Hilfe erfolgt jedoch häufig unstrukturiert über private Kontakte, WhatsApp-Gruppen oder zufällige Empfehlungen.

Dadurch ist es schwierig, schnell eine passende Person zu finden, die:

- das konkrete Modul kennt,
- bei einem bestimmten Thema helfen kann,
- auf Deutsch oder Englisch unterstützen kann,
- zeitlich verfügbar ist,
- und bereit ist, Lernhilfe anzubieten.

Besonders bei anspruchsvollen Modulen wie Programming, Databases, Accounting, Statistics oder Web Development kann passende Unterstützung den Lernprozess deutlich erleichtern.

---

### Warum dieses Projekt sinnvoll ist

Ich kenne das Problem selbst aus dem Studium. Gleichzeitig sehe ich, dass Studierende oft Unterstützung suchen, aber keine strukturierte Plattform dafür haben.

HWR Study Buddy passt direkt zum Studienalltag, weil die Plattform ein konkretes Problem innerhalb der Hochschule adressiert: Studierende sollen leichter passende Lernhilfe für konkrete Module finden können.

---

### Lösung

**HWR Study Buddy** bietet eine strukturierte Web-App, über die Studierende passende Lernunterstützung für HWR-Module finden können.

Studierende, die Hilfe suchen, können nach Tutorinnen und Tutoren suchen, Profile ansehen und eine Lernanfrage senden. Tutorinnen und Tutoren können ein Profil erstellen, unterstützte Module angeben und eingehende Anfragen annehmen oder ablehnen.

---

## 5. Two-Sided Platform

HWR Study Buddy ist eine zweiseitige Plattform, weil sie zwei verschiedene Nutzergruppen miteinander verbindet, die gegenseitig voneinander profitieren.

| Seite A | Seite B | Interaktion |
|---|---|---|
| Studierende, die Hilfe suchen | Studentische Tutorinnen und Tutoren | Studierende suchen Tutorinnen/Tutoren und senden Lernanfragen |
| Studentische Tutorinnen und Tutoren | Studierende, die Hilfe suchen | Tutorinnen/Tutoren erhalten Anfragen und können diese annehmen oder ablehnen |

Der Wert der Plattform steigt, wenn beide Seiten teilnehmen:

- Studierende profitieren von mehr verfügbaren Tutorinnen und Tutoren.
- Tutorinnen und Tutoren profitieren von mehr passenden und gezielten Anfragen.
- Die Plattform wird nützlicher, je mehr passende Profile und Anfragen vorhanden sind.

---

## 6. Geschäftslogik / Bezahlmodell

Das Projekt konzentriert sich im MVP nicht auf Online-Zahlungen.

Tutorinnen und Tutoren können in ihrem Profil optional angeben, ob sie Unterstützung kostenlos, freiwillig oder gegen einen kleinen Betrag anbieten.

Die eigentliche Bezahlung ist nicht Teil des technischen MVPs. Dadurch bleibt der Umfang realistisch und die App konzentriert sich auf die zentrale Plattformfunktion: passende Lernhilfe finden und Anfragen verwalten.

Mögliche Preisstatus im Tutorprofil:

- free
- voluntary
- paid

---

## 7. Target Scope

Die erste Version der Anwendung konzentriert sich auf einen einfachen und realistischen Happy Path.

### Geplante Kernfunktionen

1. Registrierung und Login
2. Auswahl einer Rolle: Student oder Tutor
3. Tutorprofil erstellen
4. Tutorensuche nach Modul
5. Filter nach Modul, Sprache, Verfügbarkeit, Preisstatus und Online/Vor-Ort
6. Tutor-Detailseite anzeigen
7. Lernanfrage senden
8. Student-Dashboard für gesendete Anfragen
9. Tutor-Dashboard für eingehende Anfragen
10. Anfrage-Status: pending, accepted, rejected

---

## 8. MVP-Fokus

Der MVP fokussiert sich auf Matching und Request Management.

Nicht Teil des MVPs sind:

- Online-Payment
- Chat-System
- Video-Meetings
- automatische Terminbuchung
- Bewertungen oder Ratings

Diese Funktionen können später ergänzt werden, sind aber für die erste Version bewusst nicht vorgesehen.

---

## 9. Rollenmodell

In der ersten Version wählt ein Nutzer bei der Registrierung eine Rolle:

- Student: sucht Unterstützung
- Tutor: bietet Unterstützung an

Für eine spätere Version kann erweitert werden, dass ein Nutzer beide Rollen gleichzeitig haben kann. Zum Beispiel könnte ein Student Unterstützung in Accounting suchen, aber gleichzeitig Nachhilfe in Programming anbieten.

---

## 10. UI-Scribbles / Textual Wireframes

Da die Anwendung noch nicht implementiert ist, zeigen die folgenden textuellen Wireframes den geplanten visuellen Umfang der Web-App.

Diese Wireframes dienen als Target Scope und zeigen, welche Screens für den MVP geplant sind.

---

### Screen 1: Landing Page

**Zweck:** Die Plattform kurz erklären und Nutzer zur Registrierung oder Anmeldung führen.

```text
+------------------------------------------------------+
| HWR Study Buddy                                      |
|------------------------------------------------------|
| Find help for your HWR modules                       |
|                                                      |
| Connect with student tutors for Programming,         |
| Databases, Accounting, Statistics and Web Development|
|                                                      |
| [ Tutor finden ]        [ Tutor werden ]             |
|                                                      |
| Login | Register                                     |
+------------------------------------------------------+
```

Wichtige Elemente:

- App-Name
- Kurze Beschreibung
- Button: Tutor finden
- Button: Tutor werden
- Login/Register-Link

---

### Screen 2: Registrierung / Login

**Zweck:** Nutzer können ein Konto erstellen oder sich anmelden.

```text
+------------------------------------------------------+
| Register                                             |
|------------------------------------------------------|
| E-Mail:        [                               ]      |
| Password:      [                               ]      |
|                                                      |
| Rolle auswählen:                                    |
| ( ) Ich suche Hilfe                                  |
| ( ) Ich biete Nachhilfe an                           |
|                                                      |
| [ Registrieren ]                                     |
|                                                      |
| Already have an account? Login                       |
+------------------------------------------------------+
```

Wichtige Elemente:

- E-Mail
- Passwort
- Rollenauswahl
- Registrieren-Button
- Login-Link

---

### Screen 3: Tutorensuche

**Zweck:** Studierende können passende Tutorinnen und Tutoren suchen.

```text
+------------------------------------------------------+
| Tutorensuche                                         |
|------------------------------------------------------|
| Suche: [ Programming                         ]        |
|                                                      |
| Filter:                                              |
| Modul:        [ Programming v ]                      |
| Sprache:      [ Deutsch v ]                          |
| Verfügbar:    [ This week v ]                        |
| Preisstatus:  [ free / voluntary / paid v ]          |
| Ort:          [ online / vor Ort v ]                 |
|                                                      |
|------------------------------------------------------|
| Tutor Card                                           |
| Name: Sara M.                                        |
| Modul: Programming                                   |
| Sprache: Deutsch, Englisch                           |
| Preisstatus: voluntary                               |
| [ Profil ansehen ]                                   |
|------------------------------------------------------|
| Tutor Card                                           |
| Name: Max K.                                         |
| Modul: Databases                                     |
| Sprache: Deutsch                                     |
| Preisstatus: paid                                    |
| [ Profil ansehen ]                                   |
+------------------------------------------------------+
```

Wichtige Elemente:

- Suchfeld
- Filter nach Modul
- Filter nach Sprache
- Filter nach Verfügbarkeit
- Filter nach Preisstatus
- Filter nach online/vor Ort
- Tutor-Karten
- Button: Profil ansehen

---

### Screen 4: Tutorprofil

**Zweck:** Detailinformationen zu einer Tutorin oder einem Tutor anzeigen.

```text
+------------------------------------------------------+
| Tutorprofil                                          |
|------------------------------------------------------|
| Name: Sara M.                                        |
|                                                      |
| Unterstützte Module:                                 |
| - Programming                                        |
| - Web Development                                    |
|                                                      |
| Sprache: Deutsch, Englisch                           |
| Verfügbarkeit: Mittwoch und Freitag                  |
| Ort: online oder vor Ort                             |
| Preisstatus: voluntary                               |
|                                                      |
| Beschreibung:                                        |
| I can help with Python basics, Flask routing,        |
| templates and small web app exercises.               |
|                                                      |
| [ Anfrage senden ]                                   |
+------------------------------------------------------+
```

Wichtige Elemente:

- Name
- Unterstützte Module
- Beschreibung
- Sprache
- Verfügbarkeit
- Online/vor Ort
- Preisstatus
- Button: Anfrage senden

---

### Screen 5: Lernanfrage senden

**Zweck:** Studierende senden eine Anfrage an eine Tutorin oder einen Tutor.

```text
+------------------------------------------------------+
| Lernanfrage senden                                   |
|------------------------------------------------------|
| Tutor: Sara M.                                       |
|                                                      |
| Modul:                                               |
| [ Programming v ]                                    |
|                                                      |
| Thema / Problem:                                     |
| [ Flask routes and templates                  ]      |
|                                                      |
| Gewünschter Zeitraum:                                |
| [ Friday afternoon                            ]      |
|                                                      |
| Nachricht:                                           |
| [ Hi, I need help understanding Flask routes   ]      |
| [ and how templates are rendered with Jinja2.  ]      |
|                                                      |
| [ Anfrage absenden ]                                 |
+------------------------------------------------------+
```

Wichtige Elemente:

- Ausgewählter Tutor
- Modul
- Thema / Problem
- gewünschter Zeitraum
- Nachricht
- Button: Anfrage absenden

---

### Screen 6: Student-Dashboard

**Zweck:** Studierende sehen ihre gesendeten Anfragen und deren Status.

```text
+------------------------------------------------------+
| Student-Dashboard                                    |
|------------------------------------------------------|
| Meine gesendeten Anfragen                            |
|                                                      |
|------------------------------------------------------|
| Tutor: Sara M.                                       |
| Modul: Programming                                   |
| Thema: Flask routes                                  |
| Status: pending                                      |
|------------------------------------------------------|
| Tutor: Max K.                                        |
| Modul: Databases                                     |
| Thema: SQL joins                                     |
| Status: accepted                                     |
|------------------------------------------------------|
| Tutor: Anna B.                                       |
| Modul: Accounting                                    |
| Thema: BAB calculation                               |
| Status: rejected                                     |
+------------------------------------------------------+
```

Wichtige Elemente:

- Liste der gesendeten Anfragen
- Tutorname
- Modul
- Thema
- Status: pending, accepted, rejected

---

### Screen 7: Tutor-Dashboard

**Zweck:** Tutorinnen und Tutoren verwalten eingehende Anfragen.

```text
+------------------------------------------------------+
| Tutor-Dashboard                                      |
|------------------------------------------------------|
| Eingehende Anfragen                                  |
|                                                      |
|------------------------------------------------------|
| Student: Abdul                                       |
| Modul: Programming                                   |
| Thema: Flask routes and templates                    |
| Nachricht: I need help understanding Flask routes.   |
|                                                      |
| [ Annehmen ]        [ Ablehnen ]                     |
|------------------------------------------------------|
| Student: Maria                                       |
| Modul: Statistics                                    |
| Thema: Hypothesis testing                            |
| Nachricht: I need help preparing for the exam.       |
|                                                      |
| [ Annehmen ]        [ Ablehnen ]                     |
+------------------------------------------------------+
```

Wichtige Elemente:

- Liste der eingehenden Anfragen
- Name des Studierenden
- Modul
- Thema
- Nachricht
- Button: Annehmen
- Button: Ablehnen

---

## 11. Happy Path

Der zentrale Happy Path der Anwendung ist:

1. Ein Student registriert sich.
2. Der Student wählt die Rolle „Ich suche Hilfe“.
3. Der Student sucht nach einem Tutor für ein bestimmtes Modul.
4. Der Student filtert nach Modul, Sprache, Verfügbarkeit, Preisstatus oder Online/Vor-Ort.
5. Der Student öffnet ein Tutorprofil.
6. Der Student sendet eine Lernanfrage.
7. Der Tutor loggt sich ein.
8. Der Tutor sieht die eingehende Anfrage im Tutor-Dashboard.
9. Der Tutor nimmt die Anfrage an oder lehnt sie ab.
10. Der Student sieht den aktualisierten Status im Student-Dashboard.

---

## 12. Planned Data Model

Für die spätere Umsetzung ist folgendes vereinfachtes Datenmodell geplant.

### users

Speichert registrierte Nutzer.

Mögliche Felder:

- id
- name
- email
- password_hash
- role

### tutor_profiles

Speichert zusätzliche Informationen für Tutorinnen und Tutoren.

Mögliche Felder:

- id
- user_id
- description
- languages
- availability
- location_mode
- price_status

### modules

Speichert unterstützte Module.

Mögliche Felder:

- id
- name

Beispielwerte:

- Programming
- Databases
- Accounting
- Statistics
- Web Development

### tutoring_requests

Speichert Lernanfragen von Studierenden an Tutorinnen und Tutoren.

Mögliche Felder:

- id
- student_id
- tutor_id
- module_id
- topic
- message
- preferred_time
- status

Mögliche Statuswerte:

- pending
- accepted
- rejected

---

## 13. Geplanter Technology Stack

Der geplante Technology Stack ist:

- Python
- Flask
- Jinja2
- SQLite
- HTML
- CSS

Die Anwendung soll lokal auf einem aktuellen Windows- oder macOS-System ausführbar sein.

---

## 14. AI Usage Disclosure

Für die Erstellung dieser ersten Projektbeschreibung habe ich ChatGPT als unterstützendes Werkzeug verwendet.

Die KI wurde verwendet für:

- Brainstorming zur Projektidee
- Strukturierung der README
- Formulierung der Value Proposition
- Ausarbeitung des Target Scopes
- Erstellung der textuellen UI-Wireframes

Ich habe die Inhalte geprüft, angepasst und stelle sicher, dass ich die eingereichten Inhalte erklären kann.

Es wurde keine Agentic AI verwendet. Es wurden keine Dateien, Commits oder Repository-Strukturen automatisiert durch KI erstellt.
---

## 15. Quellen / References

- HWR Berlin – Full-Stack Web Development Assessment: https://hwrberlin.github.io/fswd/assessment.html
- GitHub Docs – About READMEs: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes
