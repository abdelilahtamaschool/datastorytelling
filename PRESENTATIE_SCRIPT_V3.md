# Netflix Data Storytelling - Presentatie Script V3 (Uitgebreid)

> Gestructureerd volgens de **Data Storytelling Arc** | Geschatte tijd: **12-15 minuten**

---

# ACT 1: SETTING & HOOK
*Doel: Pak de aandacht, introduceer het probleem en de context*

---

## SLIDE 1: Opening - De Wereld van Netflix
**Afbeelding:** Netflix logo of interface screenshot
**Tijd:** ~45 seconden

### Spreektekst:
"Netflix. Een naam die iedereen kent. Wat begon als een DVD-verhuurbedrijf in 1997, is uitgegroeid tot 's werelds grootste streamingplatform met meer dan 230 miljoen abonnees wereldwijd.

Maar achter die bekende rode interface schuilt een enorme machine van beslissingen. Elke dag moet Netflix kiezen: welke content kopen we in? Wat produceren we zelf? En misschien wel de belangrijkste vraag: wordt iets een film... of een serie?

Die keuze lijkt simpel, maar bepaalt alles. Het budget, de marketingstrategie, hoe lang kijkers op het platform blijven.

Vandaag duiken we in de data achter die beslissingen. En ik beloof je: wat we ontdekken, zal je verrassen."

---

## SLIDE 2: De Onderzoeksvraag
**Afbeelding:** Tekst van de onderzoeksvraag, eventueel met vraagteken visual
**Tijd:** ~30 seconden

### Spreektekst:
"De centrale vraag van dit onderzoek is:

**Kunnen we op basis van data voorspellen of nieuwe content een film of een TV-show wordt?**

Klinkt misschien abstract, maar denk er eens over na. Als we kunnen voorspellen hoe Netflix content categoriseert, begrijpen we hoe ze denken. We ontrafelen hun strategie.

En spoiler alert: het antwoord is ja. Met 98 procent nauwkeurigheid. Maar laten we bij het begin beginnen."

---

## SLIDE 3: Het Speelveld - De Netflix Catalogus
**Afbeelding:** viz_02_content_distribution.png
**Tijd:** ~40 seconden

### Spreektekst:
"Dit is ons speelveld. De complete Netflix catalogus, gevisualiseerd.

Links zie je een donut chart: 8.807 titels in totaal. Bijna 70 procent daarvan - ruim 6.100 titels - zijn films. De overige 30 procent, zo'n 2.700 titels, zijn TV-shows.

Rechts zie je dezelfde data als staafdiagram. Het verschil is enorm. Meer dan twee keer zoveel films als series.

Maar waarom? Is dit toeval? Een historisch overblijfsel? Of zit hier strategie achter?

Om dat te begrijpen, moeten we eerst kijken naar de kwaliteit van onze data."

---

## SLIDE 4: Data Kwaliteit - De Basis op Orde
**Afbeelding:** viz_01_missing_values.png
**Tijd:** ~35 seconden

### Spreektekst:
"Voordat we conclusies kunnen trekken, moeten we weten of onze data betrouwbaar is. Deze grafiek toont hoeveel data er mist per kolom.

Wat direct opvalt: het veld 'director' mist bijna 30 procent van de waarden. Dat klinkt alarmerend, maar het is logisch. TV-shows hebben vaak meerdere regisseurs per seizoen. Netflix laat dat veld dan leeg.

Onthoud dit. Dit detail wordt later cruciaal.

De goede nieuws: de essentiële velden - titel, type, release jaar - zijn 100 procent compleet. We kunnen door."

---

# ACT 2: RISING POINTS
*Doel: Bouw spanning op met ondersteunende inzichten die naar het aha-moment leiden*

---

## SLIDE 5: De Explosieve Groei
**Afbeelding:** viz_03_timeline_growth.png
**Tijd:** ~50 seconden

### Spreektekst:
"Nu begint het verhaal echt. Kijk naar deze tijdlijn van Netflix's groei.

Linksboven zie je de jaarlijkse toevoegingen. Tot 2014 was het rustig. Een paar honderd titels per jaar. Maar dan, vanaf 2015, ontploft het. In 2019 voegde Netflix meer dan 2.000 nieuwe titels toe. Dat is gemiddeld 5 tot 6 nieuwe titels per dag.

Maar kijk goed naar de kleuren. Rood zijn films, zwart zijn TV-shows. In de beginjaren domineerde rood. Films waren koning. Maar zie je hoe het zwart groeit? Elk jaar een groter aandeel series.

Rechtsonder zie je de ratio. Die daalt van meer dan 100 films per TV-show naar ongeveer 2 op 1.

Netflix verschuift. Van films naar series. Maar waarom maken ze die keuze?"

---

## SLIDE 6: De Reden - Kijkersretentie
**Afbeelding:** viz_08_duration_analysis.png
**Tijd:** ~45 seconden

### Spreektekst:
"Hier is een deel van het antwoord. Links zie je de verdeling van filmduur. De gemiddelde Netflix-film duurt 100 minuten. Anderhalf uur. Dan is het klaar. De kijker kan weggaan.

Maar kijk rechts. TV-shows hebben seizoenen. En hier is het interessante: 67 procent van alle TV-shows op Netflix heeft maar 1 seizoen. Maar de shows die doorbreken, hebben er 2, 3, soms 10 of meer.

Elke nieuwe aflevering is een reden om terug te komen. Elke cliffhanger houdt je op het platform. Binge-watching werkt alleen met series.

Netflix wil dat je blijft. En series zijn het middel."

---

## SLIDE 7: Van Amerika naar de Wereld
**Afbeelding:** viz_04_geographical_distribution.png
**Tijd:** ~45 seconden

### Spreektekst:
"Maar waar komt al die content vandaan? Deze lollipop chart geeft antwoord.

De Verenigde Staten domineren. Meer dan 3.200 titels, 36 procent van alles. Logisch - Netflix is een Amerikaans bedrijf.

Maar kijk naar nummer twee: India. Meer dan 1.000 titels. Bollywood op Netflix. Dan het Verenigd Koninkrijk, Canada, Japan.

En let op landen als Zuid-Korea en Turkije. Niet in de top 5, maar wel aanwezig. De K-drama's en Turkse series die steeds populairder worden? Die zie je hier terug.

Netflix is niet langer alleen Amerikaans."

---

## SLIDE 8: De Internationale Transformatie
**Afbeelding:** viz_05_international_growth.png
**Tijd:** ~40 seconden

### Spreektekst:
"Dit is misschien wel de meest onthullende grafiek. Het toont het percentage niet-Amerikaanse content over tijd.

Volg de lijn. In 2008 was vrijwel alles Amerikaans. Maar dan begint de stijging. Langzaam eerst, dan steeds sneller.

Zie je die stippellijn op 50 procent? Rond 2016 passeert Netflix die grens. Voor het eerst is meer dan de helft van de nieuwe content internationaal.

In 2018 piek: bijna 70 procent. Netflix transformeerde van een Amerikaans platform naar een écht globaal platform.

Dit is geen toeval. Dit is strategie."

---

## SLIDE 9: De Genre Landschap
**Afbeelding:** viz_06_genre_analysis.png
**Tijd:** ~45 seconden

### Spreektekst:
"Laten we kijken naar genres. Links de top 15 genres op Netflix.

International Movies staat bovenaan met bijna 2.800 titels. Gevolgd door Dramas en Comedies. Klassiekers.

Maar kijk rechts - daar splitsen we het uit per type. En hier worden de patronen zichtbaar.

Die grote rode balk bij International Movies? Dat zijn bijna allemaal films. Maar 'International TV Shows'? Per definitie alleen series.

Sommige genres zijn film-genres. Andere zijn serie-genres. De data begint een verhaal te vertellen."

---

## SLIDE 10: De Genre Race Over Tijd
**Afbeelding:** viz_storytelling_01_bump_chart.png
**Tijd:** ~45 seconden

### Spreektekst:
"Nu een van mijn favoriete visualisaties: de bump chart. Dit toont hoe genre-rankings veranderen over tijd. Elke lijn is een genre. Positie 1 is bovenaan.

Kijk naar de rode lijn: Dramas. Al jaren stabiel op nummer 1. De koning van Netflix.

Maar daaronder is het chaos. Comedies en International Movies wisselen constant van positie. Ze vechten om plek 2 en 3.

En zie je die turquoise lijn onderaan? Documentaries. Die klimt langzaam maar zeker omhoog. Netflix investeert in documentaires - denk aan Tiger King, Making a Murderer.

De smaak verandert. En Netflix past zich aan."

---

## SLIDE 11: Wie Kijkt Wat? - De Rating Analyse
**Afbeelding:** viz_07_rating_analysis.png
**Tijd:** ~40 seconden

### Spreektekst:
"Voor wie is al deze content bedoeld? Deze grafiek toont de leeftijdsratings.

TV-MA - Mature Audiences - domineert met meer dan 3.200 titels. Gevolgd door TV-14. Netflix richt zich primair op volwassenen en tieners.

Rechts zie je het uitgesplitst. Bij zowel films als series domineert content voor adults. Kids content is er, maar het is een kleiner segment.

Netflix is geen kinderplatform. Het is gebouwd voor volwassen kijkers die 's avonds op de bank zitten."

---

## SLIDE 12: Slope Chart - De Verschuiving
**Afbeelding:** viz_storytelling_02_slope_chart.png
**Tijd:** ~40 seconden

### Spreektekst:
"Laten we de verandering concreet maken. Deze slope chart vergelijkt 2017 met 2020.

De Verenigde Staten: van 404 naar 710 titels. Sterke groei, 76 procent.

Maar kijk naar Japan. Van 30 naar 67 titels. Dat is 123 procent groei. Meer dan een verdubbeling. De anime-explosie op Netflix begon hier.

India groeit ook, van 153 naar 193. Zuid-Korea van 42 naar 48.

De helling van elke lijn vertelt een verhaal. Hoe steiler omhoog, hoe harder dat land groeit op Netflix."

---

## SLIDE 13: De Kloof Tussen Films en Series
**Afbeelding:** viz_storytelling_04_dumbbell.png
**Tijd:** ~40 seconden

### Spreektekst:
"Nu wordt het spannend. Deze dumbbell chart toont het verschil tussen films en series per genre.

Rode punt: aantal films. Zwarte punt: aantal TV-shows. De lijn ertussen: het verschil.

Bij Dramas is de kloof enorm. Veel meer films dan series. Comedies hetzelfde.

Maar kijk naar Crime. Daar is het andersom. Meer series dan films. True crime werkt beter als serie. Je wilt het mysterie over meerdere afleveringen ontrafelen.

De lengte van de lijn is het verhaal. Maar wat bepaalt die lengte? Wat maakt dat iets een film wordt en iets anders een serie?

We naderen het antwoord..."

---

# ACT 3: AHA MOMENT
*Doel: Onthul de centrale insight - het keerpunt van het verhaal*

---

## SLIDE 14: De Machine Learning Aanpak
**Afbeelding:** Diagram van het model proces of CRISP-DM
**Tijd:** ~35 seconden

### Spreektekst:
"Om het echte antwoord te vinden, heb ik machine learning ingezet. Specifiek: een Random Forest classifier.

Het proces was als volgt: ik nam alle beschikbare kenmerken - genre, rating, land, release jaar, en meer - en trainde een model om te voorspellen of iets een film of TV-show is.

Niet om Netflix te slim af te zijn. Maar om te begrijpen: welke kenmerken maken het verschil? Wat onderscheidt films van series in de data?

En het antwoord... dat verraste me."

---

## SLIDE 15: DE ONTDEKKING
**Afbeelding:** model_03_feature_importance.png
**Tijd:** ~50 seconden

### Spreektekst:
"Hier is het. Het aha-moment van dit hele onderzoek.

Dit is de feature importance van het model. Het toont welke kenmerken het meeste gewicht hebben bij de voorspelling.

Kijk naar die bovenste balk. 'Heeft Regisseur'. Een importance score van 0,62.

Laat dat even bezinken. Dit ene kenmerk - of er een regisseur in de metadata staat - bepaalt meer dan 60 procent van de voorspelling.

Meer dan genre. Meer dan land van herkomst. Meer dan release jaar. Meer dan alles.

Het geheim van Netflix zit niet in wat ze maken. Het zit in hoe ze hun data registreren."

---

## SLIDE 16: Het Bewijs - Waarom Regisseur?
**Afbeelding:** model_04_feature_analysis.png
**Tijd:** ~50 seconden

### Spreektekst:
"Laat me dit bewijzen met data. Kijk naar de grafiek rechtsboven.

Bij films heeft 97 procent een regisseur vermeld in de metadata. Bijna allemaal. Logisch - een film heeft één regisseur die in de credits staat.

Maar bij TV-shows? Slechts 8,6 procent heeft een regisseur vermeld. Waarom? Omdat series vaak tientallen regisseurs hebben. Elke aflevering een andere. Netflix registreert dat niet op show-niveau.

Dit is geen bug. Dit is hoe Netflix hun database heeft ingericht. En dat systematische verschil? Dat maakt voorspellen mogelijk.

Kijk ook linksonder naar de tijdlijn. Films domineerden vroeger, maar series groeien sneller. Het model vangt ook deze temporele patronen."

---

## SLIDE 17: De Confusion Matrix - Hoe Goed Werkt Het?
**Afbeelding:** model_01_confusion_matrix.png
**Tijd:** ~45 seconden

### Spreektekst:
"Maar werkt het model ook echt? Deze confusion matrix geeft het antwoord.

Links Random Forest, rechts Logistic Regression ter vergelijking. Focus op de diagonaal - dat zijn correcte voorspellingen.

Random Forest: 1.212 films correct voorspeld. 521 TV-shows correct. Op de diagonaal zie je donkere kleuren - dat is goed.

De fouten staan erbuiten. Slechts 14 films foutief als TV-show geclassificeerd. En 14 TV-shows als film.

14 fouten. Op bijna 1.800 voorspellingen. Dat is een foutenpercentage van minder dan 2 procent."

---

## SLIDE 18: De ROC Curve - Technische Validatie
**Afbeelding:** model_02_roc_curve.png
**Tijd:** ~45 seconden

### Spreektekst:
"Voor de technische validatie: de ROC curve. Dit toont de trade-off tussen true positives en false positives.

Links het volledige plaatje. Beide modellen zitten bijna in de linkerbovenhoek. Dat is waar je wilt zijn - hoge true positive rate, lage false positive rate.

Maar de curves lijken bijna identiek. Daarom heb ik rechts ingezoomd op het kritieke gebied.

Nu zie je het verschil. Bij 99 procent correcte voorspellingen heeft Random Forest 8 procent fouten. Logistic Regression heeft 16,6 procent.

Random Forest wint. Niet veel, maar consistent beter."

---

## SLIDE 19: Het Dashboard - Alle Cijfers Samen
**Afbeelding:** model_05_summary_dashboard.png
**Tijd:** ~35 seconden

### Spreektekst:
"Laten we alles samenvatten in één dashboard.

98,4 procent accuracy. Het model voorspelt bijna perfect.

AUC score van 0,996. Op een schaal van 0 tot 1 is dit bijna perfect.

Getraind op 8.803 samples. Genoeg data voor betrouwbare conclusies.

De mini confusion matrix en ROC curve bevestigen: dit model werkt."

---

# ACT 4: SOLUTION & NEXT STEPS
*Doel: Vertaal inzichten naar actie en conclusies*

---

## SLIDE 20: Wat Betekent Dit? - Praktische Implicaties
**Afbeelding:** Bullet points met iconen
**Tijd:** ~45 seconden

### Spreektekst:
"Dus wat betekenen deze bevindingen in de praktijk?

**Voor content strategen:** Als je weet hoe Netflix categoriseert, kun je betere pitch-beslissingen maken. Wil je een serie verkopen? Zorg dat het past bij serie-kenmerken.

**Voor data analisten:** Metadata is geen bijzaak. Hoe een bedrijf data registreert, onthult hun denkwijze. Verborgen patronen hebben voorspellende waarde.

**Voor Netflix zelf:** Jullie data-architectuur is transparanter dan jullie denken. De manier waarop jullie regisseurs registreren, onthult het verschil tussen films en series.

Data vertelt altijd een verhaal. Soms een verhaal dat je niet bewust deelt."

---

## SLIDE 21: De Drie Grote Trends
**Afbeelding:** Infographic met 3 trends
**Tijd:** ~40 seconden

### Spreektekst:
"Uit alle analyses komen drie grote trends naar voren.

**Trend 1: Van films naar series.** Netflix investeert steeds meer in TV-shows. Series houden kijkers langer op het platform. Binge-watching is de strategie.

**Trend 2: Van Amerika naar de wereld.** Internationale content is nu de meerderheid. K-drama's, anime, Europese series - Netflix is globaal geworden.

**Trend 3: Data-structuur onthult strategie.** Het verschil tussen films en series zit niet alleen in de content, maar in hoe Netflix hun metadata organiseert. En dat is voorspelbaar."

---

## SLIDE 22: Beperkingen en Vervolgonderzoek
**Afbeelding:** Tekst of simpele visual
**Tijd:** ~35 seconden

### Spreektekst:
"Geen onderzoek is perfect. Een paar beperkingen om te noemen.

De dataset gaat tot 2021. Netflix's strategie kan sindsdien veranderd zijn.

We kijken alleen naar metadata, niet naar kijkcijfers of reviews. Die data is niet publiek beschikbaar.

En het model voorspelt categorisering, niet succes. Of iets populair wordt, is een andere vraag.

Vervolgonderzoek zou kunnen kijken naar: hoe voorspel je hits? Welke combinatie van kenmerken leidt tot hoge kijkcijfers?"

---

## SLIDE 23: Conclusie - Het Verhaal Compleet
**Afbeelding:** Samenvattende visual of quote
**Tijd:** ~50 seconden

### Spreektekst:
"Laten we het verhaal afronden.

We begonnen met een vraag: wat bepaalt of content een film of TV-show wordt?

We verkenden de data. We zagen Netflix groeien, globaliseren, verschuiven naar series. We analyseerden genres, ratings, duur.

En toen vonden we het antwoord. Niet in de content zelf. Maar in de metadata. In hoe Netflix regisseurs registreert.

Films hebben altijd een regisseur in de database. Series bijna nooit. Dat simpele verschil voorspelt met 98 procent nauwkeurigheid of iets een film of serie is.

Het is een les in data storytelling: soms zit het antwoord niet in de voor de hand liggende data. Soms zit het in de structuur. In wat er mist. In hoe iets geregistreerd wordt.

Data vertelt altijd een verhaal. Je moet alleen leren luisteren."

---

## SLIDE 24: Afsluiting
**Afbeelding:** Bedankslide met naam en eventueel contact
**Tijd:** ~20 seconden

### Spreektekst:
"Dat was mijn data storytelling analyse van Netflix. Van exploratie tot machine learning, van vraag tot antwoord.

Ik hoop dat je iets hebt geleerd over hoe data patronen kan onthullen die je niet verwacht.

Bedankt voor het kijken."

---

# OVERZICHT

## Storytelling Arc Samenvatting

| Fase | Slides | Tijd | Kernboodschap |
|------|--------|------|---------------|
| **Setting & Hook** | 1-4 | ~2:30 min | Introductie Netflix, onderzoeksvraag, data kwaliteit |
| **Rising Points** | 5-13 | ~6:30 min | Groei, internationalisering, genres, ratings, trends |
| **Aha Moment** | 14-19 | ~4:30 min | Model resultaten, de regisseur-ontdekking |
| **Solution & Next Steps** | 20-24 | ~3:00 min | Implicaties, trends, conclusie |

**Totale geschatte tijd: 12-15 minuten**

---

## Slide-Grafiek Overzicht

| Slide | Grafiek | Fase |
|-------|---------|------|
| 3 | viz_02_content_distribution.png | Hook |
| 4 | viz_01_missing_values.png | Hook |
| 5 | viz_03_timeline_growth.png | Rising |
| 6 | viz_08_duration_analysis.png | Rising |
| 7 | viz_04_geographical_distribution.png | Rising |
| 8 | viz_05_international_growth.png | Rising |
| 9 | viz_06_genre_analysis.png | Rising |
| 10 | viz_storytelling_01_bump_chart.png | Rising |
| 11 | viz_07_rating_analysis.png | Rising |
| 12 | viz_storytelling_02_slope_chart.png | Rising |
| 13 | viz_storytelling_04_dumbbell.png | Rising |
| 15 | model_03_feature_importance.png | Aha |
| 16 | model_04_feature_analysis.png | Aha |
| 17 | model_01_confusion_matrix.png | Aha |
| 18 | model_02_roc_curve.png | Aha |
| 19 | model_05_summary_dashboard.png | Aha |

---

## Tips voor de Opname

### Emotionele Curve:
- **Slides 1-4:** Nieuwsgierig, uitnodigend - "Kom mee op reis"
- **Slides 5-13:** Opbouwend, steeds meer hints - "Zie je het patroon?"
- **Slides 14-19:** Enthousiast, onthullend - "Dit is het!"
- **Slides 20-24:** Reflectief, afsluitend - "Wat hebben we geleerd?"

### Belangrijke Pauzes:
1. Na de hook vraag in slide 1 (laat het inzinken)
2. Na "onthoud dit" in slide 4 (foreshadowing)
3. Voor je slide 15 onthult (bouw spanning)
4. Na de "98,4%" reveal (laat het landen)
5. Voor de finale conclusie in slide 23

### Stemgebruik:
- Begin rustig en warm
- Bouw energie op tijdens Rising Points
- Piek bij het Aha Moment
- Eindig kalm en reflectief

### Technische Tips:
- Wijs naar specifieke elementen als je ze noemt
- Maak oogcontact met de camera bij belangrijke punten
- Gebruik je handen om groei/daling aan te geven
