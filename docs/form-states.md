# Fix the Flow - Interactive Website

## Forms en states

Feedback en Feedforward leren ontwerpen en bouwen voor formulieren. 

In Sprint 4 ben je begonnen met het maken van formulierelementen. Misschien heb je er ook al een paar toegepast voor je opdrachtgever; filters, een contactformulier, een zoekveld, een chatformulier, een reactieformulier, etc. Met een goede basis in HTML maak je ze voor iedereen _Toegankelijk_ en bruikbaar. En met CSS zorg je dat de verschillende _states_ in de huisstijl van de opdrachtgever vormgegeven worden.

In HTML kun je ook al een aantal extra regels meegeven als attribuut. Of een invoerveld vereist is bijvoorbeeld (met het `required` attribuut). Hiermee voegen we _validatie_ aan een formulier toe (niet te verwarren met HTML validatie, wat weer wat anders is). Deze extra validatieregels zorgen ervoor dat een formulier prettiger te gebruiken is. Browsers bieden een hoop extra's in CSS en JS rondom het valideren van formulieren.

Probeer na deze workshop de nieuwe kennis over formuliervalidatie toe te passen in je huidige project.


## Aanpak

We gaan weer een klein experiment maken: een formulier met daarin een vereist element. Als je het formulier probeert te versturen, valideert de browser het formulier, en toont deze een standaard melding. Dit ziet er in verschillende browsers verschillend uit. De standaard teksten verschillen ook per browser.

En aangezien we net met JavaScript en _events_ zijn begonnen, gaan we de standaard feedback van de browser aanpassen, zodra er een `invalid` event wordt afgevuurd door de browser.

![](required.png)

![](required-radios.png)


## Verschillende browsers

Als frontender is het verstandig om zoveel mogelijk browsers te verzamelen, ook op je telefoon. Jouw eindgebruikers hebben _waarschijnlijk_ namelijk ook een andere browser dan jij.

![](browsers.jpg)

Dus download [Firefox](https://www.firefox.com/), [Chrome](https://www.google.com/chrome/), [Arc](https://arc.net/download), [Edge](https://www.microsoft.com/edge/), [Vivaldi](https://vivaldi.com/download/), [Brave](https://brave.com/download/), [Samsung Internet](https://www.samsung.com/nl/apps/samsung-internet/), [Polypane](https://polypane.app/), [Orion](https://orionbrowser.com/), [Dolphin](https://dolphin.com/), [Zen Browser](https://zen-browser.app/), [LibreWolf](https://librewolf.net/), [Servo](https://servo.org/download/) etc.

Maar ook [Safari Technology Preview](https://developer.apple.com/safari/technology-preview/) (als je op een Mac zit), [Firefox Nightly](https://www.firefox.com/channel/desktop/), [Chrome Canary](https://www.google.com/chrome/canary/), [Edge Canary](https://www.microsoft.com/edge/download/insider) en [Brave Nightly](https://brave.com/download-nightly/), zodat je als frontender klaar bent om nieuwe technieken uit te proberen.

Schrijf met je tafel op het whiteboard welke browsers jullie geïnstalleerd en uitgeprobeerd hebben. De tafel met de meeste browsers krijgt een cookie melding.


## Formuliervalidatie in HTML

Maak een nieuw HTML bestand in je _i-love-web_ repo, genaamd `validatie.html` (tussen al je andere experimenten). Voeg hier de volgende HTML aan toe.

```html
<form>
  <label>Zoekterm <input required></label>
  <button type="submit">Zoek!</button>
</form>
```

Om de formuliervalidatie van een browser te kunnen gebruiken, heb je altijd een `<form>` tag nodig. De styling maakt voor dit voorbeeld niet uit. Onderaan deze workshop staan nog een aantal bronnen voor het vormgeven en stylen van goede formulierelementen, mocht je deze nodig hebben in je project.

Sla je HTML op en probeer het formulier te versturen in verschillende browsers.

### Bronnen

- [Client-side form validation: Using built-in form validation @ MDN](https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation#using_built-in_form_validation)
- [Form Validation Part 1: Constraint Validation in HTML @ CSS Tricks](https://css-tricks.com/form-validation-part-1-constraint-validation-html/)


## Het `invalid` event gebruiken

Zoals je deze en vorige week hebt geleerd, biedt je browser een hoop _events_. Je kunt naar events luisteren met `addEventListener`. Zo hebben formuliervelden een `invalid` _event_, dat wordt afgevuurd zodra de browser een veld niet door de validatie laat komen. Je kunt vervolgens vragen aan de browser _waarom_ dat veld _invalid_ was, maar je kunt ook de feedback op dat moment aanpassen. Zet bijvoorbeeld het volgende script in je HTML. Meestal doen we dat via een apart bestand, maar voor kleine experimenten werkt dit ook:

```html
<script type="module">
// Stap 1: zoek de input en stop die in een variabele
let inputElement = document.querySelector('input');

// Stap 2: luister naar het invalid event, en wacht tot dat afgevuurd wordt..
inputElement.addEventListener('invalid', function(ev) {

  // Stap 3: pas de tekst in de validatiemelding aan
  inputElement.setCustomValidity('Dit veld mag niet leeg zijn hoor..');

});
</script>
```

Sla dit op, en test het in je nieuwe favoriete browser. Met JavaScript kun je dus aangepaste feedback geven!

Om het echt goed te krijgen, moet je nog wat extra werk doen, maar je weet nu in ieder geval hoe je het driestappenplan op een totaal ander onderwerp en _event_ kunt toepassen. Als je hier meer mee wilt doen in de opdracht voor de opdrachtgever, of in je eigen I Love Web website, klik dan vooral door naar de bronnen op MDN.

### Bronnen

- [setCustomValidity() method @ MDN](https://developer.mozilla.org/en-US/docs/Web/API/HTMLInputElement/setCustomValidity)
- [input.validity property @ MDN](https://developer.mozilla.org/en-US/docs/Web/API/HTMLInputElement/validity)
- [ValidityState @ MDN](https://developer.mozilla.org/en-US/docs/Web/API/ValidityState)
- [invalid event @ MDN](https://developer.mozilla.org/en-US/docs/Web/API/HTMLInputElement/invalid_event)
- [Form Validation Part 2: The Constraint Validation API (JavaScript) @ CSS Tricks](https://css-tricks.com/form-validation-part-2-constraint-validation-api-javascript/)


## Feedback van formuliervelden vormgeven en stylen

Vooral de `:user-invalid` en `:user-valid` _pseudo-classes_ werken goed samen met bovenstaande HTML en JS. Vrijwel alles rondom de feedback en feedforward van formuliervalidatie is met deze bouwstenen te maken. Zeker als je `:has()` hierin combineert. Voeg dit bijvoorbeeld eens toe aan je HTML, en probeer het formulier te versturen. Meestal voegen we CSS toe via een extern bestand, maar voor kleine experimenten werkt dit ook:

```html
<style>
fieldset:has(:user-invalid) {
  background: #faa;
}
</style>
```

<img src="sorry-but-no.png" width="386" height="175" alt="" loading="lazy">

Formuliervelden zelf consistent vormgeven is een vak apart, en biedt soms uitdagingen. Hieronder staan een aantal bronnen, die je gaan helpen bij het oplossen van styling problemen. Lees ook vooral het eerste artikel door, als je meer wilt leren over wat formuliervelden _usable_ maakt.

### Bronnen

- [Form design; Best practice, research insights and examples](https://gerireid.com/forms.html)
- [Styling web forms @ MDN](https://developer.mozilla.org/en-US/docs/Learn/Forms/Styling_web_forms)
- [UI pseudo-classes @ MDN](https://developer.mozilla.org/en-US/docs/Learn/Forms/UI_pseudo-classes)
- [:user-invalid @ MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/:user-invalid)
- [:user-valid @ MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/:user-valid)
- [:has() @ MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/:has)
- [Advanced form styling @ MDN](https://developer.mozilla.org/en-US/docs/Learn/Forms/Advanced_form_styling)

💡 Wist je trouwens dat checkboxjes en radio elementen al meer dan 30 jaar die vorm hebben? En dat veel mensen dus gewend zijn aan de _feedforward_ die vierkantjes en rondjes binnen formulieren bieden?

- [In Loving Memory of Square Checkbox](https://tonsky.me/blog/checkbox/)


## Extra uitdaging?

Voeg de volgende HTML toe aan `validatie.html`:

```html
<form>
  <fieldset>
    <legend>Selecteer een optie</legend>

    <label><input type="radio" name="option" required> Optie 1</label>
    <label><input type="radio" name="option" required> Optie 2</label>
    <label><input type="radio" name="option" required> Optie 3</label>

    <input type="submit" value="Verstuur">
  </fieldset>
</form>
```

Door radio inputs dezelfde `name` en een `required` attribuut te geven, worden die ook gevalideerd tijdens een _form submit_. Test de standaard formuliervalidatie van de browser en probeer ook deze tekst te overschrijven met JavaScript. Hou er rekening mee dat je `setCustomValidity()` ook weer moet aanroepen met een lege string (`''`), omdat je hiermee de browser validatie overschreven hebt.
