# Datengetriebene Prognosen im Hochschulbereich:
## Ein Data-Mining-Ansatz zur Vorhersage von Abschlussquoten an universitären Hochschulen und Fachhochschulen in der Schweiz

Dieses Projekt verarbeitet und prognostiziert Hochschulabschlussdaten (FH & HS) in der Schweiz. Es wurde im Rahmen eines Data-Mining-Projekts (unter Verwendung des CRISP-DM-Prozesses) entwickelt, um einem EdTech-Startup datengetriebene Einblicke zur Optimierung der Lernplattform zu liefern.

## Inhalt
- **Problemstellung:** Prognose zukünftiger Abschlussquoten zur Unterstützung strategischer Entscheidungen.
- **Datenakquise:** Import von CSV-/Excel-Dateien (von opendata.swiss) mit relevanten Abschlussdaten.
- **Datenaufbereitung:** Bereinigung, Normalisierung (BCNF) und Integration in eine SQLite-Datenbank.
- **Feature Engineering:** Erstellung von Interaktions- (z.B. field_university_interaction) und aggregierten Merkmalen.
- **Modellierung:** Evaluation verschiedener Modelle (z.B. Lineare Regression, ARIMA, Neural Networks, Decision Tree, GBM, LSTM, Prophet) – laut Studienarbeit liefert Prophet die besten Ergebnisse für 2024.
- **Studienarbeit:** Detaillierte Analyse des Data-Mining-Prozesses, Einsatz generativer KI und kritische Evaluierung der Modelle.
- **Visualisierungen:** Diverse Charts zur Darstellung von Trends und Prognosen.

## Voraussetzungen & Setup
- Python 3.x mit folgenden Libraries: pandas, numpy, matplotlib, sqlite3, ydata_profiling, scikit-learn, statsmodels, tensorflow, prophet, joblib
- VS Code als Entwicklungsumgebung
- pip install -r requirements.txt

### Ausführung
1. **Input-Daten:** Lege die CSV- und Excel-Dateien in einen Ordner `input`.
2. **Datenbank:** Das Skript erstellt die SQLite-Datenbank im Ordner `output` mithilfe von `CREATE TABLE IF NOT EXISTS`.
3. **Pipeline:** Das Skript führt alle Schritte von der Datenbereinigung über Feature-Generierung bis zur Modellierung und Evaluation aus.
4. **Ergebnisse:** Reports, Visualisierungen und Modellprognosen (inkl. Vorhersagen für 2024) werden im Ordner `output` abgelegt.

Viel Spass!