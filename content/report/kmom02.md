---
Title: Redovisning i Kmom02
Description: Delredovisning i Kmom02 för kursen PA1436.
---

# Kmom02

## Vad tycker du om SASS än så länge?

Utan SASS vore livet som webbutvecklare i dag ganska jobbig med repetitiv stilkod som skulle ge huvudvärk så fort man behöver ändra på något. Med SASS:s DRY (_don't repeat yourself_) i åtanke och med dess utökade funktioner som saknas i traditionell CSS minimeras den mängden kod drastiskt. Sen finns det två olika SASS-syntaxer: SASS och SCSS; den sistnämnda har även sina fördelar när man är i en övergång från CSS till SCSS då den stödjer CSS rakt av, medan SASS kräver att man formaterar om koden.

## Är du bekant med Node, npm eller npm scripts (t.ex. `npm run lint`) sedan tidigare? Vad anser du om det?

Eftersom jag är Linux-användare så är det svårt att inte vara bekant med det, i synnerlighet NPM, där återfinns massa trevliga bibliotek och appar som kan hämtas ner via NPM eller Yarn som förgyller Linux-vardagen.

Node.js har jag primärt kommit i kontakt med i samband när jag höll på med React, Vue.js eller gjort snabba JS-appar med Express.js.

Vad jag anser om att lägga in scripts? Ja, men det är väl inge fel med det, tänker jag? Det kan underlätta att lägga in aliaskommandon som körs frekvent som kan vara jobbiga att skriva ut manuellt varje gång. Tycker dock att Makefile är lite bättre, om man ska göra lite mer saker än att förkorta ett kommando, t.ex. om man ska köra deploy där man behöver kompilera, rensa ut grjer, köra scp och dylikt. Dock är det förvisso inget som hindrar än från att lägga in aliaskomandon som refererar till Makefile.

## Hur kändes det att kompilera SASS till CSS, var det något du reflekterade över?

Lite jobbigt att manuellt kompilera varje gång man gör en ändring i SCSS. Nu fuskade jag och körde auto-watch på filerna, men la inte in det i package.json eftersom det inte ingick i inlämningsuppgiften. Men annars hade jag inte någon direkt reflektion kring kompileringen.

## Kommentera ditt tema, hur kan man beskriva dess design och hade du några planer på “design” när du byggde ditt tema?

Nej, jag hade ingen plan alls där. Mitt temat bygger på den ursprungliga default Pico-temat där färgerna är väl det som skiljer dem åt. Gillar inte att temat går från desktop och skalas ner till mobile-view. Tycker det känns mer naturligt att ha en mobilanpassad sida som man sen modifierar utefter bredden än att göra det tvärtom.
Vidare följer det med JS-bibliotek för saker som kan hanteras via CSS vilket känns lite obsolet. Då frsöker jag se mellan fingrarna med de CSS-fixar för IE8 och IE9 jag hittade i CSS-filen. Själva temat är spartanskt upplagd bestående av en index.twig-fil, så funderar på att göra om temat så att det verkligen blir mitt enga tema. Kanske hinner jag pilla lite på det till nästa inlämning.

## Valde du att dela upp din kod? Vilka uppdelningar valde du att göra?

Jag valde dela upp SCSS i moduler och försöka kategorisera dem efter dess huvudområde. Sen använder jag mig av `variables` modulen för konstanter.

## Vilken är din TIL för detta kmom?

Förvånad att `max-nesting-depth` för SCSS är satt till 1 per default.
