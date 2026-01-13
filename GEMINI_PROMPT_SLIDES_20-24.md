# Gemini Prompt Context - Slides 20-24

## Project Overzicht

Dit is een **Netflix Data Storytelling** project voor een schoolopdracht. Het doel is om met data een verhaal te vertellen volgens de **Data Storytelling Arc**:
1. Setting & Hook
2. Rising Points
3. Aha Moment
4. Solution & Next Steps

De presentatie is een video-opname van 12-15 minuten.

---

## Dataset Informatie

- **Bron:** Netflix Titles Dataset
- **Aantal titels:** 8.807 (6.131 Movies, 2.676 TV Shows)
- **Verdeling:** 69.6% Movies, 30.4% TV Shows
- **Kolommen:** type, title, director, cast, country, date_added, release_year, rating, duration, listed_in (genres), description

---

## Samenvatting van Slides 1-19 (Wat de kijker al weet)

### Act 1: Setting & Hook (Slides 1-4)
- Netflix heeft 8.807 titels, 70% films en 30% series
- Onderzoeksvraag: "Kunnen we voorspellen of content een film of TV-show wordt?"
- Data kwaliteit check: 'director' veld mist 30% van de data (belangrijk voor later)

### Act 2: Rising Points (Slides 5-13)
De kijker heeft de volgende inzichten gezien:

1. **Explosieve groei:** Netflix groeide van honderden naar duizenden titels per jaar (2015-2019)
2. **Verschuiving naar series:** Het aandeel TV-shows groeit elk jaar
3. **Duur analyse:**
   - Gemiddelde film: 100 minuten
   - 67% van TV-shows heeft maar 1 seizoen
   - Series houden kijkers langer vast (binge-watching strategie)
4. **Geografische verdeling:**
   - VS domineert (36.4%, 3.210 titels)
   - India tweede (11.4%, 1.008 titels)
   - UK derde (7.1%, 626 titels)
5. **Internationale transformatie:** In 2016 passeerde Netflix de 50% grens voor internationale content, piek van 70% in 2018
6. **Genre analyse:**
   - International Movies is grootste genre
   - Dramas en Comedies zijn universeel populair
   - Sommige genres zijn "film-genres", andere "serie-genres"
7. **Genre ranking race (bump chart):** Dramas blijft #1, Documentaries stijgt
8. **Rating analyse:** TV-MA (mature) domineert met 3.207 titels, Netflix richt zich op volwassenen
9. **Slope chart:** Japan groeit het snelst (+123%), anime-explosie
10. **Dumbbell chart:** Bij Crime zijn er meer series dan films (true crime werkt beter als serie)

### Act 3: Aha Moment (Slides 14-19)
De kijker heeft de centrale ontdekking gezien:

**Het Machine Learning Model:**
- Random Forest Classifier
- **98.4% accuracy**
- **AUC score: 0.996**
- Getraind op 8.803 samples

**De Grote Ontdekking (Feature Importance):**
- **"Heeft Regisseur"** is de belangrijkste feature met importance score 0.621
- Dit ene kenmerk bepaalt 60%+ van de voorspelling
- Waarom? 97% van films heeft een regisseur in metadata, slechts 8.6% van TV-shows
- Netflix registreert regisseurs anders voor films vs series (systematisch verschil in data-architectuur)

**Model Validatie:**
- Confusion Matrix: 1.212 correct voorspelde films, 521 correcte TV-shows, slechts 28 fouten totaal
- ROC Curve: Bijna perfecte curve in linkerbovenhoek

---

## Slides 20-24: Solution & Next Steps

Dit zijn de slides die nog gemaakt moeten worden. Ze vormen de **afsluiting** van het verhaal.

### SLIDE 20: Wat Betekent Dit? - Praktische Implicaties
**Doel:** Vertaal de bevindingen naar praktische waarde

**Kernpunten:**
1. **Voor content strategen:**
   - Als je weet hoe Netflix categoriseert, kun je betere pitch-beslissingen maken
   - Wil je een serie verkopen? Zorg dat het past bij serie-kenmerken

2. **Voor data analisten:**
   - Metadata is geen bijzaak
   - Hoe een bedrijf data registreert, onthult hun denkwijze
   - Verborgen patronen in data-structuur hebben voorspellende waarde

3. **Voor Netflix zelf:**
   - Hun data-architectuur is transparanter dan gedacht
   - De manier waarop regisseurs geregistreerd worden, onthult het verschil tussen films en series

**Afsluitende gedachte:** "Data vertelt altijd een verhaal. Soms een verhaal dat je niet bewust deelt."

---

### SLIDE 21: De Drie Grote Trends
**Doel:** Vat de belangrijkste trends samen in memorable punten

**Trend 1: Van films naar series**
- Netflix investeert steeds meer in TV-shows
- Reden: Series houden kijkers langer op het platform
- Binge-watching is de strategie
- Data bewijs: Groeiend aandeel zwart (series) in timeline grafiek

**Trend 2: Van Amerika naar de wereld**
- Internationale content is nu de meerderheid (>50% sinds 2016)
- K-drama's, anime, Europese series groeien
- Netflix transformeerde van Amerikaans naar globaal platform
- Data bewijs: 70% internationale content in 2018

**Trend 3: Data-structuur onthult strategie**
- Het verschil tussen films en series zit niet alleen in content
- Het zit in hoe Netflix hun metadata organiseert
- Regisseur-registratie is het sleutelkenmerk
- Dit is voorspelbaar met 98.4% nauwkeurigheid

---

### SLIDE 22: Beperkingen en Vervolgonderzoek
**Doel:** Wees eerlijk over de grenzen van het onderzoek

**Beperkingen:**
1. Dataset gaat tot 2021 - Netflix's strategie kan sindsdien veranderd zijn
2. Alleen metadata geanalyseerd, geen kijkcijfers of reviews (niet publiek beschikbaar)
3. Model voorspelt categorisering, niet succes - of iets populair wordt is een andere vraag
4. Mogelijke bias in hoe Netflix data registreert per regio

**Mogelijkheden voor vervolgonderzoek:**
1. Hoe voorspel je hits? Welke combinatie van kenmerken leidt tot hoge kijkcijfers?
2. Vergelijking met andere streamingplatforms (Disney+, Amazon Prime)
3. Sentiment analyse van beschrijvingen
4. Tijdreeksanalyse: hoe veranderen patronen per kwartaal?

---

### SLIDE 23: Conclusie - Het Verhaal Compleet
**Doel:** Rond het verhaal af met een sterke conclusie

**De reis samengevat:**
1. We begonnen met een vraag: "Wat bepaalt of content een film of TV-show wordt?"
2. We verkenden de data: groei, globalisering, genres, ratings, duur
3. We vonden het antwoord: niet in de content zelf, maar in de metadata
4. Specifiek: hoe Netflix regisseurs registreert

**Het centrale inzicht:**
- Films hebben bijna altijd een regisseur in de database (97%)
- Series bijna nooit (8.6%)
- Dit simpele verschil voorspelt met 98% nauwkeurigheid of iets een film of serie is

**De les:**
- Soms zit het antwoord niet in de voor de hand liggende data
- Soms zit het in de structuur, in wat er mist, in hoe iets geregistreerd wordt
- "Data vertelt altijd een verhaal. Je moet alleen leren luisteren."

---

### SLIDE 24: Afsluiting
**Doel:** Bedank en sluit af

**Inhoud:**
- Korte bedanking
- Eventueel naam/studentnummer
- Eventueel bronvermelding (Netflix dataset van Kaggle)

**Spreektekst:**
"Dat was mijn data storytelling analyse van Netflix. Van exploratie tot machine learning, van vraag tot antwoord. Ik hoop dat je iets hebt geleerd over hoe data patronen kan onthullen die je niet verwacht. Bedankt voor het kijken."

---

## Stijl en Toon

- **Taal:** Nederlands
- **Toon:** Professioneel maar toegankelijk, niet te academisch
- **Publiek:** Docenten en medestudenten die bekend zijn met data analyse
- **Doel:** Aantonen dat data storytelling principes zijn toegepast

---

## Belangrijke Cijfers om te Onthouden

| Metric | Waarde |
|--------|--------|
| Totaal titels | 8.807 |
| Movies | 6.131 (69.6%) |
| TV Shows | 2.676 (30.4%) |
| Model Accuracy | 98.4% |
| AUC Score | 0.996 |
| Top Feature | "Heeft Regisseur" (0.621) |
| Films met regisseur | 97% |
| TV Shows met regisseur | 8.6% |
| Internationale content (2018) | ~70% |
| Top land | VS (36.4%) |

---

## Beschikbare Grafieken (voor referentie)

Geen specifieke grafiek nodig voor slides 20-24, deze zijn tekst/bullet-based slides. Eventueel kunnen worden gebruikt:
- Een infographic met de 3 trends (zelf maken)
- Het model_05_summary_dashboard.png als achtergrond voor conclusie
- De Data Storytelling Arc afbeelding voor de afsluiting

---

## Gewenste Output

Maak voor elke slide (20-24):
1. Een PowerPoint-vriendelijke layout suggestie
2. De belangrijkste bullet points
3. Eventuele visual/icoon suggesties
4. Speaker notes (wat te zeggen)
