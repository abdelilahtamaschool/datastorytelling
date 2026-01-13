# Netflix Data Storytelling Project

## Algemene Context

### Over de Dataset
De Netflix Titles dataset bevat **8.807 titels** (films en TV-shows) die beschikbaar zijn op het Netflix streaming platform. De data omvat informatie over:
- Type content (Movie of TV Show)
- Titel, regisseur en cast
- Land van productie
- Datum toegevoegd aan Netflix
- Release jaar
- Rating (leeftijdscategorie)
- Duur (minuten voor films, seizoenen voor TV-shows)
- Genre(s)
- Beschrijving

### Doel van het Project
Dit project heeft twee hoofddoelen:

1. **Exploratory Data Analysis (EDA)**: Het verkennen en visualiseren van patronen in de Netflix catalogus om inzicht te krijgen in:
   - De samenstelling van de content library
   - Geografische en temporele trends
   - Genre- en rating-verdelingen

2. **Machine Learning Model**: Het bouwen van een classificatiemodel dat kan voorspellen of nieuwe content een **Movie** of **TV Show** wordt op basis van kenmerken zoals genre, rating, land van herkomst en release jaar.

### Onderzoeksvraag
*"Kunnen we op basis van kenmerken zoals genre, rating, land van herkomst en release jaar voorspellen of nieuwe content een Film of TV Show wordt?"*

---

## EDA Visualisaties

### 1. Missende Waarden (viz_01_missing_values.png)
**Type**: Horizontale staafdiagram

**Wat het toont**: Het percentage missende waarden per kolom in de dataset.

**Key Insights**:
- **Director** heeft de meeste missende waarden (29.91%) - dit is logisch omdat TV-shows vaak meerdere regisseurs per seizoen hebben
- **Country** en **cast** missen elk ongeveer 9.4% van de data
- Kernvelden zoals titel, type en release_year zijn 100% compleet

**Waarom deze grafiek**: Een staafdiagram maakt direct duidelijk welke kolommen aandacht nodig hebben bij data cleaning.

---

### 2. Content Verdeling (viz_02_content_distribution.png)
**Type**: Donut chart + Staafdiagram

**Wat het toont**: De verhouding tussen Movies en TV Shows op Netflix.

**Key Insights**:
- **69.6% Movies** (6.131 titels)
- **30.4% TV Shows** (2.676 titels)
- Netflix heeft meer dan 2x zoveel films als series

**Waarom deze grafiek**: De donut chart werkt goed voor een simpele tweedeling en toont tegelijk het totaal (8.807 titels).

---

### 3. Timeline & Groei (viz_03_timeline_growth.png)
**Type**: Samengestelde visualisatie (4 panels)

**Wat het toont**:
- **Panel 1**: Jaarlijkse content toevoegingen (gestapeld)
- **Panel 2**: Cumulatieve catalogusgroei
- **Panel 3**: Movie vs TV Show trend over tijd
- **Panel 4**: Movie/TV Show ratio per jaar

**Key Insights**:
- Netflix bereikte de **5.000 titels milestone** rond 2018
- Explosieve groei tussen 2015-2019
- De ratio Movies/TV Shows daalt: Netflix investeert steeds meer in series
- 2019 was het piekjaar met 2.016 nieuwe titels

**Waarom deze grafiek**: Meerdere perspectieven op dezelfde data vertellen een completer verhaal over Netflix's contentstrategie.

---

### 4. Geografische Distributie (viz_04_geographical_distribution.png)
**Type**: Lollipop Chart + Proportionele staaf

**Wat het toont**: De top 15 producerende landen en hun aandeel in de totale catalogus.

**Key Insights**:
- **Verenigde Staten** domineert met 3.210 titels (36.4%)
- **India** is tweede met 1.008 titels (11.4%)
- **United Kingdom** derde met 626 titels (7.1%)
- 9.4% van de content heeft geen bekend land van herkomst

**Waarom deze grafiek**: De lollipop chart is een eleganter alternatief voor staafdiagrammen en maakt de enorme voorsprong van de VS visueel duidelijk.

---

### 5. Internationale Content Groei (viz_05_international_growth.png)
**Type**: Area chart met referentielijn

**Wat het toont**: Het percentage niet-Amerikaanse content over tijd.

**Key Insights**:
- Rond 2016 passeerde Netflix de **50% threshold** voor internationale content
- In 2018 bereikte internationale content een piek van ~70%
- Netflix transformeerde van een US-centric naar een global platform

**Waarom deze grafiek**: De area chart met de 50% referentielijn maakt het kantelpunt visueel duidelijk.

---

### 6. Genre Analyse (viz_06_genre_analysis.png)
**Type**: Horizontale staafdiagrammen (2 panels)

**Wat het toont**:
- **Links**: Top 15 genres overall
- **Rechts**: Genre verdeling per content type (Movie vs TV Show)

**Key Insights**:
- **International Movies** is het grootste genre (2.752 titels)
- **Dramas** en **Comedies** zijn universeel populair
- "International TV Shows" genre bestaat alleen voor series (per definitie)
- Documentaries zijn overwegend films

**Waarom deze grafiek**: De vergelijking naast elkaar toont hoe genrevoorkeuren verschillen tussen films en series.

---

### 7. Rating Analyse (viz_07_rating_analysis.png)
**Type**: Staafdiagram met kleurcodering + Gegroepeerde staafdiagram

**Wat het toont**:
- **Links**: Verdeling van content ratings (TV-MA, TV-14, etc.)
- **Rechts**: Leeftijdscategorie per content type

**Key Insights**:
- **TV-MA** (Mature Audiences) is de meest voorkomende rating (3.207 titels)
- **TV-14** is tweede (2.160 titels)
- Content voor **Adults** domineert in zowel Movies als TV Shows
- Kids content is relatief klein maar aanwezig

**Waarom deze grafiek**: Kleurcodering (Kids=turquoise, Teens=geel, Adults=rood) maakt patronen direct zichtbaar.

---

### 8. Duur Analyse (viz_08_duration_analysis.png)
**Type**: Histogram + Staafdiagram

**Wat het toont**:
- **Links**: Distributie van film duur in minuten
- **Rechts**: Aantal seizoenen per TV Show

**Key Insights**:
- Gemiddelde filmduur: **100 minuten** (mediaan: 98 min)
- De meeste films duren 80-120 minuten
- **67% van TV Shows** heeft slechts 1 seizoen
- Slechts enkele shows hebben 10+ seizoenen

**Waarom deze grafiek**: Histogrammen tonen de verdeling, wat belangrijk is voor feature engineering in het model.

---

## Storytelling Visualisaties

### 9. Bump Chart - Genre Ranking Race (viz_storytelling_01_bump_chart.png)
**Type**: Bump Chart (ranking visualisatie)

**Wat het toont**: Hoe genre rankings veranderen over tijd (2016-2021).

**Key Insights**:
- **Dramas** blijft consistent #1
- **Comedies** wisselt met **International Movies** om positie #2-3
- **Action & Adventure** daalde van #3 naar #4
- **Documentaries** steeg in populariteit

**Waarom deze grafiek**: Bump charts zijn perfect voor het visualiseren van ranking-veranderingen over tijd - een verhaal van competitie.

---

### 10. Slope Chart - Content Productie (viz_storytelling_02_slope_chart.png)
**Type**: Slope Chart

**Wat het toont**: Verandering in content productie per land tussen 2017 en 2020.

**Key Insights**:
- **Verenigde Staten**: 404 -> 710 titels (+76%)
- **Japan**: 30 -> 67 titels (+123%) - sterkste relatieve groei
- **India**: 153 -> 193 titels (+26%)
- **United Kingdom**: lichte daling van 120 naar 107

**Waarom deze grafiek**: Slope charts zijn ideaal voor before/after vergelijkingen en tonen zowel absolute als relatieve verandering.

---

### 11. Radial Bar Chart - Genre Populariteit (viz_storytelling_03_radial_bar.png)
**Type**: Radiale staafdiagram

**Wat het toont**: Genre populariteit in een circulaire weergave.

**Key Insights**:
- Visueel aantrekkelijke weergave van genre-aantallen
- **Dramas** (3.199) en **International Movies** (2.752) domineren
- Kleinere genres worden nog steeds zichtbaar weergegeven

**Waarom deze grafiek**: Een radial bar chart is visueel opvallend en past goed bij presentaties - het vertelt hetzelfde verhaal als een bar chart maar op een memorabele manier.

---

### 12. Dumbbell Chart - Movies vs TV Shows per Genre (viz_storytelling_04_dumbbell.png)
**Type**: Dumbbell Chart

**Wat het toont**: Het verschil tussen aantal Movies en TV Shows per genre.

**Key Insights**:
- **Dramas**: Enorm verschil (Movies ~2.400, TV Shows ~800)
- **Comedies**: Ook grote gap in voordeel van Movies
- **Crime**: Uniek - TV Shows domineren over Movies
- De verbindingslijn visualiseert de "gap" tussen content types

**Waarom deze grafiek**: Dumbbell charts zijn perfect voor het vergelijken van twee groepen over meerdere categorieen - de lengte van de lijn vertelt het verhaal.

---

## Model Visualisaties

### 13. Confusion Matrix (model_01_confusion_matrix.png)
**Type**: Heatmap (2 matrices naast elkaar)

**Wat het toont**: De voorspellingsprestaties van Random Forest vs Logistic Regression.

**Key Insights**:
- **Random Forest**: 1.212 correct voorspelde Movies, 521 correcte TV Shows
- Slechts 14 false positives en 14 false negatives
- Beide modellen presteren zeer vergelijkbaar
- Accuracy: 98.4%

**Interpretatie**:
- Diagonaal = correcte voorspellingen (donkerrood/donkergrijs)
- Off-diagonal = fouten (lichter)

---

### 14. ROC Curve (model_02_roc_curve.png)
**Type**: ROC Curve met ingezoomde view

**Wat het toont**: De trade-off tussen True Positive Rate en False Positive Rate.

**Key Insights**:
- **Random Forest AUC**: 0.996 (bijna perfect)
- **Logistic Regression AUC**: 0.993
- De ingezoomde view (rechts) toont het echte verschil in de kritieke hoek
- Bij 99% TPR heeft RF 8.0% FPR vs LR met 16.6% FPR

**Waarom twee views**: De standaard ROC curve (links) toont bijna perfecte curves. De ingezoomde view onthult de subtiele verschillen die relevant zijn voor modelselectie.

---

### 15. Feature Importance (model_03_feature_importance.png)
**Type**: Horizontale staafdiagram

**Wat het toont**: Welke kenmerken het model gebruikt om Movies vs TV Shows te onderscheiden.

**Top 5 Belangrijkste Features**:
1. **Heeft Regisseur** (0.621) - Verreweg de belangrijkste
2. **Genre: International TV Shows** (0.235)
3. **Genre: Documentaries** (0.032)
4. **Genre: Children/Family** (0.024)
5. **Release Jaar** (0.023)

**Interpretatie**: Movies hebben bijna altijd een regisseur in de metadata (96.9%), terwijl TV Shows dit slechts 8.6% van de tijd hebben. Dit maakt het een zeer sterke voorspeller.

---

### 16. Feature Analysis (model_04_feature_analysis.png)
**Type**: 4-panel dashboard

**Wat het toont**: Hoe de belangrijkste features verschillen tussen Movies en TV Shows.

**Panel 1 - "International TV Shows" Genre**:
- 0% van Movies heeft dit genre (logisch, het is een TV-specifiek label)
- 50.5% van TV Shows heeft dit genre

**Panel 2 - Regisseur Informatie**:
- 96.9% van Movies heeft een regisseur vermeld
- Slechts 8.6% van TV Shows heeft dit

**Panel 3 - Genre Count**:
- Movies en TV Shows hebben gemiddeld ~2 genres
- TV Shows hebben iets meer spreiding

**Panel 4 - Release Jaar Trend**:
- Movies waren dominant tot ~2015
- TV Shows groeiden sneller na 2015

---

### 17. Model Summary Dashboard (model_05_summary_dashboard.png)
**Type**: Executive Dashboard

**Wat het toont**: Een samenvatting van de modelprestaties op een blik.

**KPIs**:
- **98.4%** Model Accuracy
- **0.996** AUC Score
- **8.803** Training Samples

**Componenten**:
- Mini Confusion Matrix
- Mini ROC Curve
- Top 5 Features bar chart

**Waarom deze grafiek**: Een dashboard brengt alle key metrics samen voor stakeholders die snel de bottomline willen zien.

---

## Conclusies

### EDA Conclusies
1. Netflix's catalogus is **film-gedomineerd** (70/30 split)
2. De **VS** produceert het meeste content, maar internationale content groeit
3. **Mature content** (TV-MA) domineert de catalogus
4. De catalogus groeide explosief tussen **2015-2019**

### Model Conclusies
1. Het model bereikt **98.4% accuracy** - Movies en TV Shows zijn goed te onderscheiden
2. **"Heeft Regisseur"** is de sterkste voorspeller (films hebben vrijwel altijd een regisseur vermeld)
3. Genre-labels zoals "International TV Shows" zijn sterke indicatoren
4. Netflix categoriseert content op een voorspelbare, systematische manier

### Business Implicaties
- Netflix's metadata-structuur verschilt systematisch tussen films en series
- Internationale content is een groeiprioriteit
- De verschuiving naar meer TV Shows wijst op een strategie voor langere kijkerbinding
