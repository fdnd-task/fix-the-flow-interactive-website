# Fix the Flow - Interactive Website

## Navigeren en labels

Navigatie is de manier waarop de gebruiker door een website kan surfen en zoeken. 
Als een gebruiker op jouw website komt vraagt die zich af: 
Wat is er, waar ben ik en waar kan ik naartoe? 
Je helpt de gebruiker door "antwoord" te geven op die vragen ... met feedback en feedforward!

In het boek *Designing Web Navigation* schrijft James Kalbach:

- Navigatie geeft toegang tot de informatie op een website

- Navigatie toont waar je bent op een website

- Navigatie toont waar de website over gaat

- Navigatie laat het merk zien

- Navigatie zorgt voor geloofwaardigheid

<!--
> Keep users in control by regularly surfacing system status, by describing causation (if you do this that will happen) and by giving insight into what to expect at every turn 
>
> - Joshua Porter, Principles of User Interface Design
-->

### Aanpak

Eerst ga je leren wat straatnaambordjes en bewegwijzering in web design zijn, en waar je op moet letten als je iconen en labels gebruikt. 

Daarna ga je in groepjes de interactie die je aan het ontwerpen en bouwen bent bespreken.

## Straatnaambordjes en bewegwijzering.

Goede navigatie maakt gebruik van feedback en feedforward, dat zijn de straatnaambordjes en bewegwijzering van een website.
_Feedback_ is dat een gebuiker weet _“waar”_ die is. _Feedforward_ laat zien waar de gebruiker _“naartoe”_ kan.

Op de website van Ziggo.nl zijn het logo, de titel van de pagina en het oranje menu-item Straatnaambordjes, ze geven aan waar de gebruiker zich bevindt. Bewegwijzering zijn bijvoorbeeld de menu-items, daarmee kan een gebruiker ergens 'naartoe':
![Straatnaambordjes en bewegwijzering op ziggo.nl](ziggo-straatnaambordjes-en-bewegwijzering.png)


## Iconen en labels

Voor het gebruik van iconen is het aan te raden bij het icon altijd een label te gebruiken. Zoals de input elementen in een formulier hebben alle interactieve elementen duidelijke labels nodig.

![](hamburger-menu-types-examples.jpeg) *Verschillende menu icons voor dezelfde interactie.*

Online zul je vaak zien dat menu knoppen of andere interactieve elementen geen labels hebben. Dan geef je de gebruiker geen duidelijke feedback en feedforward. Er zijn geen regels voor het gebruik van iconen, dus zul je vaak zien dat dezelfde iconen worden gebruikt voor andere doeleinden, of verschillende iconen voor dezelfde interactie. Om misverstanden te voorkomen, is het aan te raden om bij een icon _altijd_ een label te plaatsen. Om duidelijk te maken wat het betekent en wat een gebruiker kan verwachten.

### Hoe ontwerp je goede labels?

**Begrijpbare terminologie** ‘gebruikersnaam’ i.p.v. ‘userid’. Gebruik geen jargon, dat is voor experts en je weet niet of jouw gebruiker dat is.

**Gebruik precieze en nauwkeurige woorden** Precieze woorden is dus niet ‘voer  gegevens in’, maar benoem welke gegevens moeten worden ingevuld, wees concreet. Gebruik alleen afkortingen als de gebruiker ze kent, mensen schamen zich wanneer ze de afkortingen niet kennen.

**‘Do...with’** Mensen zijn taakgericht, dus “Print deze brief”, “Koop festival tickets”. Als Do…with teveel ruimte in beslag neemt, doe dan alleen een werkwoord. Wanneer je buttons labeled, dan zegt vijf keer een OK op een pagina niets, wel Print, Zoek, Bestel, Opslaan, Aanmelden.

**Labels niet laten overlappen** Labels mogen niet overlappen (qua betekenis), want dan moet een gebruiker beide uitproberen om er achter te komen wat het betekent. Bv. de links Agenda en Activiteiten of Agenda en Kalender naast elkaar.

### Bronnen

- [Icon Usablity](https://www.nngroup.com/articles/icon-usability/)
- [Yes, Icons Need Text Labels](https://www.nngroup.com/videos/icon-text-labels)

<!--
#### Design patterns en mental models

Design patterns: hamburger, carousel, progressive disclosure.

Hide and cry.

Alternatieven ontwerpen, schetsen op Whiteboard

Wat zit er in? Mental model?
https://lawsofux.com/mental-model/
https://www.nngroup.com/articles/mental-models/

-->

### Opdracht User test bespreken

Bespreek de testresultaten van de user test die je hebt gedaan met een mentor en 3 studenten. Bespreek de interacties en testen om en om, laat zien wat je hebt getest, wat goed ging en wat nog verbeterd kan worden. (Heb je nog geen user test gedaan, doe dan eerst alsnog de [user test van vrijdag](code-design-review-user-testing.md).)

<!--
*Heb je de test en de testresultaten goed beschreven in het issue?*
-->

Schets gezamenlijk hoe je de interactie kan verbeteren door feedback en feedforward toe te passen:

- Let op het gebruik van straatnaambordjes en bewegwijzering, noteer deze in de tekening. 
- Let op het gebruik van labels en iconen en pas toe hoe je goede labels ontwerpt.
- Schets ook de hover-, active- en focus-states van de interactieve elementen.
- Voeg de tekening met uitleg toe aan het issue met de user story en interactie. (Als je die nog niet hebt, kijk dan nog even naar de [workshop User Interface Design](user-interface-design.md))


<!-- 

### Structural navigation

Voor deze opdracht ga je de _Structural navigation_ van jouw opdracht schetsen.

Navigatie is de manier waarop de gebruiker door een website kan surfen en zoeken. Wat is er, waar ben ik en waar kan ik naartoe?
Er zijn drie verschillende soorten navigatie: _Structural navigation_, _Associative navigation_ en _Utility navigation_.

<img width="880" alt="image" src="https://user-images.githubusercontent.com/1391509/146066136-afca4b34-85bd-46cf-afa0-82a5a5b1ca36.png">

_Structural Navigation_ is super belangrijk voor de gebruikers, bezoekers van jouw website stellen zichzelf een aantal vragen, zoals: Is dat wat ik zoek op deze pagina? Waar is het? Hoe kan ik mijn taak volbrengen? De _Structural navigation_ zorgt hiervoor. 

Voordat je de _Structural navigation_ kan schetsen moet je eerst weten welke structuur een website heeft. Welke pagina's zijn er en wat is de hiërarchische structuur?


1. Teken alle pagina's van jouw opdracht op post-its
2. Structureer alle pagina's op een logische hiërarchische manier met een sitemap. 
3. Bepaal de top-level pagina's en sub-level pagina's. Misschien heeft jouw site ook sub-sub-level, geef dat ook aan.


### Ontwerpen

Als je weet wat de top-level pagina's en de sub-level pagina's zijn kun je de _Structural navigation_ schetsen. 
_Structural navigation_ verbindt de verschillende pagina's van een website met elkaar volgens de hiërarchische structuur. Op elke pagina moet een gebruiker naar de 'bovenliggende' pagina en naar de 'onderliggende' pagina's kunnen browsen.

Schets op basis van de top-level pagina's een menu voor de _Structural navigation_ 

1. Schrijf voor elke top-level pagina een passend label om te gebruiken in het menu
2. Bepaal een logische volgorde van de menu items 
3. Schets het menu voor de _Structural navigation_
4. Bepaal de active state, de in-active states en de hover state van de menu elementen zodat de gebruiker weet waar die is en waar die heen kan 

#### Bronnen

- [Designing Web navigation - Chapter 4. Types of Navigation](https://www.oreilly.com/library/view/designing-web-navigation/9780596528102/ch04.html)
- [Presenting Information Architecture - Site diagrams](https://www.webstyleguide.com/wsg3/3-information-architecture/4-presenting-information.html)

## Criteria

De Structural Navigation opdracht is *done* als

- [ ] Er is een Sitemap waarin de pagina's op een logische hiërarchische manier gestructureerd zijn
- [ ] Er is een menu getekend met passende labels en een logische volgorde van de menu items
- [ ] De verschillende states van een menu item zijn goed weergegeven, active state, de in-active states en de hover state
- [ ] De opdracht is gedocumenteerd in de Readme van de leertaak

Focus sprint 5 - De focus van deze sprint ligt op navigatie en informatie architectuur van een website. Organiseren en structureren van informatie, Design Patterns toepassen, Navigatie, filteren en zoekstrategieën, Micro Interacties.
-->
