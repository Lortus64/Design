Laddningstid och användbarhet
=======================

Detta är en rapport om hur olika sidor laddar och hur användbara de är.

Urval
-----------------------

Jag försökte välja tre sidor som hade olika syften, utseende och mängd saker på sidan.

[Steam](https://store.steampowered.com/)
Jag började först med Steam som är en ett företag som säljer spel. Sidan har ganska mycket att ladda in. Sidan är full med länkar och bildspel.

[Wikipedia](https://sv.wikipedia.org/wiki/Portal:Huvudsida)
Sen valde jag wikipedia. Sidan har inte jättemycket på sig utan nästan allt är brödtext. Men troligen händer det ganska mycket i bakgrunden. Mycket data ska hämtas från en databas.

[Tesla](https://www.tesla.com/sv_se)
Den sista jag valde var tesla. Sidan har en väldigt spännande stil med videor och vad som ser ut som interaktiva bilder/ bildspel.

Metod
-----------------------

Alla mina tester gjordes i chrome för att alla sidor skulle ha samma förutsättninghar.
Först så anväder jag [Page Speed Insight](https://developers.google.com/speed/pagespeed/insights/). Denna sidan analyserar hur en sida laddas och hur den jämförs med lighthouse Scoring. Sen använd jag chromes inspect tool för att kolla nätverksinfo. Sist samlade jag all data i ett googel drive document.

Resultat
-----------------------

[Document med data](https://docs.google.com/spreadsheets/d/1VCB1ToxlFBDNpWgo58y22U9e9l5pfWetBM1h1l7sQBU/edit?usp=sharing)

**Steam**: [FIGURE src=image/steam.PNG?w=300 caption="Steam startsida."]
Steam hade väldigt mycket problem gällande bilderna. Det de kan göra är att minska antalet bilder eller använda dem i ett annat format för att minska laddningstiden. Datan jag fick här kan vara felaktig då sidan hade mycket data som kom när man utforskade sidan (mycket gömda bilder). 

**Wikipedia**: [FIGURE src=image/wiki.PNG?w=300 caption="Wikipedia startsida."]
Wikipedia var lätt den sidan som laddade snabbast. I alla mina försök så laddade sidan under en sekund. Detta kan bero på att sidan är ganska liten jämfört med alla andra sidor jag valde. Det som man hade kunnat ändra är antalet DOM element vilket enligt pagespeed skulle vara över 970st.

**Tesla**: [FIGURE src=image/tesla.PNG?w=300 caption="Tesla startsida."]
Tesla var den sidan som fick sämst betyg detta kan bero på mycket oanvänd css och många ställen som blockar rendering. Detta ser ut att bero på att sidan använder mycket css-kod som stoppar sidans rendering. Tesla hade samma typ av svårighet som steam mycket av sidan laddar inte föränns den behövs vilket gjorde den svår att få data ifrån.

Analys
-----------------------

Jag hittade ett tydligt mönster i att alla sidornas mobilversion var alltid sämre när det gällde betyg och hastighet. Detta beror troligen på att sidan börjar som desktop sida sen tvingar proggramerarna ner det till en mobilsida. Troligen hade det varit andra resultat om sidan var gjord för mobil från början. Jag såg även att många av sidorna hade css element som aldrig användes men även att bilder inte hade rätt format.

Om jag ska utse en vinnare bland mitt urval så är det lätt wikipedia. Sidan är den minsta men den laddade extremt snabbt och hade ett väldigt bra betyg på båda desktop och mobil. Den sidan jag skulle säga var näst bäst var steam. Med tanke på hur mycket bilder och annat som är på sidan så är den förvånansvärt snabb. Sen vet jag från tidigare år att sidan har svårigheter att hantera när det är väldigt många på den. Tesla är därför automatiskt den sämsta. Sidan är väldigt imponerade designvis men många av sidorna kan ta lite tid att ladda in. Jag skulle fortfarande säga att den är mer än acceptabel.

Den absoluta laddningstiden för en sida får variera beroände på hur mycekt som finns på sidan. Så om wikipedia hade tagit 4 sekunder att ladda hade sidan troligen inte varit acceptabel men en sida som steam hade varit acceptabel vid den tiden. Teslas modelS sida är dock inte acceptabel med en laddningstid på 16 sekunder.

Övrigt
-----------------------
Adam Eriksson