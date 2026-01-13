# Netflix Data Storytelling - Presentatie Script V2

> Gestructureerd volgens de **Data Storytelling Arc**: Setting & Hook → Rising Points → Aha Moment → Solution & Next Steps

---

# ACT 1: SETTING & HOOK
*Doel: Pak de aandacht, introduceer het probleem*

---

## SLIDE 1: De Hook
**Afbeelding:** Netflix logo of startscherm
**Tijd:** ~30 seconden

### Spreektekst:
"Stel je voor: je bent content manager bij Netflix. Elke dag moet je beslissen over duizenden nieuwe titels. Wordt dit een film? Of maken we er een serie van?

Die beslissing bepaalt alles. Het budget. De marketing. Hoe lang kijkers blijven hangen.

Maar wat als ik je vertel dat er een patroon zit in die keuzes? Dat we met data kunnen voorspellen wat Netflix gaat doen... met 98 procent nauwkeurigheid?

Vandaag ontrafelen we dat geheim."

---

## SLIDE 2: Het Speelveld
**Afbeelding:** viz_02_content_distribution.png
**Tijd:** ~25 seconden

### Spreektekst:
"Dit is ons speelveld. 8.807 titels op Netflix. Bijna 70 procent daarvan zijn films. 30 procent TV-shows.

Maar waarom die verhouding? Is het toeval? Of zit er een strategie achter?

Om dat te ontdekken, moeten we dieper in de data duiken."

---

# ACT 2: RISING POINTS
*Doel: Bouw spanning op met ondersteunende inzichten*

---

## SLIDE 3: De Stille Revolutie
**Afbeelding:** viz_03_timeline_growth.png
**Tijd:** ~40 seconden

### Spreektekst:
"Hier begint het interessant te worden. Kijk naar deze tijdlijn.

Tussen 2015 en 2019 explodeerde Netflix. Van een paar honderd titels naar duizenden per jaar. In 2019 alleen al: meer dan 2.000 nieuwe titels. Dat is 5 per dag.

Maar let op de kleuren. Rood zijn films, zwart zijn series. In het begin: bijna alleen films. Maar kijk naar de laatste jaren... het zwart groeit.

Er is iets aan het veranderen. Netflix verschuift. Maar waarom?"

---

## SLIDE 4: De Globalisering
**Afbeelding:** viz_05_international_growth.png
**Tijd:** ~35 seconden

### Spreektekst:
"Hier is nog een puzzelstuk. Deze grafiek toont het percentage internationale content over tijd.

Zie je wat er rond 2016 gebeurt? Netflix passeert de 50 procent grens. Voor het eerst komt meer dan de helft van de content van buiten Amerika.

In 2018 is bijna 70 procent internationaal. K-drama's uit Korea. Anime uit Japan. Telenovela's uit Mexico.

Netflix werd een wereldspeler. En dat heeft gevolgen voor wat ze maken."

---

## SLIDE 5: De Genre Race
**Afbeelding:** viz_storytelling_01_bump_chart.png
**Tijd:** ~35 seconden

### Spreektekst:
"Kijk naar deze race tussen genres. Elke lijn is een genre, de positie toont de ranking.

Drama's - de rode lijn - blijven al jaren nummer 1. Stabiel aan de top.

Maar kijk naar wat eronder gebeurt. Comedies en International Movies vechten om plek 2. En die turquoise lijn onderaan? Documentaires. Die klimmen langzaam omhoog.

De smaak van kijkers verandert. En Netflix past zich aan.

Maar we hebben het echte geheim nog niet gevonden..."

---

## SLIDE 6: Een Vreemd Patroon
**Afbeelding:** viz_storytelling_04_dumbbell.png
**Tijd:** ~30 seconden

### Spreektekst:
"Kijk eens naar deze grafiek. Rood is films, zwart is series. De lijn ertussen toont het verschil.

Bij Drama's: enorm veel meer films dan series. Bij Comedies hetzelfde.

Maar kijk naar Crime. Daar is het andersom. Meer series dan films.

Waarom? Wat bepaalt of iets een film of serie wordt?

De data wijst naar iets. Iets wat we bijna over het hoofd zagen..."

---

# ACT 3: AHA MOMENT
*Doel: Onthul de centrale insight*

---

## SLIDE 7: De Ontdekking
**Afbeelding:** model_03_feature_importance.png
**Tijd:** ~45 seconden

### Spreektekst:
"En hier is het. Het aha-moment.

Ik trainde een machine learning model om films van series te onderscheiden. En dit is wat het model ontdekte.

Kijk naar die bovenste balk. 'Heeft Regisseur'. Een importance van 0,62. Dat betekent: dit ene kenmerk bepaalt meer dan 60 procent van de voorspelling.

Meer dan genre. Meer dan land. Meer dan release jaar.

Het geheim zit in de regisseur."

---

## SLIDE 8: Het Bewijs
**Afbeelding:** model_04_feature_analysis.png
**Tijd:** ~40 seconden

### Spreektekst:
"Laat me het bewijzen. Kijk rechtsboven.

97 procent van alle films op Netflix heeft een regisseur in de metadata. Maar bij TV-shows? Slechts 9 procent.

Waarom? Simpel. Een film heeft één regisseur. Die staat in de credits. Maar een serie heeft vaak tientallen regisseurs - elke aflevering een andere. Netflix laat dat veld dan leeg.

Het is geen toeval. Het is een systematisch verschil in hoe Netflix hun data structureert.

En dat verschil? Dat is voorspelbaar."

---

## SLIDE 9: De Resultaten
**Afbeelding:** model_05_summary_dashboard.png
**Tijd:** ~30 seconden

### Spreektekst:
"Het model werkt. 98,4 procent accuracy. Van bijna 9.000 titels voorspelt het model correct of iets een film of serie is.

De AUC score is 0,996. Bijna perfect.

We hebben het patroon gekraakt."

---

# ACT 4: SOLUTION & NEXT STEPS
*Doel: Geef concrete aanbevelingen en vervolgstappen*

---

## SLIDE 10: Wat Betekent Dit?
**Afbeelding:** Bullet points of infographic
**Tijd:** ~35 seconden

### Spreektekst:
"Dus wat betekent dit voor de praktijk?

**Voor content strategen:** Je kunt voorspellen hoe Netflix nieuwe content zal categoriseren. Dat helpt bij pitch-beslissingen.

**Voor data analisten:** Metadata-structuur is geen bijzaak. Het bevat verborgen patronen die grote voorspellende waarde hebben.

**Voor Netflix zelf:** De manier waarop je data vastlegt, onthult je strategie. Bewust of onbewust."

---

## SLIDE 11: De Grotere Trend
**Afbeelding:** viz_storytelling_02_slope_chart.png
**Tijd:** ~30 seconden

### Spreektekst:
"En de trend is duidelijk. Kijk naar deze slope chart.

Amerika groeit, maar Japan groeit sneller. Van 30 naar 67 titels - meer dan 100 procent groei.

Netflix's toekomst is internationaal. En steeds meer van die internationale content zal series zijn. Series houden kijkers langer vast. Dat is de strategie.

De data vertelt het verhaal."

---

## SLIDE 12: Afsluiting - De Reis
**Afbeelding:** Data Storytelling Arc diagram of samenvattend beeld
**Tijd:** ~25 seconden

### Spreektekst:
"We begonnen met een vraag: wat bepaalt of content een film of serie wordt?

We ontdekten patronen in groei, geografie en genres. En toen vonden we het antwoord: het zit in de metadata. In hoe Netflix regisseurs registreert.

Een simpel dataveld. Een krachtig inzicht. 98 procent voorspelkracht.

Dat is de kracht van data storytelling.

Bedankt voor het kijken."

---

# SAMENVATTING: De Storytelling Arc

| Fase | Slides | Doel | Kernboodschap |
|------|--------|------|---------------|
| **1. Setting & Hook** | 1-2 | Aandacht pakken | "Wat als we Netflix's keuzes kunnen voorspellen?" |
| **2. Rising Points** | 3-6 | Spanning opbouwen | Groei, globalisering, genre-shifts - er is een patroon |
| **3. Aha Moment** | 7-9 | Centrale insight | "Het geheim zit in de regisseur metadata!" |
| **4. Solution & Next Steps** | 10-12 | Actie en conclusie | Praktische implicaties en de grotere trend |

---

# Tips voor de Opname

### Emotionele Curve:
- **Slides 1-2:** Nieuwsgierig, vragend
- **Slides 3-6:** Opbouwend, steeds meer hints
- **Slides 7-9:** Enthousiast, de "eureka"
- **Slides 10-12:** Reflectief, concluderend

### Pauzes:
- Pauzeer NA de hook vraag (laat het inzinken)
- Pauzeer VOOR je het aha-moment onthult
- Pauzeer NA de 98,4% reveal

### Geschatte Tijd: 6-8 minuten
