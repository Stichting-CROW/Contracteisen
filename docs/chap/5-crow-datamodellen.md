# CROW-datamodellen

In de volgende secties worden de classes en relaties toegelicht uit 2 datamodellen van CROW:

1. Het CROW Specificatieschema <a>CSPEC</a>: volgens dat schema worden de specificaties gestructureerd. Dit schema wordt door CROW gebruikt voor het publiceren van de Standaard RAW Bepalingen als de RAW Catalogus Bepalingen.
2. Het CROW Documentschema: <a>CDOC</a>: dit model beschrijft de publicatiestructuur voor de CROW Basisspecificaties en de resultaatsbeschrijvingen. De specificaties van de Standaard RAW Bepalingen en de RAW Catalogus Bepalingen volgen de structuur van hoofdstuk, deelhoofdstuk, paragraaf en artikel. De CROW specificaties van de RAW Catalogus Resultaatsbeschrijvingen opgebouwd volgens werkcategorie, subwerkcategorie en romptekst.

De datamodellen zijn te vinden op de [GitHub omgeving](https://github.com/Stichting-CROW/Contracteisen), onder de noemers:

- SpecificatieSchema_v\*\*\*.ttl
- DocumentSchema_v\*\*\*.ttl

<p class="note" title="Eisen aan data van derden">
	<i>In relatie tot de eisen die we stellen aan data van derden kan CROW uiteraard ook besluiten bepaalde data-inhoud niet mee te nemen in de publicatie. Bijvoorbeeld omdat de markt er nog niet rijp voor is of omdat de keuzes stand heden nog te arbitrair zijn en niet robuust genoeg voor software(ontwikkeling).
	</i>
  </p>

<p class="note" title="Eisen en specificaties">
	<i>Als in deze ReSpec gesproken wordt over eisen en niet over specificaties, is dat om taalgebruik niet teveel geweld aan te doen. Het zou daardoor minder toegankelijk worden. Ter illustratie: we hebben het in Nederland meestal over verschillende soorten eisen. Dus niet ‘functiespecificatie’ bijvoorbeeld, maar ‘functie-eis’, etc..</i>
  </p>

## Classes

Deze sectie geeft een overzicht van alle classes binnen de CROW-datamodellen

<p class="ednote" title="This section will undergo changes soon">
	Deze concepten en definities in deze secties zijn onderwerp van discussie
  </p>

### CSPEC Classes

In <!--TODO-->sectie is een overzicht gegeven van de concepten (classes) die zijn gebruikt in het CROW datamodel. Concepten zijn allerlei ‘dingen’ die zijn gebruikt in de data modellen. De definities van die ‘dingen’ zijn eveneens opgenomen in de betreffende sectie. De concepten van <a>CSPEC</a> zijn hier in alfabetische volgorde weergegeven.

#### `Activiteit`

<dfn>Activiteit</dfn> is iets dat gebeurt

Toelichting: <i>Activiteiten zijn vereenzelvigd met werkwoorden. Bij het structuren en aanbrengen van betekenisvolle relaties spelen naast zelfstandige naamwoorden (objecten), werkwoorden (activiteiten) een belangrijke rol. </i>

#### `Begrip`

<dfn>Begrip</dfn> geeft een bepaald ding aan

Toelichting: <i>Definities binnen de context van een onderwerp voor objecten, activiteiten, hulpmiddelen of overig. Definities voor objecten en activiteiten zijn relevant voor de semantische relaties tussen eisen, objecten en activiteiten. Voorkeurstermen en synoniemen worden gebruikt. Als er een objectdefinitie is met een URI (Uniform Resource Identifier) die overeenkomt met een object in RAW wordt die URI gebruikt als voorkeursterm; een eventuele objectnamen met een gelijke betekenis als synoniem. Een voorbeeld daarvan is een rioleringsobject dat door Rioned al is gedefinieerd en gekoppeld aan een URI met een gelijke betekenis als in RAW.
</i>

#### `Collectie`

<dfn>Collectie</dfn> is een verzameling van dingen die bij elkaar horen.

#### `Dataset`

<dfn>Dataset</dfn> is een collectie van bibliotheekdata die zijn gepubliceerd om contracten mee op te stellen.

Toelichting: <i>CROW heeft het over bibliotheekdata en niet over projectspecifieke data(sets). De datasets kunnen een verschillende bron hebben: CROW, Provincie etc.. Bij data(set) die specifiek voor een project is gegenereerd, spreken we over een contract(data)set.</i>

#### `Eenheid`

<dfn>Eenheid</dfn> is de dimensie van de grootheid waarin een aspect wordt uitgedrukt.

Toelichting: <i>Het concept ‘Eenheid’ komt voor in de RAW Catalogus Resultaatsbeschrijvingen. Die catalogus kan worden beschouwd als een productcatalogus met allerlei (deel)objecten c.q. bouwstoffen. Een deel van de objecten heeft een dimensie: een ‘Eenheid’.</i>

#### `Fase`

<dfn>Fase</dfn> is een periode als onderdeel van een langere ontwikkeling.

Toelichting: <i>In de levenscyclus van een object worden een aantal fasen onderscheiden: initiatief, ontwerp, realisatie, gebruik en sloop.</i>

#### `Functie`

<dfn>Functie</dfn> is een potentieel meetbare prestatie van een object/systeem.

Toelichting: <i>Een andere verwoording: functie is de beoogde werking en verrichting van een product of dienst. In de datamodellering is volstaan met functies op systeemniveau (of hoofdstukniveau). Zo is wel de functie beschreven van een rioolstelsel maar niet van allerlei in te kopen onderdelen van een rioolstelsel. Functie-eisen zijn eisen aan te realiseren functies; zij geven aan ‘wat het systeem moet kunnen doen’.</i>

#### `Methode`

<dfn>Methode</dfn> is een vaste weldoordachte manier van handelen om een bepaald doel te bereiken.

Toelichting: <i>Het concept ‘Methode’ verificatie- of validatiemethoden aan een specificatie te kunnen koppelen.</i>

#### `Object`

<dfn>Object</dfn> is een door de mens geproduceerd of gerealiseerd voorwerp, constructie, bouwwerk.

Toelichting: <i>Een object is een ‘ding’. Een afzonderlijk identificeerbaar onderdeel van een fysiek geheel. </i>
<br>Het is <b>geen</b> object als het een van onderstaande ook kan zijn:

- Een verzameling
- Een samenstelling van twee objecten (deze is arbitrair)
- Een proces of activiteit
- Een Norm
- Een woord eindigt op -ing. bebakening, voorziening, bewapening, inrichting. Dit zijn gevaarlijke woorden en ‘verboden’ als naam van een object. Het zijn groepen dingen.
- Een object dat een bepaalde status meekrijgt, zoals bestaande ankerstang.

#### `Raakvlak`

<dfn>Raakvlak</dfn> is het punt, aspect of gebied dat twee objecten gemeen hebben.

Toelichting: <i>Stand heden is er voor gekozen om ‘raakvlakken’ aan te maken voor RAW-bibliotheekdata. Zo kan worden volstaan met het koppelen van de eis aan dit raakvlak (in het voorbeeld van een raakvlakeis tussen twee objecten, kan zo worden volstaan met 1 koppeling i.p.v. een koppeling van de raakvlakeis aan twee objecten). Voorbeeld: Riolering en Verharding: eisen die worden gesteld aan het hoogteverschil tussen de bovenkant van putten en kolken t.o.v. de (geprojecteerde) verharding.</i>

#### `Specificatie`

<dfn>Specificatie</dfn> is een nadere aanduiding waaraan een product moet voldoen.

Toelichting: <i>Woordgebruik eis en specificatie wordt nogal eens door elkaar gebruikt in spreek- en schrijftaal. Ook in dit document dat dient als ‘toelichting op….’. Formeel is een specificatie hetzelfde als een eis, mits opgenomen in een contract. Als onderdeel van een (specificatie)bibliotheek dus niet. </i>

#### `Specificatiecategorie`

<dfn>Specificatiecategorie </dfn> is een categorie waar een specificatie toe kan behoren.

Toelichting: <i>Een specificatie is van een bepaalde type. De specificatiecategorieën die worden onderscheiden zijn: functie-eis, aspecteis, objecteis, raakvlakeis en proceseis. Het gebruik van specificatiecategorie wordt nader toegelicht in [deze sectie](#specificatiecategorie).
</i>

#### `Status`

<dfn>Status</dfn> is de stand of toestand van iets.

Toelichting: <i>Status geeft de kwaliteitsaanduiding aan van een (deel)specificatie of document. Bijvoorbeeld status ‘concept, ‘vastgesteld’ of ‘vervallen’.</i>

### CDOC Classes

De concepten van <a>CDOC</a> zijn hier in een logische volgorde weergegeven.

#### `Context`

<dfn>Context</dfn> is het verband waarin iets zich voordoet.

Toelichting: <i>Context heeft een brede betekenis. In het CROW-model wordt ‘Juridische context’ gebruikt om het juridische kader (<abbr title="Uniforme Administratieve Voorwaarden">UAV</abbr>/UAV-<abbr title="Uniforme Administratieve Voorwaarden geïntegreerde contracten">GC</abbr>) aan te geven, behorend bij een bepaalde specificatie. De geschiktheid/passendheid van een specificatie is afhankelijk van de samenwerkingsvorm (contractvorm). </i>

#### `Publicatie`

<dfn>Publicatie</dfn> is een selectie uit de CROW data die voor een specifiek doel aan gebruikers aangeboden wordt, online of als hardcopy. Binnen een publicatie kunnen de aangeboden gegevens een structuur krijgen, bijvoorbeeld een hoofdstukindeling.

Toelichting: <i>Voor de CROW Basisspecificaties 2018 geldt, dat de publicatie een selectie is van de data uit De Standaard RAW Bepalingen en de RAW Catalogus Bepalingen.</i>

#### `Document`

<dfn>Document</dfn> is (1) een verzameling gegevens die elk als één geheel wordt vastgelegd en/of gepresenteerd aan de gebruiker. Is (2) een verzameling gegevens van derden, waarnaar verwezen wordt als zijnde de bron van een publicatie

Toelichting: <i>Het concept ‘Document’ wordt tweeledig gebruikt:

1. Om in Publicaties meer dan één structuur te kunnen opnemen, zoals bijvoorbeeld een document met hoofdstukken en paragrafen; en een document dat bestaat uit gegevens. Zoals in de publicatie RAW 2015 drie documenten zitten: de Standaard RAW Bepalingen 2015, de RAW Catalogus Bepalingen 2015 (beide met hoofdstukindelingen) en de RAW Resultaatsbeschrijvingen (de gegevens waarmee het bestek kan worden gemaakt in daartoe bestemde software)
2. Om de bron te vermelden van bijv. een specificatie of een object.
   </i>

#### `Hoofdstuk`

<dfn>Hoofdstuk</dfn> is een deel van een boek of publicatie dat een afgerond geheel vormt.

Toelichting: <i>De CROW Basisspecificaties 2018 op basis van de Standaard RAW Bepalingen en de RAW Catalogus Bepalingen zijn opgedeeld in Hoofdstukken, Deelhoofdstukken, Paragrafen en Artikelen. </i>

#### `Deelhoofdstuk`

<dfn>Deelhoofdstuk</dfn> is een opdeling van een hoofdstuk naar onderdelen.

Toelichting: <i>De CROW Basisspecificaties 2018 op basis van de Standaard RAW Bepalingen en de RAW Catalogus Bepalingen zijn opgedeeld in Hoofdstukken, Deelhoofdstukken, Paragrafen en Artikelen.</i>

#### `Paragraaf`

<dfn>Paragraaf</dfn> is een deel van een tekst dat kleiner is dan een (deel)hoofdstuk en groter dan een artikel.

Toelichting: <i>De CROW Basisspecificaties 2018 op basis van de Standaard RAW Bepalingen en de RAW Catalogus Bepalingen zijn opgedeeld in Hoofdstukken, Deelhoofdstukken, Paragrafen en Artikelen.</i>

#### `Artikel`

<dfn>Artikel</dfn> is een opdeling van een paragraaf naar onderdelen, met tekst waarin een specificatie is opgenomen.

Toelichting: <i>De CROW Basisspecificaties 2018 op basis van de Standaard RAW Bepalingen en de RAW Catalogus Bepalingen zijn opgedeeld in Hoofdstukken, Deelhoofdstukken, Paragrafen, Artikelen (en leden).</i>

## Relaties

Bij het koppelen van specificaties aan concepten wordt gebruikt gemaakt van relaties. In het CROW-model is gedefinieerd welke relaties mogelijk zijn.

Het gebruik van betekenisvolle relaties is uiteraard afhankelijk van de behoefte aan semantiek in de database. Semantiek en complexiteit zal ongetwijfeld worden toegevoegd in de toekomst.

1. Functie-eisen worden gekoppeld aan een functie;
2. Objecteisen en aspecteisen worden gekoppeld aan een object;
3. Raakvlakeisen worden gekoppeld aan een raakvlak;
4. Proceseisen worden gekoppeld aan een activiteit;
5. En eisen die een verificatiemethode hanteren, worden gekoppeld aan die verificatiemethode.

Naast de koppelingen van eisen, zijn er nog koppelingen voor de objectenboom en raakvlakken. Objecten bestaan bijvoorbeeld uit deelobjecten of hebben verschillende varianten. Zo is zichtbaar in een objectenboom of er sprake is van soorten of van samenstellingen.

Hieronder staan de mogelijke relaties die gelegd kunnen worden tussen eisen, objecten, functies, activiteiten, raakvlakken en verificatiemethoden. Met een enkel voorbeeld beperkt tot de relaties die misschien wat toelichting vergen.

### CSPEC Relaties

#### `specificeert`

Iedere eis (specificatie) is gekoppeld aan één of meerdere relevante hoofdconcepten middels de relatie `specificeert`:

- Activiteit
- Functie
- Object
- Raakvlak (raar, is bron van specificatie, niet subject)
  Indien er een verificatiemethode is voor een specificatie, is die specificatie gekoppeld aan die verificatiemethode middels de relatie `heeft verificatiemethode`:
- Verificatiemethode (dit zorgt er voor dat een specificatie niet aan meerdere objecten gekoppeld kan zijn als niet altijd deze verificatiemethode geldt),
  Er kan uiteraard sprake zijn van meer dan één toegestane verificatiemethode.

##### `specificeert` bij Activiteit

Indien een specificatie betrekking heeft op een bepaalde activiteit dan is deze gekoppeld. Hiervoor wordt de relatie `specificeert` gebruikt. De activiteiten zijn werkwoorden; niet de combinatie van werkwoord – zelfstandig naamwoord.
Ook bij gebruikte werkwoorden in RAW is soms ook onduidelijk of een werkwoord nu eenzelfde of een andere betekenis heeft. Als die onduidelijkheid bestaat in ‘te ontrafelen’ inhoud, blijft die onduidelijkheid uiteraard bestaan. Zo kunnen er twee verschillende werkwoorden voorkomen die misschien wel hetzelfde betekenen voor dezelfde onderwerpen of voor verschillende onderwerpen, maar dat is niet altijd helder. Dan blijven die twee werkwoorden (stand heden) naast elkaar bestaan. De semantische discussies die mogelijk zijn over objecten speelt dus ook bij werkwoorden. Iets dat minder belangrijk is voor een contract op een wat hoger aggregatieniveau dan RAW. In RAW gaat het ondanks het streven, nog vaak over het ‘hoe’ en niet het ‘wat’. Betekent meer belang van werkwoorden in het contract.

Een werkwoord als baggeren of maaien heeft nog weinig betekenis. Baggeren van een vaargeul, of maaien van een talud zegt veel meer. Door deze activiteit te koppelen aan de vaargeul, worden er zinnige eisen gesteld. Het maaien van een talud kent andere eisen dan het maaien van een grasveld. Misschien zijn de eisen (specificaties) nog wel gelijk (grashoogte bijvoorbeeld) maar de omstandigheden waaronder de werkzaamheden moeten worden uitgevoerd zijn totaal verschillend bepalen in een groot aantal gevallen de kosten.

In model 1 is in 2016 gebruik gemaakt van de relaties `specificeert activiteit bij object` en `specificeert object bij activiteit`. Denk hierbij aan allerlei eisen die worden gesteld aan objecten afhankelijk van activiteiten als aanbrengen, verwijderen, inspecteren, renoveren etc. Of aan allerlei eisen die worden gesteld aan activiteiten die afhankelijk zijn van object. Naast de koppeling van de eis aan het betreffende object of de betreffende activiteit, geeft deze relatie extra informatie.

<p class="note" title="Groeimodel activiteiten en objecten">
	<i>Deze wijze van modellering blijft in het groeimodel straks waarschijnlijk niet gehandhaafd. Waarschijnlijk gaat CROW over op het structureren van combinaties van activiteiten en objecten.
	</i>
  </p>

<aside class="example" title="specificeert activiteit bij object">
	<p><i>De afwijking in hoogteligging van elementenverharding ten opzichte van het voorgeschreven dwarsprofiel is ten hoogste 10 mm.</i>
	<br>Eis specificeert activiteit met ‘elementenverharding’ en eis wordt gesteld aan (specificeert) ‘aanbrengen’.</p>
</aside>

<aside class="example" title="specificeert activiteit bij object">
	<p><i>Als voegen worden gemaakt door middel van het verkleinen van de doorsnede, de zaagsnede of de scheurinleider op een zodanig tijdstip in de betonverharding aanbrengen dat geen scheurvorming optreedt op plaatsen waar geen voegen zijn voorzien en dat overigens ook geen schade aan het betonoppervlak ontstaat.</i>
	<br>Eis specificeert activiteit met ‘voeg’ en eis specificeert (wordt gesteld aan) ‘aanbrengen’.</p>
</aside>

<aside class="example" title="specificeert activiteit bij object">
	<p><i>De hoogteligging van een rioolput van een vrijvervalriool wijkt ten hoogste 20 mm af van de voorgeschreven hoogteligging. Deze eis geldt bij het (nieuw) aanbrengen van een rioolput.</i>
	<br>De eis wordt gesteld aan het ‘object’ bij het ‘aanbrengen’</p>
</aside>

<aside class="example" title="specificeert activiteit bij object">
	<p><i>Het afschot van een leiding voor een perceelaansluiting ligt tussen 1 : 50 en 1 : 200.</i>
	<br>De eis specificeert het object ‘rioolleiding’. En de eis specificeert ‘rioolleiding’ bij ‘aanbrengen’.</p>
</aside>

<aside class="example" title="specificeert object bij activiteit">
	<p><i>Het gehalte aan zeer fijn materiaal  63 m van brekerzand is volgens de categorie f3.</i>
	<br>Eis specificeert ‘brekerzand’ en eis specificeert ‘object brekerzand’ bij ‘realiseren elementenverharding’.</p>
</aside>

<aside class="example" title="specificeert object bij activiteit">
	<p><i>Het dwarsprofiel van bestrating is gewijzigd tonrond.</i>
	<br>Eis specificeert ‘elementenverharding’ en 	eis specificeert ‘elementenverharding’  bij ‘aanbrengen’.</p>
</aside>

##### `specificeert` bij Raakvlak

Raakvlakeisen zijn eisen die zijn gesteld aan de interactie van het beschouwde systeem met de omgeving, of eisen die worden gesteld aan de interactie tussen objecten binnen het beschouwde systeem (respectievelijk een externe raakvlakeis of een interne raakvlakeis).
Stand heden is er voor gekozen om ‘raakvlakken’ aan te maken voor RAW-bibliotheekdata. Zo kan worden volstaan met het koppelen van de eis aan dit raakvlak (in het voorbeeld van een raakvlakeis tussen twee objecten, kan zo worden volstaan met 1 koppeling i.p.v. een koppeling van de raakvlakeis aan twee objecten).

Naar verwachting is het aantal raakvlakken in RAW beperkt: met accent op raakvlakken tussen objecten. Het betreft generieke (uitvoerings)kennis en geen projectspecifieke kennis (met een projectspecifieke omgeving etc.).

<aside class="example" title="specificeert raakvlak">
	<p>Riolering: eisen aan het overstorten van het riool(systeem) op het oppervlaktewater(systeem)
		<br>Riolering en verharding: eisen die worden gesteld aan het hoogteverschil tussen de bovenkant van putten en kolken t.o.v. de (geprojecteerde) verharding.</p>
</aside>

#### `sluit combinatie uit met`

Indien een specificatie niet gebruikt mag worden in combinatie met een andere specificatie dienen deze specificaties gekoppeld te worden middels de relatie `Sluit combinatie uit met` gebruikt te worden. Deze relatie is bi-directioneel.

#### `vereist combinatie met`

Indien een specificatie een combinatie met een andere specificatie vergt dan dient de relatie `vereist combinatie met` gelegd te worden.

#### `heeft betrekking op`

De volgende fasen worden in de levenscyclus van een object onderscheiden:

- Initiatief
- Ontwerp
- Realisatie
- Gebruik (Gebruiksfase is tevens fase Beheer; onderhoud is onderdeel van Beheer)
- Sloop

Beheer en onderhoud maakt deel uit van de fase Gebruik en is geen andere fase in de levenscyclus.
Overigens wordt op veel vakgebieden onderhoud als een onderdeel c.q. als een aspect van Beheer gezien. Beheer heeft dus een bredere, overkoepelende betekenis en staat dus op een hoger aggregatieniveau. Geadviseerd wordt dit als standaard te adopteren.

De data die CROW beschikbaar stelt betreft generieke data c.q. bibliotheekdata. Het is geen projectspecifieke data. Daardoor is niet altijd expliciet aan te geven in welke fase eisen gelden of kunnen gelden. Bepaalde eisen kunnen immers behoren tot de projectfase realisatie, maar ook tot fase beheer. Deels dus arbitrair. Zaak het in ieder geval consistent te doen. Bibliotheekpecificaties die voor meerdere projectfasen gebruikt kunnen worden moeten dus ‘gelabeld’ worden aan meerdere projectfasen. Denk daarbij met name aan specificaties die betrekking hebben op verificatie: verificaties die niet alleen gebruikt worden bij het realiseren van objecten, maar ook bij het beheer (monitoren) van objecten. Meestal is dat wel duidelijk voor auteurs en reviewers.

Eerder is al in deze ReSpec beschreven welk datamodel is gehanteerd en welke inhoud is opgenomen in dat datamodel. Dat wil niet zeggen dat CROW ook alle inhoud beschikbaar stelt c.q. publiceert. Dat is afhankelijk van besluitvorming intern CROW. En – zo is ook aangegeven - in deze ReSpec is niét beschreven welke eisen CROW stelt aan de modelinhoud van derden. Dat geldt dus ook de class ‘Fase’

#### `vervult`

Ieder onderwerp/hoofdstuk/hoofdobject RAW kent minstens 1 functie. Het object is de functievervuller (en wordt gekoppeld door ‘functie – wordt vervuld door – object’). Er is niet altijd is sprake van een object; denk aan een onderwerp als ‘Baggerwerken’ of ‘Grondwerken’.
Van deelobjecten die je kant en klaar bij de leverancier bestelt worden door CROW geen functies beschreven. Denk bijvoorbeeld aan allerlei deelobjecten waaruit een rioolstelsel wordt opgebouwd.

#### `bestaat uit` & `is variant van`

Objecten filteren uit de inhoud en structureren in een zorgvuldig opgezette objectenboom die deels uit een samenstelling bestaat (deelobjecten van bovenliggend object) en deels uit varianten (een variant van een (deel)object). Middels de relaties `bestaat uit` of `is variant van`.

Hierbij is het belangrijk dat de definities van de deelobjecten helder zijn. Of … op basis van de definities die zijn opgenomen in de inhoud en/of …. op basis van de context. Soms worden verschillende termen gebruikt voor hetzelfde ding; soms wordt eenzelfde term gebruikt voor verschillende dingen helaas. Terminologie in de inhoud van RAW is in de Standaard RAW Bepalingen en de bijbehorende catalogi Bepalingen en Resultaatsbeschrijvingen niet overal consistent, maar is de betekenis in haar context wel helder. Bij het opslaan van data in systemen die worden begrepen door software is consistentie in terminologie uiteraard wel cruciaal.

#### `heeft verificatiemethode`

Bij het project ‘Ontvlechten’ zijn de specifieke verificatiemethoden die binnen de RAW worden gehanteerd gekoppeld aan de betreffende eis. Er is binnen het lopende project géén onderscheid gemaakt in type verificatie.

#### `heeft validatiemethode`

In de modellering is nog geen gebruik gemaakt van het concept ‘Validatie’. De RAW-contractdata zijn immers eisen op een merendeels laag aggregatieniveau. Validatie is aantonen dat het systeem geschikt is voor de toepassing. Verifiëren is aantonen dat het systeem juist is ontworpen en gebouwd.

### CDOC Relaties

#### `heeft juridische context`

Een specificatie wordt toepasbaar verklaard voor de volgende contractvormen:

- UAV en/of
- UAV-GC

Hiervoor moet de relatie `is vast binnen context` of `is facultatief binnen context` worden gebruikt.
In de ontwikkelomgeving is tevens gebruik gemaakt van de relatie `is niet van toepassing binnen context`. Dit is gedaan om het werk van de auteur en reviewers explicieter te maken, waardoor het afbreukrisico in onjuiste relaties afneemt.

#### `is vast binnen context` & `is facultatief binnen context`

Bij specificaties moet aangegeven worden of de betreffende specificatie <i>“Vast”</i> of <i>“Facultatief”</i> is. Het is immers bibliotheekdata. Zo zijn alle specificaties uit de Standaard RAW Bepalingen voor UAV vaste specificaties. Alle specificaties in de RAW Catalogus Bepalingen en de RAW Catalogus Resultaatsbeschrijvingen zijn facultatieve specificaties. Wat de markt van de specificaties in RAW als vast of facultatief beschouwt voor UAV-GC moet zich nog uitkristalliseren. In de startdataset is door CROW een voorzet gegeven. Een deel daarvan is geen discussie en vormt nu ook het hart van de contractdata in de Standaard RAW Bepalingen. Denk aan specificaties op een wat hoger niveau zoals stroefheid of vlakheid van een verharding. Een flink deel is echter arbitrair en opdrachtgeverafhankelijk. Nogal wat UAV-GC contracten worden niet functioneel gespecificeerd of zelfs niet (geheel) objectgericht gespecificeerd. Waar stand heden de scheidslijn ongeveer ligt moet voortschrijdend worden bepaald met de markt. Voortschrijdend, omdat een vraagspecificatie in de toekomst naar verwachting op een steeds hoger niveau komt te liggen.

Aangegeven dient te worden of een specificatie toepasbaar is binnen de juridische context van UAV en/of UAV-GC. In de toekomst kunnen meerdere contexten onderscheiden worden. Voor nu volstaat deze kwalificatie. De volgende opties zijn mogelijk:

- <b>(juridische) context UAV</b>: vast / facultatief / niet van toepassing
- <b>(juridische) context UAV-GC</b>: vast / facultatief / niet van toepassing

De contractdataset UAV-GC wordt gevoed door een deel van de contractdata UAV. Op termijn zal die dataset groeien met contractdata voor UAV-GC. Contractdata op een hoger aggregatieniveau passend bij de samenwerkingsvorm UAV-GC. Stand heden ontbreekt die contractdata in de CROW-bibliotheekdata.



## Specificatiecategorie

Met behulp van de relatie `is van categorie` is voor elke specificatie aangegeven onder welke specificatiecategorie deze valt.
In lijn met de methodiek ‘functioneel specificeren’ en ‘Systems Engineering’ wordt hierbij onderscheid gemaakt in de volgende specificatiecategorieën:

- Functie-eis
- Aspecteis
- Objecteis (of gekozen eigenschap: een objecteis zijnde geen aspecteis)
- Raakvlakeis
- Proceseis

De contractdata betreft bibliotheekdata met content RAW. Dat is veel standaard uitvoeringskennis met selectiemogelijkheden in productcatalogi (resultaatsbeschrijvingen) met activiteiten en objecten Specifieke object gerelateerde kwaliteiten, zoals de maatvoering en materialisering noemen we objecteigenschappen.
<i>Zie publicatie 289 [Handboek specificeren](https://www.crow.nl/publicaties/handboek-specificeren) en [CROW-Model Vraagspecificatie van maart 2016](https://www.crow.nl/blog/mei-2016/nieuw-model-vraagspecificatie-best-for-project-g).</i>

### Aspecteis subcategorieën

In deze paragraaf wordt ingegaan op verschillende typen aspecteisen die kunnen worden onderscheiden en wat CROW daar nu mee heeft gedaan.
Een aspecteis kan aan meer dan één aspect zwak of sterk bijdragen. Gebleken is dat auteurs en reviewers CROW heeft als afspraak gehanteerd: maximaal één aspecteistype te selecteren, tenzij onvoldoende consensus. Dus in geval consensus over het maatgevende aspect is dat aangegeven. Bij teveel onduidelijkheid of verschil is geen subcategorie aangegeven.
De meerwaarde van één subcategorie aspecteis (bij voldoende consensus) wordt stand heden hoger ingeschat dan een lijstje met veel arbitraire subcategorieën. Realiserend dat dit betekent dat de vindbaarheid zich beperkt tot aspecteisen waar een subcategorie is aangegeven én zich beperkt tot die subcategorie. Allerlei eisen met mogelijke aanvullende (meerdere) subcategorieën met meer of minder zwakke relaties worden dus niet gevonden.
Te hanteren lijst subcategorieën voor Aspecteis:

- Betrouwbaarheid
- Beschikbaarheid
- Onderhoudbaarheid
- Veiligheid
- Gezondheid
- Milieu
- Beveiliging
- Beeldkwaliteit

<i>Uitgangspunten:</i>

De content van RAW kent groot scala aan eisen op laag aggregatieniveau in de eisenpiramide. Tevens een breed scala aan technische eisen en (keuzes in) eigenschappen van deelobjecten.
Waar sprake is van een aspecteis geldt ‘zo concreet mogelijk, zo abstract als nodig’. Dit betekent volstaan met label ‘aspecteis’ als geen nadere concretisering mogelijk is c.q. er teveel verschil in inzicht en keuze blijkt te zijn in subtype door betrokken auteurs en reviewers.
Indien naar oordeel van de auteur een eis duidelijk een bepaald aspect dient, dan wordt dat aspect aangevinkt. Er kan dus maar één aspecttype worden aangevinkt. De verwachting is dat zodra er aan meerdere aspecten wordt bijgedragen naar oordeel auteur, de resultaten van verschillende auteurs teveel van elkaar zullen afwijken.

Zie [CROW-Model Vraagspecificatie van maart 2016](https://www.crow.nl/blog/mei-2016/nieuw-model-vraagspecificatie-best-for-project-g)

<p class="note" title="Beeldkwaliteit i.p.v. Vormgeving">
	<i>In afwijking van de Model Vraagspecificatie is ‘Beeldkwaliteit’ gehanteerd i.p.v. ‘Vormgeving’. Beeldkwaliteit omvat zowel vorm als materialisering. Beeldkwaliteit is tevens een veelvoorkomend begrip in contractdata voor beheer. En…. voorkomt onnodige selectieproblemen bij twijfel tussen ‘vorm’ en ‘materialisering’. Tevens zijn niet alle RAMSHEEP-aspecten gebruikt omdat het geen projectspecifieke data is maar bibliotheekdata. Politiek bijvoorbeeld is in bibliotheekdata geen issue.
	</i>
  </p>

### Proceseis subcategorieën

In de markt is er nog steeds onduidelijkheid in terminologie en afbakening van ‘Proceseis’. Niet iedereen verstaat hetzelfde onder een proceseis. Dit betekent ook dat dit type eisen op hele verschillende plaatsen in het contract voorkomen. Dat levert extra werk en afbreukrisico op in het proces van opstellen en aanbesteden van contracten.
In het CROW-model hebben we iedere eis getypeerd; dus ook eisen van de categorie ‘proces’.

<i>Toelichting</i>:

Proceseisen wordt door partijen verschillend gedefinieerd. Zie SE-wijzer BAM; zie CROW-P289; zie Provincie, Rijk etc.. Naast “eisen aan activiteiten die nodig zijn om het systeem tot stand te brengen”, zijn er ook partijen die allerlei ‘dataverkeer’ (documentenverkeer) ook als proceseis zien. De scheiding in administratieve eisen en proceseisen blijkt best lastig. Proceseisen zijn eisen gesteld aan de wijze waarop het werk tot stand gebracht moet worden. En niet zoals functie-, aspect- en objecteisen aan het te realiseren systeem.

Wat betreft duidelijkheid in het onderscheid tussen een ‘proceseis’ en overige eistypen is de rapportage van de [CROW-Model Vraagspecificatie van maart 2016](https://www.crow.nl/blog/mei-2016/nieuw-model-vraagspecificatie-best-for-project-g) het meest transparant tot heden. Niét door de vijf functierollen van IPM; en niét door het gebruik van de vier onderscheiden processen: technisch management, projectmanagement, projectbeheersing en omgevingsmanagement. Maar wél door de (soms arbitraire) keuzes die gemaakt zijn in de daarbij horende werkpakketten. Houvast daarbij is de plaats van een werkpakket in die structuur (de structurering volgens de Model Vraagspecificatie van maart 2016). Het overzicht van de vier processen en de bijbehorende werkpakketten is hieronder opgenomen.

| 1. Technisch Management     | 2. Projectmanagement                          | 3. Projectbeheersing       | 4. Omgevingsmanagement           |
| --------------------------- | --------------------------------------------- | -------------------------- | -------------------------------- |
| TM - Ontwerpen              | PM - Interactie opdrachtgever - opdrachtnemer | PB - Scopemanagement       | OM - Communicatie                |
| TM - Uitvoeren              | PM - V&G management                           | PB - Kwaliteitsmanagement  | OM - Verkeersmanagement          |
| TM - Onderhouden            | PM – Inkoopmanagement                         | PB - Planningsmanagement   | OM - Vergunningen                |
| TM - Verifiëren & Valideren |                                               | PB - Financieel management | OM - Kabels en leidingen         |
| TM – Opleveren              |                                               | PB - Risicomanagement      | OM - Archeologie                 |
|                             |                                               | PB - Documentmanagement    | OM - Flora en fauna              |
|                             |                                               | PB – Informatiemanagement  | OM - Niet gesprongen explosieven |
