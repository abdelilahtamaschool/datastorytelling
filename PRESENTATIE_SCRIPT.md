# Netflix Data Storytelling - Presentatie Script

> Dit script is bedoeld voor een video-opname. Lees de tekst onder elke slide rustig voor. Tijdsindicaties zijn suggesties.

---

## SLIDE 1: Titelpagina
**Afbeelding:** Netflix logo of dashboard screenshot
**Tijd:** ~20 seconden

### Spreektekst:
"Welkom bij mijn data storytelling presentatie over Netflix. Vandaag neem ik jullie mee in een analyse van bijna 9.000 titels op Netflix. We gaan ontdekken welke patronen er in de data zitten, en ik laat zien hoe een machine learning model kan voorspellen of nieuwe content een film of een TV-show wordt."

---

## SLIDE 2: De Onderzoeksvraag
**Afbeelding:** viz_02_content_distribution.png
**Tijd:** ~30 seconden

### Spreektekst:
"Laten we beginnen met de centrale vraag van dit onderzoek: **Kunnen we voorspellen of nieuwe content een film of TV-show wordt?**

Kijk naar deze grafiek. Netflix heeft 8.807 titels in de catalogus. Daarvan is bijna 70 procent een film, en ruim 30 procent een TV-show. Dat is een interessante verdeling. Maar de vraag is: wat maakt een film een film, en een serie een serie? Welke kenmerken bepalen dat? Daar gaan we achter komen."

---

## SLIDE 3: Data Kwaliteit Check
**Afbeelding:** viz_01_missing_values.png
**Tijd:** ~25 seconden

### Spreektekst:
"Voordat we kunnen analyseren, moeten we de datakwaliteit checken. Deze grafiek toont hoeveel data er mist per kolom.

Wat opvalt: bij 'director' mist bijna 30 procent van de data. Dat klinkt veel, maar het is logisch. TV-shows hebben vaak meerdere regisseurs per seizoen, dus dat veld blijft vaak leeg. De belangrijke velden zoals titel, type en release jaar zijn gelukkig 100 procent compleet."

---

## SLIDE 4: De Explosieve Groei van Netflix
**Afbeelding:** viz_03_timeline_growth.png
**Tijd:** ~40 seconden

### Spreektekst:
"Nu wordt het interessant. Deze grafiek vertelt het verhaal van Netflix's groei.

Kijk naar de linkerbovenkant: tussen 2015 en 2019 zie je een explosie aan nieuwe content. In 2019 alleen al voegde Netflix meer dan 2.000 nieuwe titels toe. Dat is meer dan 5 titels per dag.

Maar let ook op de verhouding. De rode balken zijn films, de zwarte zijn series. In het begin domineerden films. Maar kijk naar de laatste jaren: het aandeel TV-shows groeit. Netflix investeert steeds meer in series. Waarom? Omdat series kijkers langer vasthouden. Je bingewatcht een serie, niet een film."

---

## SLIDE 5: Van Amerika naar de Wereld
**Afbeelding:** viz_04_geographical_distribution.png
**Tijd:** ~35 seconden

### Spreektekst:
"Waar komt al die content vandaan? Deze lollipop chart geeft het antwoord.

De Verenigde Staten domineren met meer dan 3.200 titels. Dat is 36 procent van alles op Netflix. India staat tweede met ruim 1.000 titels, gevolgd door het Verenigd Koninkrijk.

Maar hier zit een verhaal. Netflix begon als een Amerikaans platform. Nu zie je landen als Zuid-Korea, Japan en Turkije opkomen. De K-drama's en anime die je kent? Die zie je hier terug in de data."

---

## SLIDE 6: De Internationale Transformatie
**Afbeelding:** viz_05_international_growth.png
**Tijd:** ~30 seconden

### Spreektekst:
"Dit is misschien wel de meest opvallende grafiek. Het toont het percentage niet-Amerikaanse content over tijd.

Zie je die stippellijn op 50 procent? Rond 2016 gebeurde er iets bijzonders. Netflix passeerde die grens. Voor het eerst kwam meer dan de helft van de nieuwe content van buiten Amerika.

In 2018 was bijna 70 procent internationaal. Netflix transformeerde van een Amerikaans platform naar een écht globaal platform. Dat is een strategische keuze die je hier in de data kunt zien."

---

## SLIDE 7: Genre Ranking Race
**Afbeelding:** viz_storytelling_01_bump_chart.png
**Tijd:** ~35 seconden

### Spreektekst:
"Nu een van mijn favoriete visualisaties: de bump chart. Dit is een race tussen genres over tijd.

Elke lijn is een genre. De positie op de Y-as toont de ranking. Bovenaan staat nummer 1.

Kijk naar de rode lijn: Dramas. Die blijft al jaren op nummer 1. Stabiel. Maar kijk naar de zwarte lijn, Comedies. Die wisselt voortdurend met International Movies om plek 2 en 3.

En zie je die turquoise lijn onderaan? Dat zijn Documentaries. Die stijgen langzaam maar zeker. Netflix investeert duidelijk meer in documentaires."

---

## SLIDE 8: Slope Chart - Wie Groeit het Snelst?
**Afbeelding:** viz_storytelling_02_slope_chart.png
**Tijd:** ~30 seconden

### Spreektekst:
"Deze slope chart vergelijkt 2017 met 2020. Links zie je hoeveel titels elk land produceerde in 2017, rechts in 2020.

De Verenigde Staten gingen van 404 naar 710 titels. Indrukwekkend. Maar kijk naar Japan. Van 30 naar 67 titels. Dat is een groei van 123 procent. De anime-explosie die je op Netflix ziet? Die begon hier.

De helling van de lijn vertelt het verhaal. Hoe steiler omhoog, hoe sneller de groei."

---

## SLIDE 9: Movies vs TV Shows per Genre
**Afbeelding:** viz_storytelling_04_dumbbell.png
**Tijd:** ~30 seconden

### Spreektekst:
"Deze dumbbell chart toont iets fascinerends. De rode punt is het aantal films, de zwarte punt het aantal TV-shows. De lijn ertussen toont het verschil.

Bij Dramas is het verschil enorm. Veel meer films dan series. Hetzelfde voor Comedies. Maar kijk naar Crime. Daar draait het om. Meer TV-shows dan films. Denk aan true crime series. Die zijn populairder als serie dan als film.

De lengte van de lijn is het verhaal. Hoe langer, hoe groter het verschil."

---

## SLIDE 10: Het Machine Learning Model - Introductie
**Afbeelding:** model_05_summary_dashboard.png
**Tijd:** ~35 seconden

### Spreektekst:
"Nu het machine learning gedeelte. Ik heb een Random Forest model getraind om te voorspellen of content een film of TV-show is.

Dit dashboard vat de resultaten samen. Kijk naar die grote rode cijfers bovenaan. 98,4 procent accuracy. Het model voorspelt bijna perfect.

De AUC score is 0,996. Dat is bijna 1, wat perfect zou zijn. Het model is getraind op bijna 9.000 voorbeelden. Dat is genoeg data om betrouwbare voorspellingen te maken."

---

## SLIDE 11: Confusion Matrix - Hoe Goed Voorspelt het Model?
**Afbeelding:** model_01_confusion_matrix.png
**Tijd:** ~35 seconden

### Spreektekst:
"De confusion matrix toont exact waar het model goed en fout zit.

Links zie je Random Forest, rechts Logistic Regression ter vergelijking. Kijk naar de diagonaal - dat zijn de correcte voorspellingen. 1.212 films correct voorspeld, 521 TV-shows correct.

De fouten staan off-diagonal. Slechts 14 films werden foutief als TV-show geclassificeerd, en 14 TV-shows als film. Dat is een heel laag foutenpercentage."

---

## SLIDE 12: ROC Curve - De Technische Validatie
**Afbeelding:** model_02_roc_curve.png
**Tijd:** ~30 seconden

### Spreektekst:
"Voor de technische validatie: de ROC curve. Links het volledige plaatje, rechts ingezoomd op het kritieke gebied.

Beide modellen zitten bijna in de linkerbovenhoek. Dat is waar je wilt zijn. Het betekent: hoge true positive rate, lage false positive rate.

De ingezoomde view rechts toont het subtiele verschil. Bij 99 procent correcte voorspellingen heeft Random Forest 8 procent fouten, Logistic Regression 16,6 procent. Random Forest wint."

---

## SLIDE 13: Feature Importance - Wat Bepaalt het Verschil?
**Afbeelding:** model_03_feature_importance.png
**Tijd:** ~40 seconden

### Spreektekst:
"Dit is de belangrijkste grafiek voor interpretatie. Welke kenmerken gebruikt het model om films van series te onderscheiden?

Nummer 1, met grote voorsprong: 'Heeft Regisseur'. Een importance van 0,62. Dat betekent dat dit kenmerk alleen al meer dan 60 procent van de voorspelling bepaalt.

Waarom? Simpel. Bijna alle films hebben een regisseur in de metadata. Bij TV-shows is dat maar 8 procent het geval. Series hebben vaak meerdere regisseurs, dus dat veld blijft leeg.

Nummer 2: het genre 'International TV Shows'. Logisch - als iets dat label heeft, is het per definitie een TV-show."

---

## SLIDE 14: Feature Analysis - Dieper Inzoomen
**Afbeelding:** model_04_feature_analysis.png
**Tijd:** ~35 seconden

### Spreektekst:
"Laten we dieper inzoomen op die belangrijkste features.

Linksboven: het 'International TV Shows' genre. Nul procent van de films heeft dit, 50 procent van de series wel. Een perfecte scheiding.

Rechtsboven: regisseur informatie. 97 procent van de films heeft dit, slechts 9 procent van de series. Dat verklaart waarom dit de sterkste voorspeller is.

Rechtsonder: de tijdslijn. Films domineerden vroeger, maar na 2015 groeien TV-shows sneller. Het model pikt ook deze temporele patronen op."

---

## SLIDE 15: Conclusies
**Afbeelding:** Bullet points of samenvattende visual
**Tijd:** ~40 seconden

### Spreektekst:
"Wat hebben we geleerd?

Ten eerste: Netflix's catalogus is filmgedomineerd, maar de trend verschuift naar series. Series houden kijkers langer vast.

Ten tweede: Netflix transformeerde van een Amerikaans naar een globaal platform. Internationale content is nu de meerderheid.

Ten derde: het model toont aan dat films en series fundamenteel anders zijn in de metadata. Het verschil zit hem vooral in hoe Netflix de regisseur-informatie vastlegt.

Met 98,4 procent accuracy kunnen we voorspellen of nieuwe content een film of serie wordt. Dat is nuttig voor content-strategie en catalogusbeheer."

---

## SLIDE 16: Afsluiting
**Afbeelding:** Bedankt slide of contact info
**Tijd:** ~15 seconden

### Spreektekst:
"Dat was mijn data storytelling analyse van Netflix. Van exploratie tot machine learning, de data vertelt een duidelijk verhaal over hoe Netflix evolueert.

Bedankt voor het kijken."

---

## Technische Notities voor de Opname

### Aanbevolen Slide Volgorde:
1. Titelpagina
2. Onderzoeksvraag (viz_02)
3. Data Kwaliteit (viz_01)
4. Timeline Groei (viz_03)
5. Geografische Distributie (viz_04)
6. Internationale Groei (viz_05)
7. Bump Chart (viz_storytelling_01)
8. Slope Chart (viz_storytelling_02)
9. Dumbbell Chart (viz_storytelling_04)
10. Model Summary (model_05)
11. Confusion Matrix (model_01)
12. ROC Curve (model_02)
13. Feature Importance (model_03)
14. Feature Analysis (model_04)
15. Conclusies
16. Afsluiting

### Tips voor de Opname:
- Spreek rustig en duidelijk
- Pauzeer even bij elke nieuwe grafiek zodat kijkers kunnen oriënteren
- Wijs naar specifieke elementen in de grafiek wanneer je ze noemt
- Totale geschatte tijd: 7-9 minuten

### Grafieken die je NIET hoeft te gebruiken:
- viz_09 t/m viz_13 (minder essentieel voor het verhaal)
- viz_storytelling_03 (radial bar - optioneel, al veel genre-grafieken)
