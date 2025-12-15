## 💼 **Projektübersicht**

Ich entwickle Software, die **funktioniert**, **verständlich bleibt** und **langfristig stabil läuft**.
Mein Schwerpunkt liegt in der **Backend- und Systementwicklung mit PHP, MySQL und JavaScript**, ergänzt durch moderne Webtechnologien wie **Smarty, jQuery, Bootstrap und DataTables**.

In den letzten Jahren habe ich bei der **Aspeo GmbH** verschiedene Systeme aufgebaut. Von **mandantenfähigen Plattformen** über **E-Rechnungstools** bis zu **automatisierten Import- und Monitoring-Lösungen**.
Alle Projekte verbindet ein Ziel: **Prozesse automatisieren, Fehlerquellen minimieren und nachhaltige Strukturen schaffen.**

Die folgenden Projekte zeigen, wie ich komplexe Anforderungen in saubere, wartbare und sichere Softwarelösungen übersetze.

---

## 🛡️ **Benutzermanagement & Mandanten-Hierarchie**

**📅 Zeitraum:** [Aktuell]
**🏢 Projekt:** System-Architektur

### 🎯 Ausgangssituation

Es wurde eine strukturierte Verwaltungsebene für Benutzer und Firmen benötigt, die eine strikte hierarchische Trennung von Zugriffsrechten und Daten gewährleistet. Ziel war es, unterschiedliche Sichtbarkeiten und Verwaltungsbefugnisse für globale Administratoren, Firmen-Admins und Endbenutzer zu etablieren.

### 💡 Aufgabe

Entwicklung eines differenzierten **Benutzer- und Mandantenmanagements**, das rollenbasierte Dashboards, spezifische CRUD-Rechte und eine mandantenabhängige Konfiguration (z. B. für LLM-Hosts und Token-Preise) bereitstellt.

### 🧠 Vorgehen

## Rollenkonzept

- **Superadmin**  
  Vollzugriff auf systemweite Daten, Firmen und Auswertungen.  
  Bereitstellung von Auswahl- und Filterfunktionen für Firmen.

- **Admin**  
  Zugriff und Bearbeitungsrechte beschränkt auf den eigenen Zuständigkeitsbereich.  

- **Benutzer**  
  Zugriff ausschließlich auf eigene, zugeordnete Daten.

## Datenbank & Konfiguration

- Erweiterung um erforderliche Parameter.
- Abbildung mandantenspezifischer Konfigurationen.
- Anpassung bestehender Systemkonfigurationen.

## Dashboard & Statistiken

- Bereitstellung statistischer Auswertungen:
  - Letzte 30 Tage
  - Letzter Monat
  - Aktueller Monat
- Rollenabhängige Aufbereitung der Daten:
  - Superadmin: systemweit
  - Admin: firmenspezifisch
  - Benutzer: personenbezogen

## Menüstruktur & Funktionen

- Dynamischer Aufbau der Hauptmenüpunkte abhängig von der Rolle:
  - **Superadmin**: Statistik, Benutzerverwaltung, Firmenverwaltung
  - **Admin**: Statistik, Benutzerverwaltung
  - **Benutzer**: Statistik
- Integration grundlegender Profilfunktionen (z. B. Passwortänderung).


### 📈 Ergebnis

Ein hierarchisches Verwaltungssystem, das eine saubere Mandantentrennung sicherstellt. Es ermöglicht Superadmins die globale Steuerung, während Company-Admins ihre Einheiten eigenständig verwalten können, ohne Zugriff auf fremde Daten zu erhalten.

### 🛠️ Technologien

`PHP` · `MySQL` · `User Role Management` · `Mandantenfähigkeit` · `Backend Architecture` · `Statistik-Module`

---

## 🏗️ **Bild- und PDF-Export-App für Immobiliengutachten**

**📅 Zeitraum:** Nov 2025 – Heute
**🏢 Unternehmen:** Aspeo GmbH

### 🎯 Ausgangssituation

Für die Erstellung von Immobiliengutachten mussten Bildmaterialien bislang manuell gesammelt, beschrieben und separat in PDF-Dokumente eingefügt werden.
Dieser Prozess war **zeitaufwendig**, **fehleranfällig** und **nicht standardisiert**.

### 💡 Aufgabe

Entwicklung einer **webbasierten Anwendung**, mit der Mitarbeitende Bildmaterial zentral verwalten, sortieren und direkt als formatiertes PDF exportieren können.
Ziel war eine **einfache Benutzerführung** und die **spätere Mandantenfähigkeit** des Systems.

### 🧠 Vorgehen

* Entwicklung der **Projekt- und Bildverwaltung** (PHP, MySQL, Smarty Framework)
* Implementierung von **Upload- und Sortierfunktionen** (Dropzone, jQuery UI Sortable)
* Aufbau der **PDF-Export-Logik** inkl. Vorlagen- und Spracheinstellungen
* Entwicklung eines **rollenbasierten Login-Systems** mit Benutzer- und Vorlagenverwaltung
* Erstellung dynamischer **Projektlisten** (DataTables) inkl. Filter- und Exportfunktionen
* Aufbau konfigurierbarer **Systemeinstellungen** (Labeltexte, Standardwerte, Sprache, Mandantenspezifika)

### 📈 Ergebnis

Die Anwendung ermöglicht eine **effiziente Erstellung und Verwaltung** von bildbasierten Gutachtenanhängen.
Sie befindet sich aktuell im **Pilotbetrieb** und wird kontinuierlich weiterentwickelt, um zukünftig **mandantenfähig ausgerollt** zu werden.

### 🛠️ Technologien

`PHP` · `MySQL` · `Smarty` · `User Role Management` · `jQuery` · `Bootstrap` · `DataTables`

---
## ⚙️ **Vermarkter-Backend – Abrechnungssystem für das Recruiting Tool**

**📅 Zeitraum:** Jan 2025 – Heute
**🏢 Unternehmen:** Aspeo GmbH

### 🎯 Ausgangssituation

Das bestehende Recruiting Tool war ursprünglich als **Einzelinstanz** konzipiert.
Mit zunehmender Nutzung entstand der Bedarf, das System **mandantenfähig** zu gestalten, um mehrere Kunden parallel betreuen und **Vermarkter automatisiert abrechnen** zu können.
Eine skalierbare Backend-Struktur existierte zu diesem Zeitpunkt noch nicht.

### 💡 Aufgabe

Konzeption und Entwicklung eines eigenständigen **Backend-Systems**, das neue Kundeninstanzen automatisch anlegt, Subdomains erzeugt und ein mehrstufiges Abrechnungs- sowie Berechtigungssystem für Vermarkter bereitstellt.

### 🧠 Vorgehen

* Aufbau der **Backend-Architektur** mit PHP, MySQL und Smarty Framework
* Implementierung eines **rollenbasierten Berechtigungssystems** *(User Role Management)*
* Automatische Erstellung neuer **Kundendatenbanken** inkl. Subdomain-Generierung
* Entwicklung einer **Abrechnungslogik** für Vermarkter mit mehrstufigem Provisionsmodell
* Integration von **DataTables** zur Verwaltung und Auswertung von Buchungs- und Rechnungsdaten
* **Anbindung an bestehende Systeme** wie das Recruiting Tool und das Shootout-Modul

### 📈 Ergebnis

Das neue Backend bildet die **technische Grundlage der Multi-Tenant-Struktur** des Recruiting Tools.
Es ermöglicht die **vollautomatische Verwaltung neuer Mandanten**, die **Subdomain-Erstellung** und die **Abrechnung von Vermarktern** über ein skalierbares, zentrales System.
Der Rollout erfolgt schrittweise parallel mit dem Hauptsystem.

### 🛠️ Technologien

`PHP` · `MySQL` · `Smarty` · `Backend & Frontend Development` · `Prozessautomatisierung` · `User Role Management` · `jQuery` · `Bootstrap` · `DataTables`

---

## 🧩 **Recruiting Tool – Bewerberverwaltung & Matching-System**

**📅 Zeitraum:** Jan 2024 – Heute
**🏢 Unternehmen:** Aspeo GmbH

### 🎯 Ausgangssituation

Im Recruiting-Prozess fehlte eine **zentrale, skalierbare Lösung**, um Kandidaten, Unternehmen und Vermarkter effizient zu verwalten und zusammenzuführen.
Bestehende Systeme waren **nicht mandantenfähig** und boten keine flexible Automatisierung für **Matching-, Abrechnungs- oder Kampagnenprozesse**.

### 💡 Aufgabe

Konzeption und Entwicklung eines **mandantenfähigen Recruiting-Systems**, das Bewerberdaten zentral verarbeitet, automatisierte Zuordnungen ermöglicht und gleichzeitig alle **Datenschutz- und Rechteanforderungen** erfüllt.

### 🧠 Vorgehen

* Entwicklung der kompletten **Backend-Logik** (PHP, MySQL, Smarty Framework)
* Aufbau einer **Multi-Tenant-Architektur** mit automatischer Mandanten- und Datenbankanlage
* Implementierung eines **rollenbasierten Berechtigungssystems** *(User Role Management)*
* Entwicklung des **Matching-Systems** zur automatisierten Zuordnung von Kandidaten und Stellenprofilen
* Integration eines **Kampagnenmoduls** für E-Mail- und CRM-basierte Ansprache
* **Anbindung externer Systeme**, u. a. Salesforce-API für Kampagnen- und Benutzerimporte
* Aufbau von **Import- und Exportfunktionen** (Excel, CSV, JSON) zur Massenverarbeitung
* Entwicklung einer **rollenabhängigen Benutzeroberfläche** für Recruiter, Administratoren und Vermarkter
* Implementierung von **DSGVO-konformen Prozessen** (Opt-in, Tracking, Lösch- und Rechteverwaltung)
* Nutzung von **DataTables und jQuery** für performante, filterbare Übersichten

### 📈 Ergebnis

Das Recruiting Tool ist **produktiv im Einsatz** bei mehreren Kunden und bildet die Grundlage für eine **skalierbare Multi-Tenant-Plattform**.
Es automatisiert Matching-, Reporting- und Abrechnungsprozesse, reduziert den manuellen Aufwand erheblich und ermöglicht den geplanten Ausbau um zusätzliche Module wie das Vermarkter-Backend.

### 🛠️ Technologien

`PHP` · `MySQL` · `JavaScript` · `Prozessautomatisierung` · `User Role Management`

---

## 🧱 **Office Add-in – Microsoft Word Plugin mit Webfrontend**

**📅 Zeitraum:** Juli 2025 – Sept 2025
**🏢 Unternehmen:** Aspeo GmbH

### 🎯 Ausgangssituation

Ein Kunde benötigte ein **Microsoft Word Add-in**, um interne Dokumentenprozesse zu automatisieren und Arbeitsabläufe direkt in Word zu integrieren.
Dafür musste ein eigenständiges, webbasiertes **Frontend** entwickelt werden, das alle erforderlichen Funktionen und UI-Komponenten für das Add-in bereitstellt.

### 💡 Aufgabe

Entwicklung des **kompletten Frontends** für das Microsoft Office Add-in.
Ziel war eine **klare Benutzeroberfläche**, eine **logische Struktur** und die technische Vorbereitung für die spätere Integration in Word.

### 🧠 Vorgehen

* Umsetzung der **Benutzeroberfläche** mit HTML, JavaScript und Bootstrap
* Vorbereitung der **Frontend-Funktionen** für die API-Anbindung
* Entwicklung **interaktiver Formulare und Komponenten** für die Office-Integration
* Abstimmung der UI-Struktur mit dem **Backend-Team** für die spätere Dateneinbindung
* Sicherstellung von **Responsivität** und stabiler Darstellung innerhalb der Office-Umgebung

### 📈 Ergebnis

Das entwickelte Frontend bildet die **Grundlage für das Word Add-in** und ermöglicht eine **nahtlose Einbindung** der geplanten Funktionen in die Microsoft Office-Oberfläche.
Der Fokus lag auf **klarer Struktur**, **intuitiver Bedienung** und einer **technisch sauberen Vorbereitung** für die spätere Backend-Integration.

### 🛠️ Technologien

`JavaScript` · `UX/UI` · `Frontend-Entwicklung` · `Bootstrap` · `jQuery`

---

## 🗃️ **Jobdatenbank & Import-System – Automatisierte Datengrundlage für spätere Recruiting-Plattform**

**📅 Zeitraum:** Jan 2024 – Juni 2025
**🏢 Unternehmen:** Aspeo GmbH

### 🎯 Ausgangssituation

Vor dem Aufbau des heutigen Recruiting Tools bestand die Anforderung, eine **zentrale Jobdatenbank** zu entwickeln, die Stellenanzeigen automatisiert sammelt, analysiert und in strukturierter Form bereitstellt.
Ziel war es, aus diesen Jobdaten **Unternehmen und Kontakte zu generieren** – als Basis für künftige Recruiting- und Matching-Prozesse.

### 💡 Aufgabe

Konzeption und Entwicklung eines **mehrstufigen Import- und Verarbeitungssystems**, das über Jobcrawler täglich neue Jobs importiert, prüft, validiert und daraus automatisch Unternehmens- und Kontaktdatensätze erstellt.

### 🧠 Vorgehen

* Entwicklung der **Cronjob-Logik** zur täglichen Verarbeitung und Aktualisierung der Jobdaten
* Aufbau **dynamischer Datenbankverbindungen** zur Verwaltung mehrerer Mandanten
* Implementierung von **Import-, Validierungs- und Duplikatserkennungsroutinen**
* Automatische Erstellung von **Unternehmens- und Kontaktdatensätzen** aus Jobinformationen
* Aufbau eines webbasierten **Dashboards** (PHP, Smarty, jQuery, DataTables) zur Analyse und Kontrolle der Importe
* Erweiterung des Systems um **Logging**, **Fehlerhandling** und **Performanceoptimierungen** für große Datenmengen

### 📈 Ergebnis

Das System bildet die **technologische Grundlage** für die spätere Recruiting-Plattform.
Es ermöglicht die **automatisierte Erfassung und Aufbereitung** von tausenden Jobdaten täglich, schafft **saubere Datenstrukturen** für Matching und Vertrieb und verbindet so **Job-, Unternehmens- und Kontaktdaten** in einem zentralen Ökosystem.

### 🛠️ Technologien

`PHP` · `MySQL` · `Cronjobs` · `Automatisierung` · `Smarty` · `jQuery` · `DataTables` · `Backend & Frontend Development` · `Datenvalidierung`

---

## 💸 **Aspeo E-Rechnung – Webbasierter E-Rechnungseditor**

**📅 Zeitraum:** Aug 2024 – März 2025
**🏢 Unternehmen:** Aspeo GmbH

### 🎯 Ausgangssituation

Viele Unternehmen benötigten eine einfache Möglichkeit, **gesetzeskonforme E-Rechnungen** zu erstellen, ohne lokale Software installieren zu müssen.
Bestehende Tools waren **kompliziert**, **unübersichtlich** oder nicht vollständig kompatibel mit aktuellen Standards wie **XRechnung** und **ZUGFeRD**.

### 💡 Aufgabe

Entwicklung eines **webbasierten Editors**, mit dem Nutzer direkt im Browser **strukturierte E-Rechnungen** erstellen, validieren und exportieren können – inklusive **Plausibilitätsprüfungen** und **Formatvalidierung** gemäß den geltenden Normen.

### 🧠 Vorgehen

* Technische **Planung und Definition der Systemarchitektur**
* Entwicklung der **Frontend- und Backend-Logik** (PHP, Smarty, Bootstrap, JavaScript)
* Implementierung der **XML-Validierung** und automatischen Formatprüfung für XRechnung & ZUGFeRD
* Aufbau einer **intuitiven Benutzeroberfläche** mit Fokus auf Benutzerfreundlichkeit und Barrierefreiheit
* Zusammenarbeit mit internen Teams für **Design, Validierung und Deployment**
* Sicherstellung einer **nachhaltigen Code-Struktur** und modularen Erweiterbarkeit

### 📈 Ergebnis

Das Tool ist **produktiv im Einsatz** unter [e-rechnung.aspeo.de/editor](https://e-rechnung.aspeo.de/editor).
Es ermöglicht Unternehmen eine **einfache, rechtssichere und barrierearme Erstellung digitaler Rechnungen** direkt im Browser – mit Fokus auf **UX**, **Datenvalidierung** und **langfristige Wartbarkeit**.

### 🛠️ Technologien

`PHP` · `JavaScript` · `MySQL` · `JSON` · `Projektplanung`

---

## 👥 **Talentpool – Anonymisierte Kandidatenplattform**

**📅 Zeitraum:** Mai 2024 – Okt 2024
**🏢 Unternehmen:** Aspeo GmbH

### 🎯 Ausgangssituation

Partnerunternehmen suchten eine **datenschutzkonforme Möglichkeit**, Fachkräfte aus unterschiedlichen Branchen **anonymisiert auszutauschen und zu vermitteln**.
Bestehende Recruiting-Systeme boten weder die notwendige Anonymisierung noch eine **technisch effiziente Struktur** für gemeinschaftliche Nutzung.

### 💡 Aufgabe

Entwicklung einer **webbasierten Plattform** mit öffentlichem Talentpool und angebundenem Backend, über die Kandidatenprofile **verwaltet, anonymisiert präsentiert** und über **standardisierte Prozesse vermittelt** werden können.

### 🧠 Vorgehen

* Entwicklung des **Backends** zur Verwaltung und Pflege von Kandidatenprofilen (PHP, MySQL, Smarty Framework)
* Aufbau von **Rollen- und Rechteverwaltung** für Administratoren und Partnerunternehmen
* Implementierung der **Such- und Filterlogik** für Kandidatenlisten (PHP, MySQL, JavaScript)
* Gestaltung der **anonymisierten Profilansichten** inkl. UX/UI-Optimierung
* Umsetzung eines **mehrstufigen Freigabe- und Exportprozesses** (DSGVO-konform)
* Integration eines **Matching-Moduls** zur automatisierten Zuordnung von Profilen zu Anfragen
* Erweiterung um **Statistiken**, **Favoritenlisten** und **Statusverwaltung**
* Technische **Skalierung des Systems** für wachsende Datenmengen und neue Branchen
* Entwicklung des öffentlichen Frontends unter [talentpool.techlister.de](https://talentpool.techlister.de)

### 📈 Ergebnis

Das System ist **produktiv im Einsatz** und verbindet **anonymisierte Präsentation** mit **leistungsfähiger Verwaltungslogik**.
Partnerunternehmen können so **DSGVO-konform Fachkräfte austauschen**, während das Backend eine **strukturierte Pflege, Auswertung und Weiterentwicklung** ermöglicht.
Die Architektur ist **modular erweiterbar** und kann zukünftig für weitere Branchen und Automatisierungen ausgebaut werden.

### 🛠️ Technologien

`PHP` · `MySQL` · `JavaScript` · `UX/UI` · `Backend & Frontend Development`

---

## 🧾 **Backup Monitoring Tool – Server Backup-Management & Automatisierung**

**📅 Zeitraum:** Sept 2023 – Jan 2024
**🏢 Unternehmen:** Aspeo GmbH

### 🎯 Ausgangssituation

Die tägliche Sicherung von Kundendaten erfolgte über mehrere **unabhängige Server-Instanzen**, deren Backup-Status bislang nur **manuell überprüft** werden konnte.
Das führte zu **Zeitverlusten**, erschwerter Fehleranalyse und einem erhöhten Risiko unbemerkter Sicherungsausfälle.

### 💡 Aufgabe

Entwicklung eines **internen Tools**, das sämtliche Backup-Vorgänge **automatisiert überwacht**, zentral protokolliert und Administratoren eine **visuelle Übersicht** über alle Sicherungsprozesse bietet.

### 🧠 Vorgehen

* Konzeption und Aufbau der **Datenbankstruktur** zur Speicherung aller Backup-Protokolle
* Entwicklung mehrerer **Cronjobs** zur täglichen Durchführung und Statusaktualisierung
* Implementierung eines **Monitoring-Dashboards** mit Erfolgs-, Fehler- und Laufzeitanzeigen
* Integration von **Benachrichtigungs- und Filterfunktionen** für schnelle Fehleranalyse
* Erweiterung der bestehenden Systeminfrastruktur zur **besseren Automatisierung und Skalierbarkeit**

### 📈 Ergebnis

Das Tool reduziert den **manuellen Kontrollaufwand** erheblich, ermöglicht eine **transparente Fehleranalyse** und gewährleistet die **stabile Sicherung aller Kundendaten**.
Es ist bis heute **produktiv im Einsatz** und ein zentraler Bestandteil des **Server-Monitorings**.

### 🛠️ Technologien

`PHP` · `MySQL` · `Cronjobs` · `Server Monitoring` · `Automatisierung` · `Backend Development`

---
## 🎮 **Game Design Lead – GTA 5 Roleplay Community-Projekt**

**📅 Zeitraum:** Feb 2021 – Feb 2023
**🏠 Privatprojekt / Community-Initiative**

### 🎯 Ausgangssituation

Ein bestehender **GTA 5 Roleplay-Server (ALTV)** benötigte eine klare Struktur, bessere interne Organisation und eine technische Weiterentwicklung.
Ziel war ein **balanciertes Spielerlebnis** mit nachvollziehbaren Spielsystemen, funktionierenden Wirtschaftskreisläufen und abgestimmten Organisationskonzepten.

### 💡 Aufgabe

Übernahme der **Leitung und technischen Weiterentwicklung** des Projekts.
Aufbau klarer Spielstrukturen und Definition von **Systemlogiken** für Unternehmen, Fraktionen und Behörden – inklusive **konzeptioneller und datenbankseitiger Umsetzung**.

### 🧠 Vorgehen

* **Leitung und Koordination** des Game-Design-Teams
* Enge **Kommunikation mit Projektleitung, Dev-Leitung und Webdesign-Abteilung**
* Entwicklung und Dokumentation **regelkonformer Spielsysteme** (z. B. Wirtschaft, Organisationen, Antragsprozesse)
* Bearbeitung und Bewertung von **Spieler- und Gewerbeanträgen**
* **Datenbankpflege** und kleinere Scripting-Aufgaben mit MySQL (HeidiSQL)
* Unterstützung bei **Bugfixing** und konzeptionellen Verbesserungen
* Selbstständige **Weiterbildung in AutoCAD und 3ds Max** zur Unterstützung von Mapping- und Designprozessen

### 📈 Ergebnis

Der Server erreichte eine **hohe Spieleraktivität** und starke **Community-Bindung** durch strukturierte Systeme, transparente Regeln und konsequente Weiterentwicklung.
Das Projekt profitierte von **klaren Entscheidungswegen**, einer **stabilen Datenbasis** und einer **konsistenten Gameplay-Struktur**.

### 🛠️ Technologien & Kompetenzen

`Projektkoordination` · `Teamführung` · `Kommunikation` · `Game Design` · `MySQL` · `AutoCAD` · `3ds Max`

---
