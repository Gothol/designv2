Utvärdering av laddningstider på webplatser
=======================

Det här är en utvärdering av laddningstider på tre stycken webplatser. Syftet är att utvärdera tiden det tar ladda olika sidor på platserna och vilka förbättringsåtgärder som platserna kan göra.

Urval
-----------------------

Jag har valt att utvärdera e-butiker för kläder där du kan beställa måttsydda och egendesignade skjortor. De här är sidor som alla är bild och script-tunga, i och med att du redan på sidan skall kunna välja olika tyger och design för din skjorta och efter varje val se hur skjortan ska kunna se ut. Det är alltså sidor där hänsyn till laddningstider borde en mycket viktig del av siddesignen. De webplatser jag valt är itailor.com, tailorstore.se och skjortfabriken.com. Urvalet gjordes genom att göra en googlesökning på "designa egen skjorta herr" och sedan välja de tre första platserna där jag kunde beställa en skjorta som var både måttsydd och egendesignad. itailor.com, tailorstore.se hamnade överst då de betalat för annonsplatser.

Metod
-----------------------

För varje plats valde jag tre sidor att mäta hastigheten på, jag mätte hastigehten dels med Google pagespeed insights https://developers.google.com/speed/pagespeed/insights/ och dels med dev tools network i chrome. Med pagespeed gjorde jag en mätning för mobiler och för datorer på varje sida. Med dev tools mätte jag tre gåner på varje sida och använde mig sedan av medelvärdet från dessa mätningar. Varje mätning utfördes genom en omladdning av sidan med komandot shift+ctrl+r med disable cache aktiverat i dev tools. Resultaten sparades i ett excellark på google documents.

Resultat
-----------------------

Insamlad mätdata finn i detta dokument: https://docs.google.com/spreadsheets/d/1PlYc7xUm5i_sAMts6npojun0wtriuhsfxtwHKBBMqBg/edit?usp=sharing. I sammanfattningen så ser ni det som visas på pagespeed samt längst ner i varje mobilkolumn finns också värden från dev tools. I fliken för respektive plats finns detaljer från pagespeed och samliga tre mätningar från dev tools för varje sida.


iTailor
Jag mätte på första sidan https://www.itailor.com/, sidan för skjortdesign https://www.itailor.com/designshirts/ och "Om oss" sidan https://www.itailor.com/about-us.php.
Itailor hade för mobilerna ett riktigt dåligt resultat på första sidan och på sidan för skjortdesign (26 i betyg på pagespeed på båda sidorna) och ett bättre men fortfarande dåligt resultat på Om-sidan (77). För datorer var betyget högre men fortfarande dåligt på alla sidor utom om-sidan, 70 för startsidan, 56 för design-sidan och 91 för om-sidan.
Samtliga mätningar på pagespeed föreslog förbättringen "Minska svarstiderna från servern (tid till första byte)", förbättringen "Skicka bilderna i modernare bildformat" förekom på alla sidor utom om-sidan.

Dev Tools ger att första sidan är 13 mb stor, har 155 resurser som laddas och blir färdigladdad på 1,1 minuter. Designsidan är 4,9 mb stor, har 144 resurser som laddas och blir färdigladdad på 13,72 sekunder.
Om-sidan är 1,3 mb stor, har 37 resurser som laddas och blir färdigladdad på 4,57 sekunder.

Printscreens:

[FIGURE src="image/rapport05/itailor01.png?w=400" class="rapport" caption="iTailor print 1"]

Tailorstore
Jag mätte på första sidan https://www.tailorstore.se/, sidan för skjortdesign https://www.tailorstore.se/skjortdesignern och "Brand-story" sidan https://www.tailorstore.se/brand-story-1 hade egentligen velat mäta på en "Om oss sida" men tailor store hade delat upp om oss på flera olika sidor och då valde jag jag brandstory med förhoppningen att den bäst skall motsvara om oss på övriga sidor.

Tailorstore hade för mobilerna dåliga pagespeed-betyg på samtliga sidor, 57 för startsidan, 62 för designsidan och 68 för brand-story. Däremot hade de riktigt bra resultat för datorer, 95 för startsidan och 99 för både designsidan och brand-story. I samtliga mätningar utom brand-story för datorer så föreslogs förbättringen "Ta bort resurser som blockerar renderingen" och i fyra av mätningarna föreslogs förbättringen "Ta bort oanvänd CSS". I mätningen brand-story för datorer föreslogs ingen förbättring.

Dev Tools ger att första sidan är 3,4 mb stor, har 84 resurser som laddas och blir färdigladdad på 10,9 sekunder. Designsidan är 3,5 mb stor, har 98 resurser som laddas och blir färdigladdad på 13,9 sekunder.
Om-sidan är 2,5 mb stor, har 54 resurser som laddas och blir färdigladdad på 7,74 sekunder.

Printscreens:
[FIGURE src="image/rapport05/tailorstore01.png?w=400" class="rapport" caption="Tailorstore print 1"]

Skjortfabriken
Jag mätte på första sidan http://skjortfabriken.com/, sidan för skjortdesign http://skjortfabriken.com/ShirtDesigner och "om skjortfabriken" sidan http://skjortfabriken.com/t-ns_aboutnordicshirts.aspx

Skjortfabriken har dåliga betyg på pagespeed för samtliga sidor, 64 för startsidan, 40 för designsidan och 68 för om-sidan. För datorer var betygen bättre, dock fortfarande dåligt för designsidan som fick 66, startsidan och om-sidan fick helt ok betyg, 91 respektive 89. i samtliga mätningar föreslogs förbättringen "Ta bort resurser som blockerar renderingen" och i all mätningar utom på om-sidan för datorer föreslogs förbättringen "Minska svarstiderna från servern (tid till första byte)".

Dev Tools ger att första sidan är 2,6 mb stor, har 71 resurser som laddas och blir färdigladdad på 10,51 sekunder. Designsidan är 2,3 mb stor, har 151 resurser som laddas och blir färdigladdad på 10,71 sekunder.
Om-sidan är 1,7 mb stor, har 59 resurser som laddas och blir färdigladdad på 4,12 sekunder.

Printscreens:
[FIGURE src="image/rapport05/skjortfabriken01.png?w=400" class="rapport" caption="Skjortfarbriken print 1"]

Analys
-----------------------

Det var förvånsvärt stor skilland mellan sidorna, jag hade förväntat mig dåliga resultat för mobiler men inte riktigt så dåliga resultat för datorer och skillnaderna i laddningstid för stratsidorna är väldigt stora speciellt mellan itailor och de andra två, till itailors försvar skall dock sägas att deras förstasida innehåller ett rullande bildspel där varje bild stannar i ett par sekunder villet gör att dte tar tid tills hela spelt har kört igenom och dev tools anser att sidan är färdigladdad. itailor verkar till viss del vara medvetna om problemet då de använder sig av en en för sida som visar hur stor del av sidan som är laddad och vid 100% redirectar till den färdigladdade sidan. Det gör det något lättar att vänta, även om man ofta också tittar på något annat ett tag och låter itailor ladda i bakgrunden. Jag var väldigt positivt överraskad av tailorstores höga resultat för datorer.
Att alla sidorna har dåliga resultat för mobiler var som sagt var inte överraskande. Själva konceptet för sidorna är att du skall designa din egen skjorta ta dina mått och sedan beställa. Det är nog något du oftast gör hemma med tillgång till en dator, för designdelen vill du nog ofta också ha tillgång till en större skärm. Jag hade dock trott att det skulle ha lagts lite mer kraft på att få till snabba första sidor och om-sidor även på mobiler. Trots allt så det nog först med en mobil som du hittar sidorna och får upp ett intresse för dem.

Minska svarstiderna från servern (tid till första byte) är nog den förbättring som pagespeed föreslår oftast om man ser till alla sidor, däremot är det långt ifrån alltid som den har mycket effekt. För både itailor och tailorstore är förbättringen "Ta bort oanvänd CSS" vanligt förekommande och det är också den förbättring jag tror skulle ge bäst effekt givet uppskattade tidsförbättringar från Pagespeed. Att ta bort resurser som blockerar renderingen är vanligt förekommande på alla platserna och kan antgligen ge en del förbättringar också. Givetvis förekom förslag om att optimera bilderna på ett eller annat sätt på alla siter, men det var inte alls i så stor utsträckning som jag hade förväntat mig och det var lite olika förslag som förekom, "Skicka bilder i modernare bildformat", var nog vanligast följt av "Koda bilder effektivt".

Jag skulle tro att samtliga sidor också bör se över antalet resurser som laddas då det är ett stort antal, speciellt på designsidorna. Itailor bör definitivt se över sina tredjepartsresurser då de enligt pagespeeds diagnostik ofta stoppade renderingen en lång tid.

På en sådan här sida här det absolut viktigaste för mig att designverktyget fungerar bra, helst även på mobilen då jag ofta leker runt med designer på mobilen och sedan tittar närmare på dem när jag sitter vid en dator. Givetvis är också förstasidan viktig, det är ju vägen till designsidan och det är även där jag ofta upptäcker nyheter och erbjudanden som gör att jag kan vilja utvärdera sidan ytterliggare. Om sidan är viktig först om jag hittat något av intresse, där brukar jag kunna hitta sådant som fraktvillkor, var företaget är beläget, om de har några etiska åtaganden etc. sådnat kan avgöra om jag vill köpa av den webplatsen eller inte och när jag väl vill få dne informationen är det bra om jag slipper vänta. Så kriterierna är i följande ordning snabb (tid till interaktivit tillstånd) designsida på dator, snabb designsida på mobil, snabb förstasida, snabb om-sida.

Skjortfabriken är snabbast till interaktivt tillstånd på design sidan och har också snabbast laddningstider i dev-tools på samtliga sidor, så jag sätter dem som vinanre med tailor-store som en nära tvåa pga deras höga betyg på pagespeed. itailor hamnar långt efter.

Om jag skall sätta en gråns mellan en snabb och en långsam webplats så ligger dte nog på 10 sekunder, vilket innebär att samtliga platser i mitt test får räkans som långsamma. Med tanke på platsernas syfte så väntar jag mig dock en långsammare plats när jag besöker dem och det är andra kvaliteter som kan avgöra om jag kommer tillbaka eller inte.

Referenser
-----------------------

Övrigt
-----------------------

Joel Sandström, gjode arbetet själv
