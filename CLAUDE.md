# Regler för det här repot (för AI och andra som lägger till prov)

Repot innehåller övningssidor inför prov för en elev i årskurs 4. Varje prov är en egen mapp med en `index.html`. Startsidan `index.html` i roten listar proven. Sidorna ska fungera på GitHub Pages (https://neckfors.github.io/prov/), alltså som statiska filer utan bygge.

## Regler för innehållet

1. **Hänvisa till källan på varje svar.** Skriv sidnummer i parentes efter varje påstående, till exempel `(s. 76)`. Hänvisa till bok och/eller häfte, så att en vuxen kan dubbelkolla. Skriv vilken bok eller vilket häfte det gäller, antingen i sidhuvudet eller i hänvisningen om det finns flera källor.
2. **Hitta inget i boken eller häftet?**
   - Läs först igenom alla sidor en gång till innan du bestämmer att svaret saknas.
   - Saknas svaret fortfarande, skriv ett eget svar, men markera tydligt att det **inte kommer från bok eller häfte**. På sidorna används en blå ruta med texten "Från nätet, inte från boken eller häftet:" följt av svaret och en rad "Källor:" med webbplatserna.
   - Skriv aldrig ett eget svar utan markering, och blanda inte in egna svar i text som hänvisar till boken.
   - Om du inte hittar något alls, skriv det och be eleven eller läraren komplettera. Gissa inte.
3. **Bara det boken eller häftet säger.** Svaren ska bygga på de sidor eleven har fått. Ta inte med fakta från minnet som om de stod i boken. Kontrollera årtal, namn och siffror mot sidan.
4. **Nivå: årskurs 4.** Korta meningar, vanliga ord, inga svåra termer utan förklaring.
5. **Frågorna ska vara de exakta frågorna från läraren.** Ta frågorna ur provets checklista eller övningsblad och behåll formuleringen så eleven känner igen dem. Slå ihop frågor som finns på flera listor så att varje fråga bara står en gång.
6. **Dela upp frågor med underfrågor.** Varje underfråga blir en egen fråga med svaret direkt under. Gruppera frågorna efter ämne med rubriker.
7. **Begrepp** från lärarens begreppslista tas med som klickbara kort med sidhänvisning.
8. **Ingen märkning av vilken lista en fråga kommer från** (som H eller P). Sidhänvisningarna räcker.

## Så ser en provsida ut

- Använd `vikingatiden/index.html` som mall. Kopiera mappen, byt innehållet i `DATA` och `TERMS` i skriptet och byt rubrik och titel.
- Sidan visar bara frågorna. Man klickar på en fråga (`<details>`) för att se svaret. Det finns knappar för att visa eller dölja alla svar och för att blanda frågornas ordning.
- Hjälpfunktioner i skriptet: `P("s. 76")` ger en sidhänvisning, `WEB(text, källor)` ger den blå rutan för svar från nätet.
- Sidan ska fungera utan internet, ha en tydlig stil och även gå att skriva ut. Använd inga externa bibliotek.
- Texten är på svenska.

## Lägga till ett nytt prov

1. Skapa en mapp, till exempel `geografi/`, med en `index.html`.
2. Lägg ett kort för provet i `index.html` i roten och en rad i `README.md`.
3. Kontrollera att skriptet i sidan kör utan fel innan du pushar.

## Övrigt

- GitHub Pages måste slås på i Settings → Pages (Deploy from a branch, `main`, `/ (root)`). Det går inte att göra via API från Claude-sessioner.
- Ägaren använder bara HTML-sidorna här. Gör inga Google-dokument om ägaren inte ber om det.
