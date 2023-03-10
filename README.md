# CSS to the Rescue @cmda-minor-web 2022 - 2023

Live demo: [firework](https://hoa0.github.io/css-to-the-rescue-2223/firework/index.html)

Bekijk mijn Wiki op [notion](https://special-sprite-fab.notion.site/Css-to-the-rescue-Wiki-6ccdc58539af4b65bc33ac9bca37684e)

## Week 1

### Gekozen opdracht:

Voor het vak CSS to the Rescue heb ik als eindopdracht 'magische vuurwerkshow' uitgekozen. Waarbij ik nieuwe CSS technieken ga experimenteren en uiteindelijk een website met magische dynamische vuurwerkshow ga realiseren.

### Met welke CSS-technieken ga je als eerste aan de slag?

Als eerst ben ik met CSS ‘background-image’ property aan de slag geweest, hiermee kan ik de achtergrond van het vuurwerkshow meer interessante body meegeven. Door het toepassen van achtergrondeffecten. Zoals de functie ‘linear-gradient’ meegeven, die zorgt ervoor dat de overgang tussen twee of meer opgegeven kleuren vloeiend verlopen. Ook is het mogelijk om de kleuren verloop specifiek aan te geven waar het moet beginnen.

## Waar liggen je (grootste) uitdagingen?

- golven animeren

## Ontwerp-schetsen + breakedown-schets

<img src="https://github.com/Hoa0/css-to-the-rescue-2223/blob/main/firework/imgWiki/schets-week1-css.png" width="600">

> Een vuurwerkshow bij het strand

### Bronnen

- [CSS gradient generator](https://mycolor.space/gradient)
- [Background-image](https://developer.mozilla.org/en-US/docs/Web/CSS/background-image)
- [Linear-gradient](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient/linear-gradient)

## Week 2

### Voortgang

<img src="https://github.com/Hoa0/css-to-the-rescue-2223/blob/main/firework/imgWiki/svg-waves.png" width="600">

<img src="https://github.com/Hoa0/css-to-the-rescue-2223/blob/main/firework/imgWiki/vuurpijl.png" width="600">

### Wat ging er soepel en wat was lastig?

Deze week ben ik verder gegaan met het toevoegen van strand elementen, zoals de zon en zee. Daarnaast heb ik ook een input check toegevoegd om van dag en nacht te kunnen verwisselen en een vuurpijl. Het toevoegen van deze elementen had ik geen problemen mee, behalve bij het creëren van een bewegende zee.

### Welke experimenten heb je gedaan die mislukt zijn?

Voor het creëren van de zee golven heb ik css before en after gebruikt en css keyframes toegepast om de golven te laten bewegen. Echter is het mij niet gelukt om een realistische zee te nabootsen in css hiermee, Dit kwam doordat ik moeite had met de positie plaatsen van de golven. Daarna heb ik nog even geprobeerd met een SVG-element, ook dit lukte niet met css.

### Heb je nieuwe inzichten hoe je de kracht CSS kunt benutten (of juist niet)?

In een korte tijd heb ik nieuwe inzichten gekregen over de kracht van CSS:

CSS: `CSS ::before ::after ` <br>
Met deze css element kun je voor en na een element interessante content toevoegen, zonder dat dit in de HTML hoeft te staan. Door het uitbreiden van css kan je deze vorm geven door het meegeven van content:””.

Stukje code waarbij ik dit heb toegepast:
In plaats van drie div-elementen te gebruiken, heb ik één label tag gebruikt om de vuurpijl te maken.

```Css
/* create the flare top*/
label::before {
 content: "";
 position: absolute;
 top: -2.2em;
 left: -0.78em;
 border-top: 1.2em solid transparent;
 border-right: 1.2em solid transparent;
 border-bottom: 1.2em solid #ff2727;
 border-left: 1.2em solid transparent;
}
```

CSS: `CSS radial-gradient() ` <br>
Met deze functie kun je een kleurverloop maken dat vanuit een middelpunt vanuit alle richtingen uitstraalt. Je kunt variabelen zoals kleur, startpunt en stoppunt instellen om het uiterlijk van je kleurverloop te bepalen. De wwardes kunnen een "circle" of "ellipse" zijn. Dit heb ik toegepast voor de zon.

```CSS
/* de zon*/
 main > div:nth-of-type(2){
 background: radial-gradient(
   ellipse at center,
   #ffd000 1%,
   #f9b700 39%,
   #f9b700 39%,
   #e06317 100%
 );
 height: 4em;
 width: 4em;
 border-radius: 50%;
 }
```

CSS `CSS has() ` <br>
Themasessie has() gevolgd

### Neem wijzigingen aan je 1e plan op.

Voor de volgende keer, laat ik de bewegende zee achterwegen en zoek ik naar andere mogelijke opvulling die past bij mijn thema. Ook wil ik css code refactoren en nieuwe css inzichten implementeren die ik deze week heb opgedaan tijdens de les.

### Waar liggen je (nieuwe) uitdagingen voor komende week?

- Animatie toevoegen aan de vuurpijl
- Vuurwerk weergeven

## Bronnen

- [waves animate](https://dev.to/patilganesh1010/a-complete-guide-to-waves-bmb)
- [waves voorbeeld](https://codepen.io/Prachl/pen/XLveVd)
- [radial-gradient()](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient/radial-gradient)
- [has()](https://developer.mozilla.org/en-US/docs/Web/CSS/:has)

## Week 3

### Voortgang

<img src="https://github.com/Hoa0/css-to-the-rescue-2223/blob/main/firework/imgWiki/wk3.png" width="600">

### Wat ging er soepel en wat was lastig?

Wat ging goed? <br>

- Animatie toevoegen aan de vuurpijl
- Code refactoren, input ~ checked vervangen met has() selector en customer properties
- SVG toevoegen

Wat ging minder goed?

- Zelf een vuurwerk maken

### Welke experimenten heb je gedaan die mislukt zijn?

### Heb je nieuwe inzichten hoe je de kracht CSS kunt benutten (of juist niet)?

- animeren

### Neem wijzigingen aan je 1e plan op.

### Waar liggen je (nieuwe) uitdagingen voor komende week?

- Achtergronden smooth weergeven wanneer het veranderd
- Verschillende soorten Vuurwerk laten zien
- Meer Vuurwerk producten creeren

### Bronnen

- [vuurwerk animatie](https://alvaromontoro.com/blog/68002/creating-a-firework-effect-with-css)

## Week 4

## Het eindresultaat

uitleg:..
<img src="https://github.com/Hoa0/css-to-the-rescue-2223/blob/main/firework/imgWiki/wk4-1.png" width="600">

<img src="https://github.com/Hoa0/css-to-the-rescue-2223/blob/main/firework/imgWiki/wk4-2.png" width="600">

### Wat ging er soepel, wat was lastig en waar ben je trots op?

Wat ging er goed? <br>

- meer vuurwerk elementen gemaakt

### Welke experimenten heb je gedaan die mislukt zijn?

### Heb je nieuwe inzichten hoe je de kracht CSS kunt benutten (of juist niet)?

### Waar wil je meer mee gaan doen?
