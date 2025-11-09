# projektarbete
Responsiv webbplats (HTML &amp; CSS)

Kort projektbeskrivning: Hemsida för en bostadsrättsförening i Växjö. Första sidan är en välkomst/landningssida med stor hero. På större skärmar dvs desktop växlar bakgrundsbilden för en mer levande känsla. På heron finns huvudrubrik och en knapp som tar användaren direkt till huvudinnehållet. Det finns också en animerad hamburgermeny där man väljer sida. 
Under hero-bilden finns de senaste nyheterna till föreningens medlemmar. 

Huvudinnehållet finns på "about.html"/Om oss. Består av bild, tabeller och text om föreningen. Layouten blir olika beroende på skärmstorlek. 

Den tredje sidan innehåller formulär och länkar. På större skärmar finns bilder med hover-effekt för att göra sidan roligare.
Det finns ett formulär att fylla i direkt på hemsidan (som mejlas till styrelsen då jag ännu inte kan ta hand om svaren i fil/på server). Övriga formulär är i form av länkar där formulären är skapade i Airtable. Det blir en fördröjning innan formulären öppnas i det nya fönstret första gången beroende på att annan tjänst anropas. 

På alla tre sidor finns samma footer med direktlänk för att mejla till föreningen, föreningens organisationsnummer samt länk till karta i Google maps om man klickar på hussymbolen. 

Den animerade menyn är också gemensam för alla tre sidor. 

Har använt en blå bakgrundsgradient och texten i vitt eller svart beroende på vad som ger bäst kontrast. 
Typsnitt och färger kan enkelt ändras genom variablerna i menustyles.css och styles.scss. 

Blandar block och flexbox samt har två gridsystem beroende på skärmstorlek och innehållet på sidan. Flex har använts för att enkelt kunna centrera innehållet. Grid för att kunna anpassa layouten efter skärmstorlek på ett smidigt sätt. 

CSS-mönster: Styling av hamburgermeny (samtliga sidor) och header (about och contact-sidorna) är skriven i css-fil med variabler.
Övrig css är skapad genom SCSS. 
SCSS-filens upplägg:
variabler
mixins
keyframes
body
css-styles för index.html
css-styles för gemensamma element (footer)
css-styles för about.html
css-styles för contact-html
media-queries för skärmar 700px och större (iPads och liknande)
media-queries för skärmar 1250px och större (desktop)
media-queries för reduced motion-preferens

Kända begränsningar/förbättringsidéer: 
Tabellerna syns bara när användaren vill läsa dem (klicka för att se hela tabellen)
Formuläret öppnas i mejlprogram och måste skickas iväg av användaren.
Menyn på about och contact ha input:checked som default vid skärm på minst 1250px så den syns från början och aktivt stängs ner istället. 
Ev mindre textstorlek i mobilversionen men samtidigt är det viktigt med god läsbarhet. 
Nyhetskorten på index.html hade kunnat anpassa så endast ett kort visades i taget i mobil-läge. 
Ej anpassat layouten efter orientation på device (porträtt eller landskapsläge).
Inte testat så det fungerar som tänkt i alla webbläsare (har testat i Chrome och Safari).

