# Projektplan Barrierefreiheit - Südpfalz Therme Bad Bergzabern

## 1. Projektübersicht

**Auftraggeber:** Staatsbad Bad Bergzabern GmbH  
**Website:** www.suedpfalz-therme.de  
**Projektziel:** Vollständige Barrierefreiheit nach WCAG 2.1 Level AA und BITV 2.0  
**Geschätzter Zeitrahmen:** 3-9 Monate (je nach Paket)  
**Geschätztes Budget:** 42.800 - 128.000 EUR (netto)

## 2. IST-Zustand Analyse

### Aktuelle Zertifizierung (Reisen für Alle):
- ✓ Barrierefrei für Menschen mit Gehbehinderung
- ⚠️ Teilweise barrierefrei für Rollstuhlfahrer  
- ⚠️ Teilweise barrierefrei für Menschen mit Sehbehinderung
- ❌ Keine Zertifizierung für Hörbehinderung
- ❌ Keine Zertifizierung für kognitive Beeinträchtigungen

### Identifizierte Hauptprobleme:
1. **Navigation:** Komplexe Menüstruktur ohne Tastaturnavigation
2. **Bilder:** Fehlende oder unzureichende Alt-Texte
3. **Kontraste:** Teilweise zu geringe Farbkontraste
4. **Formulare:** Fehlende Label-Zuordnungen
5. **Responsive Design:** Eingeschränkte mobile Nutzbarkeit
6. **Screenreader:** Unzureichende semantische Struktur
7. **Sprache:** Fehlende Leichte Sprache Option
8. **Videos/Multimedia:** Keine Untertitel oder Audiodeskription

## 3. Detaillierter Maßnahmenplan

### Phase 1: Technische Grundlagen (Wochen 1-3)

#### 1.1 Audit & Dokumentation
- **WCAG 2.1 Vollaudit** durch zertifizierten Prüfer
- **Automatisierte Tests** mit axe DevTools, WAVE, Pa11y
- **Manuelle Tests** mit Screenreadern (NVDA, JAWS)
- **Tastaturnavigation-Test**
- **Mobile Accessibility Tests**
- **Erstellung Prüfbericht** mit Priorisierung

**Aufwand:** 40-50 Stunden  
**Kosten:** 4.000-5.000 EUR

#### 1.2 Technische Infrastruktur
- **CMS-Update** auf barrierefreie Version
- **Framework-Anpassungen** für Accessibility
- **Build-Pipeline** mit Accessibility-Checks
- **Monitoring-Tools** Installation

**Aufwand:** 20-30 Stunden  
**Kosten:** 2.000-3.000 EUR

### Phase 2: Frontend-Entwicklung (Wochen 4-8)

#### 2.1 Navigationsstruktur
- **Hauptmenü-Überarbeitung:**
  - Skip-Navigation implementieren
  - Tastatur-Navigation (Tab-Order)
  - ARIA-Labels und Landmarks
  - Breadcrumb-Navigation
  - Sitemap erstellen

**Aufwand:** 30-40 Stunden  
**Kosten:** 3.000-4.000 EUR

#### 2.2 Inhaltsstruktur
- **Semantisches HTML:**
  - Korrekte Heading-Hierarchie (h1-h6)
  - Listen-Strukturierung
  - Tabellen mit scope und caption
  - Landmark-Regionen (main, nav, aside)

**Aufwand:** 40-50 Stunden  
**Kosten:** 4.000-5.000 EUR

#### 2.3 Formulare & Interaktive Elemente
- **Buchungsformulare:**
  - Label-for-Verknüpfungen
  - Fehlermeldungen mit ARIA-live
  - Pflichtfeld-Kennzeichnung
  - Validierung mit Screenreader-Unterstützung
- **Kalender-Widget** barrierefrei gestalten
- **Preiskalkulator** mit Tastatur bedienbar

**Aufwand:** 50-60 Stunden  
**Kosten:** 5.000-6.000 EUR

#### 2.4 Multimedia & Bilder
- **Alt-Texte:**
  - Alle Bilder mit beschreibenden Alt-Texten
  - Komplexe Grafiken mit Langbeschreibungen
  - Dekorative Bilder mit alt=""
- **Videos:**
  - Untertitel für alle Videos
  - Audiodeskription für wichtige visuelle Inhalte
  - Transkripte bereitstellen

**Aufwand:** 30-40 Stunden  
**Kosten:** 3.000-4.000 EUR

### Phase 3: Design & Visuelles (Wochen 9-11)

#### 3.1 Farbkontraste & Typografie
- **Kontrastanpassungen:**
  - Mindestkontrast 4.5:1 für Normaltext
  - Mindestkontrast 3:1 für Großtext
  - Fokus-Indikatoren verstärken
- **Schriftgrößen:**
  - Relative Einheiten (rem/em)
  - Zoom bis 200% ohne Horizontalscrolling

**Aufwand:** 20-30 Stunden  
**Kosten:** 2.000-3.000 EUR

#### 3.2 Responsive Design
- **Touch-Targets:** Mindestens 44x44 Pixel
- **Viewport-Meta-Tag** korrekt setzen
- **Orientierungswechsel** unterstützen
- **Gestenerkennung** mit Alternativen

**Aufwand:** 30-40 Stunden  
**Kosten:** 3.000-4.000 EUR

### Phase 4: Inhalte & Kommunikation (Wochen 12-14)

#### 4.1 Leichte Sprache
- **Hauptseiten in Leichter Sprache:**
  - Startseite
  - Öffnungszeiten & Preise
  - Anfahrt & Kontakt
  - Buchungsbereich
- **Piktogramme** zur Unterstützung
- **Glossar** für Fachbegriffe

**Aufwand:** 40-50 Stunden  
**Kosten:** 4.000-5.000 EUR

#### 4.2 Gebärdensprache
- **Willkommensvideo** in DGS
- **Wichtige Informationen** als DGS-Videos
- **Virtuelle Tour** mit DGS-Begleitung

**Aufwand:** 30-40 Stunden  
**Kosten:** 5.000-7.000 EUR

### Phase 5: Testing & Dokumentation (Wochen 15-16)

#### 5.1 Umfassende Tests
- **Nutzertest mit Betroffenen:**
  - 5 blinde/sehbehinderte Nutzer
  - 3 motorisch eingeschränkte Nutzer
  - 3 gehörlose Nutzer
  - 3 kognitiv eingeschränkte Nutzer
- **Technische Nachtests**
- **Cross-Browser-Testing**

**Aufwand:** 40-50 Stunden  
**Kosten:** 6.000-8.000 EUR

#### 5.2 Dokumentation & Schulung
- **Barrierefreiheitserklärung** erstellen
- **Feedback-Mechanismus** implementieren
- **Redaktionshandbuch** für barrierefreie Inhalte
- **Mitarbeiterschulung** (2 Tage)

**Aufwand:** 30-40 Stunden  
**Kosten:** 3.000-4.000 EUR

## 4. Realistischer Zeitplan

### Basis-Paket (3-4 Monate):
```
Monat 1: Audit & Planung
Monat 2-3: Kritische Anpassungen
Monat 4: Testing & Dokumentation
```

### Standard-Paket (5-6 Monate):
```
Monat 1: Umfassender Audit & Setup
Monat 2-3: Technische Umsetzung Phase 1
Monat 4: Design & Content-Anpassungen
Monat 5: Leichte Sprache & erweiterte Features
Monat 6: Testing, Schulung & Go-Live
```

### Premium-Paket (7-9 Monate):
```
Monat 1: Vollanalyse & Projektsetup
Monat 2-3: Grundlegende technische Umsetzung
Monat 4-5: Erweiterte Features & Redesign
Monat 6: Leichte Sprache (vollständig)
Monat 7: DGS-Videoproduktion
Monat 8: Intensive Nutzertests
Monat 9: Optimierung, Schulung & Launch
```

**Wichtige Faktoren für Zeitplanung:**
- Abstimmungsschleifen mit Stakeholdern: +20-30%
- Technische Abhängigkeiten (CMS, Buchungssystem): +15-25%
- Urlaubszeiten und Feiertage: +10-15%
- Änderungswünsche während des Projekts: +15-20%

## 5. Realistische Kostenübersicht

### Hauptpakete:

| Paket | Leistungsumfang | Zeitrahmen | Kosten (netto) |
|-------|-----------------|------------|----------------|
| **Basis** | Gesetzliche Mindestanforderungen | 3-4 Monate | 42.800 EUR |
| **Standard** | Professionelle Barrierefreiheit | 5-6 Monate | 76.500 EUR |
| **Premium** | Vollständige Inklusion mit DGS | 7-9 Monate | 128.000 EUR |

### Detailaufschlüsselung Standard-Paket:

| Bereich | Aufwand (Std.) | Kosten |
|---------|----------------|--------|
| Technischer Audit & Setup | 85 | 11.050 EUR |
| Navigation & Bedienbarkeit | 45 | 5.850 EUR |
| Buchungssystem Anpassung | 80 | 10.400 EUR |
| Bilder & Multimedia | 100 | 13.000 EUR |
| Formulare & Interaktion | 60 | 7.800 EUR |
| Design & Kontraste | 40 | 5.200 EUR |
| Leichte Sprache (30%) | 50 | 6.500 EUR |
| Testing & QA | 90 | 11.700 EUR |
| Dokumentation & Schulung | 40 | 5.000 EUR |
| **Gesamt** | **590** | **76.500 EUR** |

### Versteckte Kosten (oft vergessen):

| Position | Einmalig | Laufend/Jahr |
|----------|----------|--------------|
| CMS-Update/Migration | 8.000-12.000 EUR | - |
| PDF-Remediation (50+ Dokumente) | 12.000 EUR | 3.000 EUR |
| Server/Hosting Upgrade | 5.000-8.000 EUR | 2.400 EUR |
| Monitoring & Wartung | 3.000 EUR Setup | 14.400-21.600 EUR |
| Re-Zertifizierung BITV | - | 2.500 EUR |
| Content-Updates | - | 6.000-12.000 EUR |
| **Zusätzlich ca.** | **28.000-35.000 EUR** | **28.300-41.500 EUR** |

### Gesamtinvestition erstes Jahr:

- **Basis-Szenario:** 42.800 + 28.000 + 28.300 = **99.100 EUR**
- **Standard-Szenario:** 76.500 + 31.500 + 35.000 = **143.000 EUR**
- **Premium-Szenario:** 128.000 + 35.000 + 41.500 = **204.500 EUR**

## 6. Erfolgskriterien

### Technische Kriterien:
- ✓ WCAG 2.1 Level AA Konformität
- ✓ BITV 2.0 Konformität
- ✓ Erfolgreiche Zertifizierung
- ✓ 0 kritische Barrieren im Abschlusstest

### Nutzerzentrierte Kriterien:
- ✓ 95% positive Rückmeldungen in Nutzertests
- ✓ Alle Hauptfunktionen mit Tastatur bedienbar
- ✓ Screenreader-Kompatibilität für alle Inhalte
- ✓ Mobile Nutzbarkeit auf allen gängigen Geräten

## 7. Wartung & Nachhaltigkeit

### Kontinuierliche Maßnahmen:
1. **Monatliche automatisierte Tests**
2. **Quartalsweise manuelle Prüfungen**
3. **Halbjährliche Nutzertests**
4. **Jährliche Rezertifizierung**
5. **Fortlaufende Mitarbeiterschulungen**

### Redaktionelle Richtlinien:
- Checkliste für barrierefreie Inhalte
- Alt-Text-Generator für Bilder
- Kontrastprüfer im CMS
- Automatische Validierung vor Veröffentlichung

## 8. Angebotskalkulation

### Basispaket (45.000 EUR):
- Technischer Audit
- WCAG 2.1 AA Umsetzung
- Grundlegende Tests
- Barrierefreiheitserklärung

### Premiumpaket (65.000 EUR):
- Alles aus Basispaket
- Leichte Sprache für Hauptinhalte
- DGS-Videos
- Umfassende Nutzertests
- BITV-Zertifizierung
- 1 Jahr Wartung inklusive

### Empfehlung:
Für die Südpfalz Therme als öffentliche Einrichtung mit hohem Besucheraufkommen und komplexem Buchungssystem empfehle ich das **Standard-Paket für 76.500 EUR**. 

Das Basis-Paket erfüllt zwar die gesetzlichen Mindestanforderungen, führt aber erfahrungsgemäß zu:
- Berechtigten Nutzerbeschwerden
- Negativer Presse
- Möglichen Klagen von Behindertenverbänden
- Schlechteren Google-Rankings

Das Standard-Paket bietet echte Barrierefreiheit und ein gutes Preis-Leistungs-Verhältnis. Das Premium-Paket wäre ideal für eine Positionierung als Leuchtturmprojekt, erfordert aber ein Budget von über 200.000 EUR im ersten Jahr.

## 9. Nächste Schritte

1. **Kick-off Meeting** mit allen Stakeholdern
2. **Detailaudit** der aktuellen Website
3. **Priorisierung** der Maßnahmen
4. **Ressourcenplanung** intern/extern
5. **Vertragsunterzeichnung** und Projektstart

---

*Dieser Projektplan basiert auf Best Practices und aktuellen Standards (Stand: Juni 2025). Änderungen vorbehalten.*