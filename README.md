# Web Typography, Jorinda Waitz, VID 2022/2023

## Ontwerpkeuzes

Typografie: Font

Ik heb ervoor gekozen om gebruik te maken van het Brenner font. Dit font heeft veel verschillende mogelijkheden en dat vond ik een voordeel.

In het eerste fragment hoorde ik drie verschillende stemmen.

Voice1: De “baas” van officer KD6-3.7

Voice2: officer KD6-3.7

Voice3: Collega?

Voor Voice1 heb ik het font “Brenner Mono” gebruikt, maar dit heb ik niet in elke scene hetzelfde gebruikt.
In de eerste scène van voice1 is zijn stem neutraal, maar wel duidelijk en serieus. Daarom heb “Brenner Mono regular” gebruikt.
De tweede scène van voice1, is wanneer officer KD6-3.7 zijn test aflegt. Daar heb ik het font “Brenner mono regular italic” gebruikt. Het is namelijk dezelfde stem als in scene1, maar net wat sneller. Door italic, oogt het wat vlotter, wat past bij de snelheid van praten.
In de derde scène van voice1 heb ik weer “Brenner Mono regular” gebruikt. Hij praat daar weer rustiger, maar wel serieus.
Voor Voice2 heb ik het font “Brenner sans condensed” gebruikt. De stem van officer KD6-3.7 is zwaarder dan voice1 en is daarom dikker. Ook heeft hij niet heel veel emotie in zijn stem en past dit font daar goed bij omdat het simpel en recht is.
Voice3 zegt maar een zin. Hij fluistert “Fuck off, skin-job” snel, maar het heeft een scherpe rand eraan. Daarom heb ik gekozen voor het lettertype “brenner bold italic”. Het is een lettertype met schreef, waardoor je letterlijk dat “scherpe randje” eraan hebt. Verder zegt voice3 het redelijk zacht, maar toch ook hard en snel, daarom heb ik voor bold en italic gekozen.
Typografie: Kleur

Ik heb ervoor gekozen om voice1 geel te maken. Geel heeft namelijk een goed contrast met zwart (de achtergrond). Dit zorgt ervoor dat de tekst goed leesbaar is.

Voice2 heeft een witte kleur. Voice2 is namelijk de hoofdpersoon in de film, dus hij moest een duidelijk contrast hebben met de achtergrond (zwart).

Voice3 heb ik rood gemaakt. Rood en zwart is eigenlijk niet goed voor contrast, maar dat is juist de bedoeling. Hij fluistert namelijk en doordat rood er niet echt uitspringt, krijg je meer het gevoel dat hij het zacht zei. Ook zei hij het op een gemene manier en rood staat onder andere voor woede.

## Web Typography, 2022/2023

Als je doof bent, of als je om een andere reden geen geluid kunt horen, dan mis je veel informatie als je een film kijkt. Knisperende voetstappen, langzaam aanzwellende muziek, nerveus getik op een deur, je hoort het natuurlijk allemaal niet. Nu bestaat er zoiets als _closed caption_, wat een type ondertiteling is waarbij ook dingen als omgevingsgeluiden en de muziek beschreven worden. Hierdoor krijgt een kijker die informatie wel binnen.

Alleen wordt die auditieve informatie nogal neutraal beschreven. Het geluid van huilend persoon zou bijvoorbeeld beschreven kunnen worden als _snikgeluid op de achtergrond_. En iemand die lacht zou geschreven kunnen worden als _iemand lacht._ Heel neutraal, bijna zakelijk, en bovendien allebei in precies hetzelfde neutrale lettertype. Terwijl het toch echt over twee heel verschillende emoties gaat.

Dat kan visueel sterker.

En dat gaan jullie doen.

## Leerdoelen

- Je kan de kennis over vormgeving die je hebt opgedaan tijdens de minor technisch toepassen met behulp van CSS
- Je kan verborgen nuance uit een audiotrack overtuigend vertalen naar visuele (typografische) beelden
- Je kan je typografische keuzes onderbouwen.
- Je hebt de exclusive design principles gebruikt.

## Oplevering

Je levert een werkende versie op, gemaakt met HTML, CSS en JavaScript. Deze staat op Github. In een duidelijke readme documenteer en onderbouw je je ontwerpkeuzes. Je developmentgeschiedenis is terug te vinden op GitHub.

Je levert ook een _screen recording_ met audio op van je fragment. Dit is een video van de definitieve versie, gemaakt van jouw browserscherm.

De beoordeling is mondeling en volgt [de rubric uit het beoordelingsformulier](web-typografie-beoordeling.pdf).

## Typografische restricties

Je _moet_ een van deze twee opties kiezen, en je keuze moet je onderbouwen. In je readme staat een uitleg over je overwegingen om de ene of de andere restrictie te kiezen.

### Optie 1: Systeemfont

De eerste optie is dat je gebruik maakt van het zogenaamde _systeemfont_ van degene die naar jouw werk kijkt. Dit font verschilt per operating system, en het verschilt soms zelfs per versie van het operating system. Het is ook aan te passen door de gebruiker zelf.

Je hebt dus geen controle over welk lettertype er precies gebruikt wordt. Het levert dus een onzeker, en beperkt typografisch palet op. Je hebt geen _light_ versies, of _extrabold_. En ook geen serif en sans-serif versie van dezelfde familie. In dit geval heb je alleen de beschikking over normal, **bold** en _italic_. Dit heeft natuurlijk ook zijn voordelen!

### Optie 2: Brenner

Je kan er ook voor kiezen om gebruik te maken van de complete Brenner familie. Dit is een zeer uitgebreid en uiterst flexibel font. [Hier kan je je verdiepen in dit font](https://www.typotheque.com/blog/brenner_an_unusual_typeface_family_with_distinct_voices). Als je kiest voor dit font dan heb je de beschikking over een _sans serif_, een _condensed_, een _serif_, een _monotype_, een _slab_, een _display_ en een _script_ versie. En veel van deze versies hebben varianten van _light_ tot _bold_, en allemaal zowel _bold_ als _italic_.

Met Brenner zijn er natuurlijk veel en veel meer mogelijkheden dan met systeemfonts. Dat kan zowel een voordeel als een nadeel zijn.

Voor een overzicht, zie [de brenner.pdf](brenner.pdf).

## Het fragment

Ik heb een fragment voorbereid. Het gaat om twee scenes uit _Blade Runner 2049_. De captions staan in de HTML, en ze verschijnen in sync met de video. [Kijk maar](closed-captions/index.html).

### De captions

De captions staan in de html, in het bestand index.html. Je kan aan elke paragraaf eventueel een of meer classes toevoegen. Bijvoorbeeld `voice1` of `voice2 soft`. Classes voeg je handmatig toe in de html.

Met JavaScript worden er een paar dingen extra gedaan:

- er wordt aan elke paragraaf een unieke class toegevoegd (`p0`, `p1`, etc)
- Elk woord wordt in een aparte `span` gezet. Hierdoor kan je elk woord apart stylen, en eventueel ook [na elkaar laten verschijnen](https://github.com/cmda-minor-vid/web-typography-18-19/blob/master/closed-captions/css.css#L41).

### Tijdens het afspelen

Tijdens het afspeelen wordt er een class `on` op de caption gezet als hij moet verschijnen, en een class `off` als hij klaar is. _Zowel class `on` als class `off` blijft op de caption staan!_

De timimg van de captions kan je aanpassen in [closed-captions/captions.js](closed-captions/captions.js).

Er verschijnen ook classes op de body op momenten dat er geluiden worden afgespeeld, zoals `sound1` en `sound2`. Je kan geluiden toevoegen in [closed-captions/sounds.js](closed-captions/sounds.js).

_let op,_ de geluiden zijn niet compleet, dit zal je zelf moeten aanvullen.

## Een eigen fragment (afgeraden, uitgebreide onderbouwing is nodig)

Je kan er ook voor kiezen om een eigen, _beter_ fragment te gebruiken. Dit wordt afgeraden. De tijd die je besteedt aan het zoeken naar dat fragment kan je beter besteden aan het werken aan de opdracht. Bovendien blijkt dat er vaak fragmenten worden gekozen die niet goed voldoen aan de opdracht. Als je een ander fragment kiest dan _moet_ je dit goed onderbouwd voorleggen aan je docent. De deadline hiervoor is vrijdagochtend in de eerste week.

### Waar moet je op letten bij het kiezen van een eigen fragment.

Lees de opdracht nog eens goed door. Waar gaat het ook al weer precies om?

Voor een goede onderbouwing van je keuze voor een ander fragment moet je deze vragen in elk geval beantwoorden:

- Welke informatie zit er in de audio die echt niet zichtbaar is?
- Welke rol speelt de audio in het fragment?
- Werkt de scene nog zonder geluid?
- Waarom is dit fragment beter dan het aangeboden fragment?

Je kan dan de nodige HTML en JavaScript genereren door gebruik te maken van [caption generator](https://cmda-minor-vid.github.io/web-typography-18-19/generator/) (in Google Chrome).

Als je de closed captions wil bewerken dan kan je een tool zoals [Amber Script](https://www.amberscript.com/en) gebruiken. Daar kan je exporteren als `.srt`, en die kan je weer door de generator halen.
