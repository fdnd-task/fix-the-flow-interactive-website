# Fix the Flow - Interactive Website

## User Interface Events

Als een gebruiker interactie heeft met een website, moet je goede feedback tonen zodat een gebruiker weet of de actie gelukt is. 

Om een interactie te coderen gebruik je in javascript het 3 stappenplan. Eerst moet je het element in de DOM selecteren waar je iets mee wil, daarna koppel je daar een event aan, daarna kan je met een CSS class feedback tonen. 

### UI Events

In een browser zijn veel verschillende vormen van interactie mogelijk. Deze worden User Interface Events (UI Events) genoemd.

Met _UI Events_ kan je met javascript gebruikersinteractie afhandelen, zoals muis, touch en toetsenbord.

Zo kan je bijvoorbeeld iets doen als een gebruiker op een button klikt:

```html
<button class="show-more">Toon meer</button>
```

```js
let showMoreButton = document.querySelector('.show-more');

showMoreButton.addEventListener('click', function(){
    //feedback tonen   
});
```

### Oefenen met UI Events

Om te oefenen met verschillende UI Events, animatie en feedback, hebben we de deeltaak "UI Events" voor je klaargemaakt. Alles wat je hierin leert, kun je daarna toepassen in deze leertaak, voor je opdrachtgever.

Voer de [UI Events deeltaak](https://github.com/fdnd-task/ui-events/) uit, en ga daarna door met de leertaak.



### Bronnen

- [If you only know one thing about JavaScript, this is what I would recommend](https://css-tricks.com/video-screencasts/150-hey-designers-know-one-thing-javascript-recommend/)
- [UI Events @ MDN](https://developer.mozilla.org/en-US/docs/Web/API/UI_Events)
