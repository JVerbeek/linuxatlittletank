# `littletank` gebruiken

Hallo, welkom op mijn computer. Dit is een kleine handleiding, omdat de computer *ook* een beetje speciaal is.

## Window managers
Een window manager (WM) is het programmaatje dat je vensters op een bepaalde manier op je scherm schikt.
Een OS zoals Windows heeft naast een WM een desktop environment (DE) wat erop neerkomt dat je een bureaublad hebt waarop je dingen kunt doen. Over het algemeen 
is dit wat gebruiksvriendelijker dan een WM, maar het betekent ook dat je de muis heel veel moet gebruiken om dingen voor elkaar te krijgen. 
Deze computer heeft alleen een WM geinstalleerd en werkt dus niet echt met een bureaublad.

### i3wm
 De window manager op deze computer heet i3wm. [Er is hele goede documentatie voor](https://i3wm.org/),
maar aangezien die moeite kost om door te spitten heb ik hier een korte gids gemaakt om het snel te kunnen besturen.

### Basiscommandos
Als je iets voor elkaar wil krijgen in `i3wm` gaat dit praktisch altijd door een combinatie van een modkey (hierna aangeduid als `Mod`) en een andere toets. 
Wanneer je een programma opstart, word je scherm in kleinere blokjes verdeeld - dit is dus een *tiling window manager*. Er zijn een aantal toetscombinaties gedefinieerd die
standaard bepaalde programma's opstarten:

* `Mod-Enter` - Terminal
* `Mod-F2` - Firefox
* `Mod-D` - Laat een zoekbalk in de bovenste bar zien, waar je je programma in kan typen.

Als je een venster wil sluiten:

* `Mod-Shift-Q` - Gefocuste venster sluiten

Je zult merken dat je scherm in principe horizontaal splitst als je meerdere programma's opstart. Dit kun je veranderen: 

* `Mod-V` - Splits scherm verticaal
* `Mod-H` - Splits scherm horizontaal

Schermen zijn solide als ze 'in focus' zijn, dus dan werk je op dat scherm. Het scherm waar je je muis op beweegt heeft focus.
Focus kan je veranderen met de toetsen,. dat gaat als volgt:

* `Mod-;` - focus naar rechts
* `Mod-J` - focus naar links
* `Mod-K` - focus naar benedenu
* `Mod-L` - focus naar boven

Links bovenin zie je een vierkantje met een cijfer erin, dat is je huidige *workspace*. Workspace management is ook vrij simpel:

* `Mod-cijfer` - open workspace `cijfer`. 
* `Mod-Shift-Cijfer` - verplaats gefocust scherm naar workspace `cijfer`

Verder gaat het grootste deel van de bestandsnavigatie via de terminal `<3`. 

## Manjaro Linux

Nu je weet hoe je deze computer moet navigeren, is het tijd om wat over de OS te leren. Deze computer runt Manjaro Linux. 
Manjaro is voor Arch Linux zoals Ubuntu/Mint voor Debian is.
Het is dus een iets meer user friendly editie van het onderliggende systeem. Je weet alleen dat ik een beetje
masochistische neigingen heb soms, dus ik heb Manjaro geinstalleerd met enkel een window manager als grafische gebruikersinterface. 

Manjaro werkt niet gek veel anders dan wat je gewend bent (waarschijnlijk Ubuntu en Mint). Een groot deel van de reguliere set terminalcommandos is daarom 
hetzelfde als normaal. 
Het grootste verschil is de package manager. In Manjaro heet deze `pacman`. Om iets te installeren run je daarom 
```
sudo pacman -S $naamvanpakket
```

en om iets te verwijderen

```
sudo pacman -R $naamvanpakket
```

Soms bestaan bepaalde packages niet in pacman, die kan je dan installeren via `pamac`,  `git` of via `tar.gz` bestanden, maar we gaan er voor het gemak vanuit dat je dat 
niet nodig hebt. Mocht dat wel zo zijn, dan zijn de instructies op de desbetreffende site meestal adequaat.

### Beschikbare programma's
Zoals genoemd start je programma's met `Mod-D` en typ je de naam van het programma. Als het programma nooit eerder is opgestart stelt het systeem de vraag of je hem
in terminal of in background wil runnen. Eigenlijk wil je programma's met een GUI altijd in background runnen; de uitzonderingen op deze regel zijn van die dingen als `vim` maar 
dat gebruik je denk ik niet. 

* Browser - Firefox
* Text Editor - keuze uit vim, nano of gedit
* Terminal - termite
* Office suite - LibreOffice
* Java
* Python
* Bash
* Lua


