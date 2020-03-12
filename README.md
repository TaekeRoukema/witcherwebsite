Mijn website over The witcher
=============================


## Vragen
### Hoe is deze website gemaakt?
Ik heb de open source CSS library Bootstrap gemaakt. Bootstrap wordt gemaakt door het bedrijf Twitter. Ik heb Bootstrap gekozen omdat er heel veel basis-componenten in zitten maar je kan alsnog erg veel zelf doen. Ik heb niet gekozen voor een template omdat ik het veel leuker vind om de HTML zelf te schrijven, en je leert er ook meer van.

### Waarom heb ik the Witcher gekozen?
Ik heb the Witcher gekozen omdat ik het recent gekezen heb en omdat ik het erg leuk vond. Ik vind het leuk als er een echte wereld gebouwd wordt in de series en dat er altijd iets moois te zien is. Ik ben ook een fan van de videogames en ik ben van plan om de boeken ook te gaan lezen.

### Wat is de structuur van de website?
`index.html` is de homepagina van de website. Vanaf deze homepagina kan je bij alle pagina's komen.
<br>
Bovenaan index.html kan je een artikel zien, als je op de titel of op de link klikt kom je bij `summary.html` Dat is een pagina met alleen het artikel
<br>
`library.html` is een pagina met allemaal foto's van dingen die in de show gebeurt zijn en `witcheruniverse.html` is voor plekken waar je de witcher kunt vinden buiten de Netflix-serie.
<br>
`about.html` is een korte pagina waarin ik uitleg waar the Witcher over gaat.
<br>
`cast.html` en `characters.html` zijn pagina's waarin ik plaatjes en uitleg geef bij de acteurs en de karakters respectievelijk. 

## Code
Bovenaan elke pagina kan je een header vinden die je kunt gebruiken om over de pagina te navigeren, ik heb hier niet veel aan veranderd van wat er al in Bootstrap zit.
```HTML
<nav class="navbar navbar-expand-md navbar-dark fixed-top bg-success">
  <a class="navbar-brand" href="index.html"><img src="Pictures\logo.png" width=30 height=30></a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarCollapse">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item active">
        <a class="nav-link" href="index.html">Home <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="base.html" tabindex="-1" aria-disabled="true">Base</a>
      </li>
    </ul>
    <form class="form-inline mt-2 mt-md-0">
      <input class="form-control mr-sm-2" type="text" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-secondary my-2 my-sm-0" type="submit">Search</button>
    </form>
  </div>
</nav>
```
De jumbotron is het grote ding wat je aan de bovenkant van `index.html` kunt zien. Het is een simpel maar krachtig onderdeel van Bootstrap.
```HTML
<div class="jumbotron">
    <div class="container" align="center">
      <div class="gap-30"></div>
      <h1 class="display-3">The Witcher</h1>
      <p>
        Toss a coin!
      </p>
    </div>
</div>
```
Ik gebruik een bar aan de rechterkant van `index.html` waarmee je over de website kan navigeren.
```HTML
<div class="col">
    <b>Navigate</b>
    <hr>
    <p><a href="about.html">About</a></p>
    <p><a href="characters.html">Characters</a></p>
    <p><a href="cast.html">Cast</a></p>
    <p><a href="witcheruniverse.html">The Witcher Universe</a></p>
    <p><a href="library.html">Library</a></p>
    <p><a href="base.html">base.html</a></p>
    <div class="gap-30"></div>
    <b>Interesting links</b>
    <hr>
    <p><a href="https://en.wikipedia.org/wiki/The_Witcher_(TV_series)">Wikipedia</a></p>
    <p><a href="https://www.imdb.com/title/tt5180504/">IMDB</a></p>
    <p><a href="https://witcher.fandom.com/wiki/Witcher">Fandom</a></p>
    <p><a href="https://thewitcher.com/en">Video Games</a></p>
  </div>
</div>
```
Ik had moeite om de foto's in `library.html` goed in een grid te houden. Daardoor komt het dat als je inzoomt of als je de grootte van de website verandert dat dan de foto's over elkaar heen bewegen.
```HTML
<main role="main" class="container">
  <div class="row">
    <div class="col-sm-3">
      <div class="card" style="width: 18rem">
        <img src="Pictures\library\eyes.jpg" class="card-img-top" alt="The witcher's eyes">
        <div class="card-body">
          <p class="card-text">
            The color of witcher's eyes change based on the situation, in the image above the witcher just defeated a giant monster.
          </p>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card" style="width: 18rem;">
        <img src="Pictures\library\renfri.jpg" class="card-img-top" alt="Renfri">
        <div class="card-body">
          <p class="card-text">Geralt of Rivia meets Renfri in the beginning of the first season of The Witcher.</p>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card" style="width: 18rem;">
        <img src="Pictures\library\yenugly.jpg" class="card-img-top" alt="Yennefer">
        <div class="card-body">
          <p class="card-text">Before Yennefer became the great wizard she is now she was an ugly farmer</p>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card" style="width: 18rem;">
        <img src="Pictures\library\dragon.jpg" class="card-img-top" alt="Dragon">
        <div class="card-body">
          <p class="card-text">This dragon turned out to be a human.</p>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card" style="width: 18rem;">
        <img src="Pictures\library\jaskier.jpg" class="card-img-top" alt="Jaskier">
        <div class="card-body">
          <p class="card-text">Jaskier is known for his cheerful songs.</p>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card" style="width: 18rem;">
        <img src="Pictures\library\ciri.jpg" class="card-img-top" alt="Ciri">
        <div class="card-body">
          <p class="card-text">After Ciri lost everything she had she searched for the witcher who claimed her with the law of surprise.</p>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card" style="width: 18rem;">
        <img src="Pictures\library\calanthe.jpg" class="card-img-top" alt="Queen Calanthe">
        <div class="card-body">
          <p class="card-text">Queen Calanthe learned the consequences of not following conventions.</p>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card" style="width: 18rem;">
        <img src="Pictures\library\striga.png" class="card-img-top" alt="Striga">
        <div class="card-body">
          <p class="card-text">The striga is a very strong monster the witcher almost lost to.</p>
        </div>
      </div>
    </div>
  </div>
  <div class="gap-20"></div>
</main>
```
