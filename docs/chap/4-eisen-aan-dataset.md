# Eisen aan de dataset

In deze sectie worden de minimale eisen beschreven waaraan een dataset moet voldoen.

## Eisen aan de inhoud

De <a>Producent</a> van de data is verantwoordelijk voor de juistheid van de data (kwaliteit, volledigheid, betrouwbaarheid).
CROW stelt op dit moment enkel eisen aan de semantiek en structuur. Deze worden beschreven in de volgende secties. 

## Eisen aan het model 
<b>Eis 1:</b> Door CROW gepubliceerde model, <a>CSPEC</a>, dient als basis te worden gebruikt voor het definiëren van classes en relaties. Indien in de dataset classes en/of relaties voorkomen die afwijken, dan wordt de dataset niet meegenomen ter publicatie.

Het door CROW gepubliceerde model, <a>CDOC</a>, is optioneel om te gebruiken.

Voorbeeld:
In <a>CSPEC</a> en <a>CDOC</a> staan restricties m.b.t. de domain en range van de relaties die nauwkeurig gevold moet worden.
<p class="note" title="Domain, Ranges en restricties">
	<i>Domain is wat er links staat van de relatie. En rechts staat de range van de relatie. De restrictie is de regel die geldt voor deze. De domain en ranges met daarbij behorende restrictie zijn terug te vinden in het CROW datamodel</i>
  </p>	

De relaties en klassen in <a>CSPEC</a> en <a>CDOC</a> zijn beschreven in het volgende document: 
<p class="ednote" title="This section will be reformatted">
	“Toelichting bij classes en relaties in CROW-datamodellen <a>CSPEC</a> en <a>CDOC</a> v1.0, dd 08-05-2018” (de actuele versie van dit document is op te vragen bij CROW).
  </p>
  

In onderstaande figuur is het class diagram van <a>CSPEC</a> weergegeven. Dit class diagram beschrijft welke entiteiten bekend zijn in de CROW-datamodellen en beschikbaar voor instantiering. De betekenis van de data is beschreven d.m.v  de relaties tussen de entiteiten.

In het class diagram ligt tevens vast welke entiteiten en relaties <span style="color:red">verplicht</span>. zijn, welke <span style="color:yellow">optioneel</span>. zijn en welke niet verplicht zijn. De optionele klassen of relaties houden in dat er in ieder geval 1 of meer entiteiten <b>moeten</b> aangeleverd zijn. 


<b>Eis 2:</b>  De volgende modelleer constructies dienen minimaal in de dataset aanwezig te zijn:
* Alle specificaties c.q. eisen dienen geclassificeerd te zijn als `cspec:Specificatie`
* Elke instantie van `cspec:Specificatie` dient d.m.v. de relatie `cspec:specificeert` gekoppeld te zijn aan minimaal &#233;&#233;n van de volgende concepten:
 * `cspec:Object`
 * `cspec:Activiteit`
 * `cspec:Functie`
 * `cspec:Raakvlak`

<img src="Aanleverspecs_specificatieschema.png" alt="Specificatieschema" style="width:764px;height:538px;">

## Eisen aan de vorm

De dataset moet als separaat Turtle-bestand (.ttl) worden aangeleverd bij CROW (zie de sectie [Wijze van aanlevering](#3))

Het Turtle-bestand dient in lijn te zijn met de W3C Recommendation RDF 1.1 Turtle, gepubliceerd op  <a href="http://www.w3.org/TR/turtle/">www.w3.org/TR/turtle</a>.

## Voorbeeld

Een voorbeeld dataset is te vinden op de GitHub omgeving: 

[VoorbeeldDataset.ttl](https://github.com/Stichting-CROW/Contracteisen/blob/master/voorbeeldDataset.ttl)

<aside class="example" title="Snipped uit voorbeeldDataset.ttl">
<pre id="voorbeeldDataset snipped">
	<code   class="turtle"
			data-include-format="text"
			data-include="voorbeeldDataset snipped.ttl"></code>
  </pre>
</aside>

## Toetsen met SHACL

Zodra de aangeleverde files binnenkomen worden deze getoetst. De belangrijkste toets is een validatie met een [SHACL](https://www.w3.org/TR/shacl) shapes bestanden.

Om van te voren de aangeleverde datasets te toetsen is het SHACL.shapes bestand beschikbaar gesteld:
[CSPEC model -voor individuele sets- SHACL.shapes.ttl](https://github.com/Stichting-CROW/Contracteisen/blob/master/CSPEC%20model%20-voor%20individuele%20sets-%20SHACL.shapes.ttl)
