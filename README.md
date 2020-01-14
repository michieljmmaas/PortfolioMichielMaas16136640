# Portfolio Michiel Maas - 16136640 - Danone Powerplant

## Informatie

### Datacamp
Ik heb alle verplichte Datacamp opdrachten gedaan. Zien de onderstaande afbeelding als bewijs. 
![Datacamp](Sources/datacamp.png "Datacamp Overzicht")

Ik heb bij een eerder blok van van de HBO-ICT: Software Engineering opleiding al deze precieze opdrachten gemaakt. Daarom was het best wel saai, en ik heb ik een beetje gehaast. 

## Subjects
### Research Project
#### Aanpak
Voor dit onderzoek moesten wij kijken naar het optimalizeren van de energie productie van een Renewable Powerplant. Danone wilde graag een 'groene' energie centrale maken, maar dan het liefst zo goedkoop en effiecient mogelijk. Dit is lastig omdat de energie productie van zonnenpanelen en windturbines verschilt over het jaar, en de fabriek het hele jaar door een constante hoeveelheid energie nodig heeft om te blijven draaien. 
De energie die geproduceerd word door deze zonnepanelen en windturbines kan worden opgeslagen, maar dat is heel prijzig. Voordat Danone wilde beginnen aan het project wilde eerst graag goed weten hoe duur het zou worden en wat de beste manier was om dit te doen. 

Wij moesten dus kijken naar: 
> Een powerplant die alleen energie opwekt met zonnenpanelen en windturbines. Deze energie moet genoeg zijn om de fabriek het hele jaar draaiend te houden. En dit alles voor zo min mogelijk geld. 

Hieruit leidde onze onderzoeksvraag: 
> "How can a genetic algorithm be used to determine the most cost effective configuration for a renewable powerplant?".

Gelukkig was er al wat werk voor ons gedaan. Arie Taal, van de Energie in Transition research group, had een simulatie waarin we energie productie van een opstelling van zonnenpanelen en windturbines over een jaar konden berekenen. We hadden dus en manier van hoe we van een **opstelling** naar een **resultaat** konden komen, maar we wilde het andersom. We hadden al het **resultaat** maar wilde daar de **opstelling** van weten. We moesten dus een manier bedenken om  dit uit te vinden. 

Donnely en ik hebben even gebrainstormd over de dingen die wij konden doen, en de manieren om het aan te pakken. Ik stelde voor om een genetisch algoritme te gebruiken, omdat we dit goede toepassing was en ik er wat [ervaring me had in een eerder blok](Sources/Travelling Salesman.java "Travelings Salesman Problem opgelost in Java voor Game of Trades"). Een genetisch algoritme is een goede oplossing voor dit systeem omdat we het eigenlijk proberen te 'bruteforecen'. We willen zo veel mogelijk configuraties proberen totdat we de goede hebben, maar dan wel op een slimme manier. 
Dit is precies wat een genetisch algoritme doet. Door allemaal verschillende dingen uit te proberen, en deze resultaten te beoordelen op hun correctheid kan je het algoritme de goede kant op duwen. 

Donneley was erg ijverig en had het algoritme al snel af. Dit was fijn want hierdoor konden we snel de data analyseren. Maar voor de andere groepsgenoten die met het algoritme en de code moesten werken was het nog best ingewikkeld. Ik heb Aurin en Luc veel geholpen door het Algoritme van Donnely goed uit te leggen zodat ze er mee aan de slag konden. Ook met het goed schrijven van code zodat het makkelijk samenwerkt met andere delen en het programma. 

#### Resultaten
De resulaten waren best wel interessant. Sommige dingen haden we verwacht:
* Windturbines zijn erg rendabel en werden dus veel gebruikt
* De optimale hoek en orientatie van zonnenpanelen is ongeveer 37 graden gericht op het zuiden
* In de zomer wordt er veel meer energie opgewekt dan in de winter. 

Zie deze afbeelding van de GUI die ik heb gemaakt voor een overzicht:
![Energieproductie](Sources/GUI_Afbeeldingen/EnergieProductie.PNG "Cummulatieve Energie Productie en configuratie")

Maar wat ons zeker opviel dat er weinig wordt opgeslagen. Dit is omdat de huidige prijs van opslag enorm duur is. Het algoritme berekend dat het goedkoper is om meer zonnenpanelen neer te zetten zodat het zelfs in de wintermaanden genoeg kan produceren om de nacht door te komen. 
Dit zorgt er op zijn beurt weer voor dat het in zomer veel meer produceert dan nodig. In totaal produceert de hele opstelling 150 keer zo veel energie als nodig is, en dit is erg inefficient.  
Je kan ook duidelijk zien dat er een periode is in het begin van het jaar waar de productie erg laag is, en daar veel batterij voor moet gebruiken. Maar de rest van het jaar wordt de batterij bijna niet gebruikt. 
![AccuGebruik](Sources/GUI_Afbeeldingen/AccuGebruik.PNG "Accu gebruik")

Wat enorm veel geld kan schelen is om op moment waar de productie erg laag is, en de batterijen leeg zijn, stroom in te kopen van het net. Dit is een factor waat we niet naar hebben gekeken, en misschien voor een vervolg onderzoek een goede stap is. 
En andere stap is misschien kijken naar het doorverkopen van de over geproduceerde stroom. Dit kan veel geld opleveren en de opstelling nog voordeliger maken. 

#### Scrum
Persoonlijk ben ik erg fan van planning en overzicht, dus nam ik al snel te taak van Product Owner op me. Ik heb de volgende stappen genomen om het project in goede banen te leiden:
* Ik heb een grote backlog gemaakt van alles dat we moesten 
* Ik heb een gedetailleerd planning gemaakt van wanneer we welke sprint wilden starten
* Ik heb een Scrum Board gemaakt waarop de we taakjes konden bijhouden
* Ik heb een Trello aangemaakt waarop alle project genoten hun taakjes konden bijhouden en informatie konden delen. 

De eerste 2 sprintens gingen erg goed. Ik heb de sprint review geleid en de taken telkens verdeeld. Mensen die hulp nodig hadden konden dat goed aangeven en de taken liepen makkelijk door. Maar toen Donnely het algoritme aan het eind van de tweede week af waren er nogmaar weinig grote taken te verdelen. 
Onderhand waren de taken ookal duidelijk verdeeld en hielden project genoten zich vooral bezig met hun eigen doelen en was er niet heel veel vraag meer na de sprint planningen. Toen onze planning na twee maanden werd gevandaliseerd, en het verlengsnoer uit onze werkruimte werd gestolen, was er niet heel veel vraag meer deze taken. 

#### Git
Als enige Software Engineering student uit het groepje, was ik een enorme voorstander om Github te gebruiken. In de eerste week de [GitHub Repository](https://github.com/michieljmmaas/PowerPlantHHS) opgezet, en de benodigde instelling toegepast. Ik had het ingesteld dat mensen niet direct naar de master konden pushen, zodat die vrij was van merge conflicts. Groepsgenoten moesten een merge request aanmaken om hun stukjes code aan de master toe te voegen. Deze code kon dan controleren, en eventuele merge conflict oplossing. Ik heb vooral Aurin en Luc veel geholpen om hun code goed te verwerken door hun onbekendheid met Git.
 In totaal zijn er 320 commits gemaakt, 63 merge requests verwerkt. 
 
### Communication
#### Presentaties
Ik gaf in het begin van de periode al aan dat ik goed was in Engels en weinig problemen heb met presenteren. Dit kwam goed van pas omdat er in de groep ook mensen waren die liever niet presenteerden. Ik bood me regelmatig aan om te presenteren, en ben zelfs een paar keer last-minute (terwijl andere groepjes al aan het presenteren waren) ingesprongen toen een projectgenootje te laat was, of het programma niet aan de praat kregen. De presentaties die ik heb gegeven zijn:

* [9 December - Maandag presentatie](Sources/Presentaties/Renewable_power_plant_9_december.pptx)
* [1 November - Milestone presentatie](Sources/Presentaties/Renewable_power_plant_1_november.pptx)
* [14 Oktober - Maandag presentatie](Sources/Presentaties/Renewable_power_plant_14_oktober.pptx)
* [27 September - Milestone presentatie](Sources/Presentaties/Renewable_power_plant_27_september.pptx)

#### Research Paper
Nadat we de meeste research hebben gedaan is het skelet van de paper opgesteld. Alle kopjes werden aangemaakt zodat de project genoten de konden aanvallen. Ik heb samen met Aurin gekeken naar de papers die hij had gevonden, om te beslissen welke het beste aansloegen op wat we wilden schrijven. 
In de tussentijd hebben we veel feedback gekregen van onze opdracht gever, Arie Taal, en begeleider van de Groene Mient Groep, Baldiri Salcedo. Ik heb me best gedaan deze feedback zo goed mogelijk toe te passen op wat we hadden geschreven en benodigde stukken om te schrijven zodat het aan gewenste opmaak voldeed. 
Nadat alle kopjes waren ingevuld, we de alle benodigde resultaten hadden verzameld en alle feedback was verwerkt hebben de paper gezamenlijk verbeterd. De paper wordt op een bescherm getoond, en samen beslisten we hoe we dingen wilde verwoorden. Mijn engels skills kwamen hier goed van pas om de zinnen goed te laten verlopen.  

Omdat het schrijven van de paper voornamelijk gezamenlijk ging is het moeilijk om aan te toenen welke dingen ik precies heb gedaan op dit punt. 

 


### Data prepocessing

The student properly examined and visualized the data, distributions, outliers, correlations and used that analysis to give directions for an early hypothesis.

The student cleansed the data in a good and sufficient way.  

The student prepared the data in an appropriate way, where necessary transforming data, removing outliers, filling in missing values, etc.

The student described the the entire dataset  in a good and sufficient way.  

The student correctly visualized the data in support of decisions made for learning the model


### Predictive Analytics
The student has supported their model selection with references from literature
The student explains why the chosen configuration is reasonable (for instance using relevant literature)
The student takes appropriate countermeasures to prevent under- and overfitting and tunes hyperparameters
The student compares several models and additionally explains the differences between the models.
The student has visualized the results both quantatively in a plot and where applicable qualitatively using examples.

### Linken code: 
GUI bestanden
Aanpassen van de paramters in het mee geven

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

