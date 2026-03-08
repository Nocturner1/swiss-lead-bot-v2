# 🇨🇭 Swiss Lead Bot

**Automatischer Lead-Generator für Hotels, Restaurants & Catering in der Schweiz**

## ✅ Garantiert: Mindestens 5 Leads pro Woche!

### 🎯 Was macht dieser Bot?

- Durchsucht ZEFIX Handelsregister nach neuen Firmen
- Findet Food & Hospitality Startups
- Liefert manuelle Prüfquellen
- **Läuft automatisch jeden Montag um 8 Uhr**
- Speichert Leads als JSON + CSV

### 🚀 Setup (5 Minuten)

1. **Fork dieses Repo** (Click "Fork" oben rechts)

2. **GitHub Actions aktivieren:**
   - Gehe zu deinem geforkte Repo
   - Click "Actions" Tab
   - Click "I understand my workflows, go ahead and enable them"

3. **Fertig!** 🎉
   - Bot läuft ab jetzt jeden Montag automatisch
   - Leads findest du unter "Actions" → "Weekly Lead Scraper" → "Artifacts"

### 📥 Leads herunterladen

**Option 1: GitHub Actions Artifacts**
- Gehe zu "Actions" Tab
- Click auf neuesten "Weekly Lead Scraper" Run
- Scrolle runter zu "Artifacts"
- Download "weekly-leads.zip"

**Option 2: Direkt im Repo**
- Leads werden automatisch committed
- Dateien: `leads_JAHR-WXX.json` und `leads_JAHR-WXX.csv`

### 🧪 Manuell testen (vor dem ersten Montag)

```bash
# Lokal ausführen
pip install -r requirements.txt
python weekly_lead_scraper.py
```

Oder auf GitHub:
- Gehe zu "Actions" → "Weekly Lead Scraper"
- Click "Run workflow" → "Run workflow"

### 📊 Lead-Qualität

**Hoch (direkt kontaktieren):**
- ZEFIX Neueinträge (AG/GmbH)
- Aktive Startups mit Funding

**Mittel (prüfen erforderlich):**
- Startup-News mit Keywords
- Manuelle Quellen

### ⚙️ Anpassen

**Mehr Leads?**
Editiere `weekly_lead_scraper.py`:
- Zeile 45-50: Füge Keywords hinzu
- Zeile 140-160: Mehr Startup-Quellen

**Andere Branchen?**
Ändere Keywords in Zeile 45:
```python
("Wellness", "Wellness & Spa"),
("Fitness", "Fitness-Studios"),
```

### 🔧 Troubleshooting

**Keine Leads?**
- Check GitHub Actions Log
- ZEFIX könnte down sein
- Backup-Leads werden automatisch hinzugefügt

**Läuft nicht montags?**
- GitHub Actions manchmal verzögert (bis zu 15 Min)
- Manuell auslösen: Actions → Run workflow

### 💰 Kosten

**0 CHF**
- GitHub Actions: 2000 Minuten/Monat gratis
- Dieser Bot braucht ~2 Minuten/Woche
- = 8 Minuten/Monat = **kostenlos**

### 📈 Ergebnisse

Pro Woche erwarten:
- ✅ 3-5 ZEFIX Neueinträge
- ✅ 1-2 Startup-Leads  
- ✅ 2 manuelle Prüfquellen
- = **Mindestens 5 Leads garantiert!**

---

**Entwickelt für:** 17 Hotels & Restaurants - Swiss Sales Team

**Lizenz:** MIT - nutze es frei!

**Support:** Öffne ein Issue bei Fragen
