---
Title: Laddningstider & användbarhet
Description: Laddningstider & användbarhet
Template: report
---

Kmom05 - Laddningstider & användbarhet
==========================

Metod & urval
----------

Jag valde att använda samma 3 sidor som i Kmom04, alltså Fotografiska, Naturhistoriska Riksmuseet och Nordiska museet. Jag tyckte att det var intressant att göra en analys på dessa sidor som uppenbarligen utvecklats av professionella webbbyråer och se om jag trots detta kunde hitta förbättringsmöjligheter. Verktygen jag använde var Google PageSpeed samt DevTools i Google Chrome.

Webbsidor för analys
-----------

### Fotografiska
![alt text][fotografiska1]
[fotografiska1]: ../assets/img/kmom04/Fotografiska1.png "Fotografiska, startsida"

Jag valde att analysera de tre sidor som jag tycker känns viktigast för besökarna, nämligen [startsidan](https://stockholm.fotografiska.com/sv/), [besökssidan](https://stockholm.fotografiska.com/sv/besok) samt [programsidan](https://stockholm.fotografiska.com/sv/pa-gang). Samtliga sidor är hyfsat långsamma att ladda, ofta över 1,5 sekunder, vilket inte nådde upp till mitt mål om 1 sekunds laddningstid. Tillgänglighetsmässigt fick sidan dock bra betyg på PageSpeed med 100 poäng för alla sidor både på mobil och desktop. Sidan presterade sämst på bästa praxis (best practices), vilket främst verkar ha med hur man hanterar kakor att göra. Sidan fick även ganska låga betyg på prestanda på mobil (76 poäng), vilket inte förvånar mig så mycket eftersom man har valt att använda sig av en film i headern, vilket verkar vara det som drar ner betyget mest. Andra saker som påverkar betyget negativt på PageSpeed är stora bildstorlekar, oanvänd JavaScript-kod samt tiden det tar för själva rotdokumentet att ladda. I DevTools kunde jag också så att man laddade in resurser för exempelvis betalning vilket också adderade till den långa laddningstid, vilket jag tycker att man hade kunnat vänta med att ladda in tills besökaren gick in på biljettsidan där den resursen behövs.


### Naturhistoriska Riksmuseet
![alt text][naturhistoriska1]
[naturhistoriska1]: ../assets/img/kmom04/Naturhistoriska1.png "Naturhistoriska, startsida"

Precis som med de andra sidorna så valde jag att analysera [startsidan](https://www.nrm.se/) och [besökssidan](https://www.nrm.se/besok-museet), samt [utbudssidan](https://www.nrm.se/vart-utbud). Samtliga sidor tog under en sekund att ladda, vilket uppfyllde mitt krav på max 1 sekunds laddningstid. Tillgänglighetsnivån var på topp genom alla sidor på både mobil och desktop, även SEO och bäst praxis fick höga poäng. Den enda kategorin där det inte gick lika bra var på prestandan som på mobil ibland var nere på 66 poäng. Den främsta anledningen till detta var onödigt stora bildstorlekar och omoderna bildformat, men även onödig JavaScript och CSS-kod.


### Nordiska Museet
![alt text][nordiska1]
[nordiska1]: ../assets/img/kmom04/Nordiska1.png "Nordiska Museet, startsida"

Precis som med Fotografiska så valde jag att analysera [startsidan](https://www.nordiskamuseet.se/) och [besökssidan](https://www.nordiskamuseet.se/besok-oss/), samt [utställningssidan](https://www.nordiskamuseet.se/utstallningar/). Samtliga sidor tog även här under en sekund att ladda, även om den ofta var uppe och nosade på min ensekundsgräns. Tillgängligheten fick fulla poäng rakt igenom även på denna sida, vilket gjorde mig glad! Även SEO fick full pott överallt, till skillnad från de andra två sidorna. Bästa praxis fick också genomgående väldigt bra poäng. På desktop fick samtliga sidor nästan fulla poäng på prestandan, men på mobil var den på startsidan nere på 55 poäng vilket var väldigt lågt. Ett stort problem verkar vara hur man hanterar fönstret för att godkänna cookies, på desktop finns inte samma problem av någon anledning. PageSpeed anger också storleken på DOM:en som ett problem, vilket verkar ha med antal noder på DOM-trädet att göra (exempelvis om man har för många generella query selectors i JavaScript). Precis som med de andra sidorna så fick Nordiska Museet också nedslag på oanvänd JavaScript och CSS-kod.

Analys - sammanfattning
---------
Jag tyckte egentligen att alla sidor laddade snabbt, även Fotografiska som tog längre tid på sig än de övriga två. Dessa sidor är ju som sagt säkerligen skapade av professionella webbyråer och bör därför inte ha problem med långa laddningstider. Att man har valt att använda sig av en film på Fotografiskas webbsida är nog en avvägning man har gjort med medvetenhet kring laddningstider. Alla sidor fick liknande resultat på SEO, tillgänglighet och bästa praxis, så i min rangordning har jag därför valt att främst gå på prestanda och laddningstider.

### Rangordning
1. Naturhistoriska Riksmuseet - Bästa laddningstid och hyfsat bra prestanda, trots ett rätt stort antal resurser. 

2. Nordiska Museet - Bra laddningstider och hyfsat bra prestanda.

3. Fotografiska - Hyfsat bra prestanda men långa laddningstider.


### Förbättringsmöjligheter
Jag tyckte att det var lite roligt att se att PageSpeed rekommenderade en rensning i både JavaScript och CSS för samtliga sidor. Jag vet själv hur svårt det kan vara att rensa i CSS-kod när sidan börjar bli stor, så kanske har även professionella utvecklare på stora byråar samma problem, eller så ligger det något annat bakom som inte PageSpeed kan redogöra för. Den enda sidan som inte hade problem med stora bildstorlekar och annat som hade med media att göra var Nordiska Museet, vilka istället hade andra problem som drog ner prestandan rejält.


### Mätvärden
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTGVXjX7_6gcMt5g6aPvRc3MRjTyhCwPBx50zvLmrLXnjlp7Hy__C7cxdMHK7qs1NvW1l89Dub4UHZF/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" class="spreadsheet"></iframe>

Denna analys och rapport har utförts som ett individuellt arbete av Keshti Gyllinger.
