# Fix the Flow - Interactive Website

## Code/Design review Programming User Interacion

Deze week heb je geleerd hoe je met behulp van het _JavaScript-drie-stappenplan_ en CSS een interactieve functionaliteit kunt bouwen. Daarbij heb je rekening gehouden met de eindgebruiker door zorgvuldig _feedback_ en _feedforward_ in je ontwerp te integreren.

## Aanpak

Vandaag voer je een Code én Design review uit in een duo voor de repo 'Fix the Flow' van twee andere duo's. Idealiter vorm je een duo met iemand uit een andere groep. Jullie bekijken gezamenlijk, met behulp van een mentor waar nodig, de code van twee andere duo's en jullie bespreken eventuele verbeterpunten. Je reviewt in totaal dus het werk van vier studenten. Deel in Teams in het Draadje 'Code/design review 5 dec' in één reactie de twee repo's van jullie duo. Reageer vervolgens met een emoji op de reactie van een ander duo die jullie gaan reviewen. Zorg ervoor dat elk duo minimaal 1x een review ontvangt. Tip: kies voor het vormen van een duo of bij het selecteren van twee duo's eens iemand anders uit dan waarmee je al veel samenwerkt. 

Gebruik de onderstaande richtlijnen voor de review. Schiet samen issues in waar nodig. Maak voor elk feedback punt een apart issue aan.

### Code-review:
1.  Controleer het JavaScript-bestand en beoordeel of er duidelijke code-comments zijn toegevoegd, zoals beschreven in het kopje [Van Comments naar code](https://github.com/fdnd-task/fix-the-flow-interactive-website/blob/main/docs/programming-user-interaction.md#van-comments-naar-code). Zijn de comments begrijpelijk en helpen ze om de logica van de code te volgen? 
2.   Bekijk de aangemaakte variabelen in het JavaScript-bestand. Geven de namen van de variabelen een goed beeld van wat erin wordt opgeslagen?  
3. Controleer of er styling (CSS) wordt aangepast in het JavaScript-bestand. Indien dit het geval is, maak dan een issue aan om HTML, CSS en JavaScript van elkaar te scheiden in aparte bestanden. HTML moet verantwoordelijk zijn voor de structuur en inhoud van de pagina, CSS voor de opmaak en JavaScript voor de interactiviteit. Bespreek met het team hoe je dit het beste kunt oplossen, bijvoorbeeld door gebruik te maken van de classList.toggle() methode. Wanneer CSS in JavaScript wordt aangepast, kan dit er bijvoorbeeld zo uitzien:

```js
let button = document.querySelector('button');

button.style.color = 'red';

```

### Design-review:
1. Analyseer met elkaar hoe de feedforward is toegepast in het ontwerp. Begrijpt de gebruiker meteen wat er zal gebeuren bij interactie met het element? Bespreek in jouw duo of er visuele of tekstuele verbeteringen mogelijk zijn om dit te verduidelijken.
2. Beoordeel hoe feedback is verwerkt in de interactie. Is het voor de gebruiker duidelijk wat er gebeurt nadat een interactie heeft plaatsgevonden? Zijn de signalen die feedback geven (bijvoorbeeld kleurveranderingen, meldingen of animaties) logisch?  
3. Maak een issue aan hoe de interactie nog vetter, functioneler of toegankelijker gemaakt kan worden. Gebruik hiervoor jullie verbeeldingskracht. Het mag out-of-the-box zijn!  
