# Inleiding

Deze ReSpec bevat de aanleverspecificaties en de gehanteerde datamodellen voor het Dataplatform van CROW. 
Het maakt deel uit van de complete set aan documentatie die CROW beschikbaar heeft omtrent het CROW Linked Data Platform (verder: (<abbr title="LinkedData Platform"><a>LDP</a></abbr>). Al deze documentatie en bijbehorende bestanden zijn te vinden op de CROW Contracteisen GitHub omgeving: [https://github.com/Stichting-CROW/Contracteisen](https://github.com/Stichting-CROW/Contracteisen)
	
<a>Aanleverspecificaties</a> zijn voorwaarden waaraan een data(set) van een producent moet voldoen waaronder CROW de data(set) kan accepteren voor opname in het dataplatform.

<a>Datamodel</a> beschrijft hoe de gegevens in het LDP gestructureerd zijn. 
		
Binnen het publicatieproces wordt er onderscheid gemaakt tussen drie rollen:
1. <a>Producent</a>
2. <a>Publicist</a>
3. <a>Consument</a>

Elke rol heeft zijn eigen taken/verantwoordelijkheden. In de volgende sectie worden deze nader toegelicht.

## Het Publicatieproces

Op hoofdlijnen onderscheiden we 4 stappen in het publicatieproces:


<img src="Aanleverspecs_ProducentPublicistConsument.png" alt="Publicatieproces" style="width:595px;height:290px;" />

1. De <a>producent</a> levert een dataset aan bij de <a>publicist</a>.
2. De <a>publicist</a> publiceert de dataset in het het <a>LDP</a>.
3. De <a>publicist</a> zorgt ervoor dat de dataset beschikbaar is in het CROW Kennisbank en/of voor de relevante webservice(s)/endpoint(s).
4. De <a>consument</a> kan een eindgebruiker zijn of een software systeem die data uit het dataplatform haalt voor eigen gebruik. Dit kan bijvoorbeeld door het ophalen van data met zijn/haar software door middel van een webservice.

In de sectie [Eisen aan de dataset](#4) worden de eisen die CROW stelt aan de kwaliteit van aan te leveren datasets bij CROW <i>(=Stap 1)</i> uiteengezet. Informatie over andere stappen of onderdelen van het publicatieproces is opgenomen in andere delen van de documentatie. Hiervoor kunt u contact opnemen met CROW. Na publicatie van een dataset wordt door CROW de URI van de dataset gedeeld met de <a>Producent</a>.
