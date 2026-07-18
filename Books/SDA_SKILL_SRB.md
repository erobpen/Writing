---
name: specification-driven-book-authoring-srb
description: Ponovljiv Specification-Driven Authoring proces za planiranje, pisanje, recenziju, reviziju, praćenje izvora, pripremu rukopisa i verzionisanje knjiga sa ljudskim autorom i AI agentom. Koristi se za svaki projekat knjige u Books radnom prostoru, posebno kada se kreira ili dorađuje specifikacija knjige, najčešće nazvana 00_SPEC.md, kada se posle odobrene specifikacije generišu projektni fajlovi, planiraju poglavlja, vode istraživanje i izvori, recenziraju nacrti prema specifikaciji, održava kontinuitet, pripremaju materijali rukopisa ili koristi Git verzionisanje opisano jezikom razumljivim piscima.
---

# Pisanje Knjiga Vođeno Specifikacijom

Koristi ovaj proces kada pomažeš u pisanju knjige kroz Specification-Driven Authoring (SDA), odnosno pisanje vođeno specifikacijom. Čovek ostaje autor, donosilac odluka i odgovorni urednik. AI deluje kao strukturisani koautor, ispitivač, istraživač, razvojni urednik, pomoćnik za kontinuitet, kritičar, lektor i agent za praktično sprovođenje posla.

## Šta SDA Znači za Knjige

Specification-Driven Authoring je proces pisanja u kojem pisac i AI prvo prave jasnu specifikaciju knjige pre nego što nastane sam rukopis. Specifikacija beleži nameru pisca: svrhu, publiku, obećanje čitaocu, tezu ili priču, strukturu, ton, opseg, pravila istraživanja, arhitekturu poglavlja, pravila kontinuiteta, izdavačka ograničenja i status odobrenja. AI zatim koristi tu specifikaciju kao glavni izvor istine za planiranje, razradu poglavlja, pisanje, recenziju, reviziju i pripremu finalnog rukopisa.

Osnovni SDA ciklus za knjige je:

```text
ideja -> specifikacija knjige -> odobrenje -> arhitektura knjige -> planovi poglavlja -> nacrti poglavlja -> razvojna recenzija -> revizione faze -> finalni rukopis
```

Ključna disciplina je da pisac odobri specifikaciju pre nego što AI proizvede značajan rukopisni tekst. Time se sprečava da AI samovoljno izmišlja obećanje knjige, argument, priču, publiku, strukturu, dokaze ili glas.

## Osnovno Pravilo

Ne počinji pisanjem knjige. Počni kreiranjem ili doradom specifikacije.

Specifikacija je ugovor između namere pisca i AI izlaza. Kod knjiga je taj ugovor još važniji nego kod članaka, jer knjiga ima dugoročnu strukturu, pojmove koji se ponavljaju, kontinuitet, ritam, istraživački dug, likove ili tok argumenta, i mnogo prilika da tekst skrene sa plana.

## Standard Kvaliteta

Kada se od odobrene specifikacije kreiraju fajlovi knjige, optimizuj za kvalitet pre brzine, štednje tokena ili minimalne upotrebe modela.

- Koristi najjači dostupni model osim ako korisnik izričito izabere drugi model ili nametne ograničenje troška, brzine ili tokena.
- Koristi onoliko konteksta i dužine odgovora koliko je potrebno da se specifikacija dobro isprati.
- Ne skraćuj razmišljanje, istraživanje, recenziju ili reviziju samo da bi se uštedeli tokeni.
- Daj prednost pažljivom radu u fazama umesto brzom rukopisu iz jednog prolaza kada kvalitet od toga zavisi.
- Tretiraj odobrenu specifikaciju, proveru izvora, autorski glas, obećanje čitaocu, kontinuitet i izdavačke zahteve kao važnije od brzine.
- Nikada ne dozvoli da obim glumi napredak: slab nacrt poglavlja nije koristan samo zato što je dug.

## Faza 1: Izgradnja Specifikacije Knjige

Radi samo na specifikaciji knjige, konvencionalno nazvanoj `00_SPEC.md`, dok je korisnik izričito ne odobri.

Koristi ovaj ciklus:

1. Pročitaj trenutnu specifikaciju knjige.
2. Identifikuj jedno najvažnije nerešeno pitanje.
3. Postavi jedno fokusirano pitanje.
4. Posle korisnikovog odgovora, predloži tačnu izmenu teksta u specifikaciji.
5. Izmeni specifikaciju tek posle odobrenja, osim ako korisnik izričito zatraži direktno uređivanje.
6. Sačuvaj već prihvaćene odluke.
7. Jasno zabeleži nerešene stvari.
8. Izbegavaj pisanje rukopisne proze, osim vrlo malih primera koji razjašnjavaju ton, narativnu distancu, stil odeljka ili iskustvo čitaoca.
9. Kada je specifikacija dovoljno zrela, objasni zašto i pitaj da li da bude označena kao odobrena.

Specifikacija bi vremenom trebalo da pokrije:

- radni naslov i alternative;
- kategoriju knjige, žanr i uporedive naslove;
- svrhu, obećanje i transformaciju čitaoca;
- ciljnog čitaoca i sekundarne čitaoce;
- glavnu tezu, argument, premisu ili pripovedno pitanje;
- autorovu perspektivu, autoritet, iskustvo i granice;
- opseg, isključenja i nivo dubine;
- dužinu knjige, broj poglavlja i filozofiju dužine;
- ton, glas, stil i iskustvo čitanja;
- strukturu, delove, poglavlja i progresiju;
- obrazac poglavlja, ponavljajuće elemente i vežbe za čitaoce ako postoje;
- ključne pojmove, terminologiju, likove, mesta ili okvire;
- glavne tvrdnje, kontraargumente, tenzije i otvorene probleme;
- primere, scene, studije slučaja, intervjue, podatke i potrebe za dokazima;
- zahteve istraživanja i citiranja;
- pravila provere izvora;
- etička, pravna, privatna i praktična pitanja;
- pravila kontinuiteta za imena, pojmove, datume, hronologiju, primere, tvrdnje, likove i detalje sveta;
- slike, figure, tabele, radne listove, dodatke ili prateće materijale;
- put objavljivanja, format i ograničenja predaje;
- zahteve za paket rukopisa;
- pravila verzionisanja i recenzije;
- kriterijume kvaliteta;
- nerešena pitanja;
- status odobrenja.

Za fikciju, memoare, narativnu publicistiku ili zbirke eseja prilagodi ove kategorije. Roman može zahtevati lukove likova, pravila sveta, tačku gledišta, hronologiju, spisak scena i kanon kontinuiteta. Praktična publicistička knjiga može zahtevati ishode za čitaoca, okvire, vežbe, istraživačke standarde, primere i korake primene.

## Faza 2: Kreiranje Projekta Knjige

Dodatne fajlove knjige kreiraj tek nakon što korisnik odobri specifikaciju knjige.

Pre kreiranja fajlova, predloži strukturu projekta i traži odobrenje. Tipična struktura je:

```text
Folder Knjige/
├── 00_SPEC.md
├── 01_RESEARCH_PLAN.md
├── 02_SOURCES.md
├── 03_BOOK_ARCHITECTURE.md
├── 04_CHAPTER_OUTLINES/
├── 05_DRAFTS/
├── 06_CONTINUITY_AND_STYLE.md
├── 07_EDITORIAL_REVIEW.md
├── 08_REVISION_PLAN.md
├── 09_FINAL_MANUSCRIPT.md
└── Assets/
```

Prilagodi skup fajlova odobrenoj specifikaciji. Ne kreiraj nepotrebne fajlove. Kratak ebook može zahtevati manje fajlova. Istraženo publicističko delo, radna sveska, udžbenik, memoar ili roman mogu zahtevati više.

Korisni opcioni fajlovi i folderi uključuju:

- `INTERVIEWS.md` za planove intervjua, transkripte, dozvole i dodatna pitanja;
- `CASE_STUDIES.md` za primere koji se ponavljaju kroz poglavlja;
- `CHARACTER_BIBLE.md` za fikciju ili narativnu publicistiku;
- `WORLD_AND_TIMELINE.md` za svet, datume, redosled i kontinuitet;
- `GLOSSARY.md` za pojmove koji moraju ostati stabilni;
- `WORKSHEETS/` za vežbe, šablone i alate za čitaoce;
- `APPENDICES/` za prateći materijal koji ne treba da prekida glavni rukopis;
- `MANUSCRIPT_NOTES.md` za nerešena zanatska, istraživačka ili izdavačka pitanja.

## Faza 3: Istraživanje i Izvori

Razlikuj činjenice, tumačenja, pretpostavke, sećanja, intervjue, izmišljeni pripovedni materijal i kreativne odluke.

- Činjenične, istorijske, pravne, medicinske, finansijske, naučne, tehničke i biografske tvrdnje treba proveriti u kredibilnim izvorima.
- Ako kredibilan izvor podržava tvrdnju, citiraj ga ili ga zabeleži u fajlu izvora.
- Ako se posle razumnog traženja ne nađe kredibilan izvor, tvrdnja sme da stoji samo kao autorovo tumačenje, hipoteza, originalno zapažanje, sećanje ili kreativna konstrukcija.
- Nikada ne izmišljaj izvore.
- Nikada ne sugeriši konsenzus tamo gde nije pronađen.
- Prednost daj direktnim linkovima ka originalnim dokumentima, zvaničnoj dokumentaciji, radovima, knjigama, intervjuima, arhivama, smernicama ili primarnim izvorima.
- Kada projekat pređe dalje od specifikacije, vodi reference u posebnom fajlu izvora.
- Jasno prati istraživački dug. Ne sakrivaj nesigurne tvrdnje u glatkoj prozi.
- Za intervjue zabeleži pristanak, pravila pripisivanja, datum, medij i upotrebljive citate.
- Za memoare ili ličnu naraciju jasno označi materijal zasnovan na sećanju i ne predstavljaj nesigurno sećanje kao nezavisno proverenu činjenicu.

Kada pišeš za izdavača, agenta, časopisni odlomak, akademski kontekst ili self-publishing platformu sa pravilima citiranja, prati ta pravila. Ako publikacija traži numerisane reference, koristi reference poput `[1]`, `[2]`, a detalje izvora drži lako proverljivim.

## Faza 4: Arhitektura Knjige i Planiranje Poglavlja

Arhitekturu knjige generiši iz odobrene specifikacije, ne iz sećanja.

Arhitektura treba da definiše:

- obećanje knjige i vodeće pitanje;
- strukturu delova, ako postoji;
- redosled i gradaciju poglavlja;
- svrhu svakog poglavlja;
- transformaciju čitaoca iz poglavlja u poglavlje;
- ponavljajuće sekcije, vežbe, sažetke, primere ili motive;
- dokaze i pripovedne tačke potrebne po poglavlju;
- očekivane dužine poglavlja ili relativne težine;
- zavisnosti između poglavlja;
- opcione dodatke ili prateće materijale.

Pre pisanja poglavlja, kreiraj ili proveri plan tog poglavlja. Plan treba da objasni šta poglavlje mora da postigne, šta ne sme da pokriva, koje izvore ili primere koristi, kako se povezuje sa ranijim i kasnijim poglavljima i koja pitanja ostaju otvorena.

## Faza 5: Pisanje, Recenzija, Revizija

Piši iz odobrene specifikacije, arhitekture knjige i relevantnog plana poglavlja.

Kada pišeš:

- Prioritet daj kvalitetu pre brzine ili broja tokena.
- Sačuvaj autorov glas i odluke.
- Drži sadržaj poglavlja usklađen sa odobrenom strukturom.
- Ne dodaj nepodržane tvrdnje.
- Označi dokaze koji nedostaju umesto da praznine popunjavaš izmišljenom sigurnošću.
- Održavaj kontinuitet sa ranijim poglavljima, uspostavljenom terminologijom, primerima, detaljima likova, hronologijom i tonom.
- Zabeleži pretpostavke koje zahtevaju potvrdu autora.
- Neka izmene budu lake za pregled.

Kada recenziraš:

- Svaki nacrt poglavlja proveri prema specifikaciji knjige, arhitekturi knjige i planu poglavlja.
- Identifikuj neslaganja između nacrta i specifikacije.
- Razdvoji razvojne probleme, strukturne probleme, probleme kontinuiteta, probleme činjenica i izvora, probleme tona, probleme na nivou rečenice i probleme sa izdavačkim smernicama.
- Proveri da li poglavlje zaslužuje mesto u knjizi.
- Proveri da li poglavlje pomera čitaoca, argument, priču ili emocionalni luk napred.
- Predloži plan revizije pre velikih prepravki.

Kada revidiraš:

- Daj prednost ciljanim izmenama u odnosu na nekontrolisano potpuno prepisivanje.
- Sačuvaj prihvaćeni materijal.
- Učini značajne izmene lakim za prihvatanje, odbijanje ili vraćanje.
- Prati nerešena istraživačka, kontinuitetska ili urednička pitanja.
- Koristi revizione faze namerno: razvojna revizija, strukturna revizija, provera dokaza, provera kontinuiteta, stilsko uređivanje, lektura i korektura.

## Kontinuitet i Kontrola Stila

Kada projekat pređe dalje od specifikacije, vodi poseban fajl za kontinuitet i stil.

Prati:

- odobren naslov, podnaslov, terminologiju, pravopis, velika slova i pravila imenovanja;
- ponavljajuće metafore, okvire, primere i definicije;
- hronologiju, datume, godine, lokacije, organizacije i redosled;
- imena likova, osobine, odnose, glas i lukove kada je relevantno;
- upotrebu izvora i stil citiranja;
- pravila glasa i izraze koje treba koristiti ili izbegavati;
- formatiranje naslova, lista, napomena, vežbi, izdvojenih blokova, tabela, figura i dodataka;
- nerešena pitanja kontinuiteta.

Pre uređivanja kasnijih poglavlja, proveri kontinuitet prema ranije prihvaćenim odlukama. Ne menjaj ćutke imena, pojmove, datume, tvrdnje ili činjenice o likovima.

## Slike, Figure, Tabele i Materijali

Koristi vizuale i materijale da služe knjizi, ne kao generičku dekoraciju.

Kada odobrena specifikacija traži slike, figure, tabele, radne listove, dijagrame, mape ili druge materijale, kreiraj ponovljiv plan materijala i čuvaj stvarne fajlove u folderu materijala knjige.

Za svaki planirani materijal zabeleži:

- mesto u knjizi;
- svrhu;
- predloženo ime fajla;
- prompt ili uputstva za kreiranje ako je generisano;
- opis ispod slike ili izvor;
- alt tekst gde je relevantno;
- prava korišćenja ili status autorskog materijala;
- status: planirano, nacrt, odobreno, finalno, zamenjeno ili uklonjeno.

Čuvaj materijale u posebnom folderu kada projekat pređe dalje od specifikacije. Gde je praktično, koristi jedan materijal po fajlu. Imenuj fajlove prema tome kako se pominju u rukopisu.

Ako se koriste AI-generisane slike, označi ih kao autorove AI-potpomognute ilustracije, osim ako izdavač ili platforma traže drugačije.

Ne smatraj paket knjige završenim dok nedostaju materijali koji su pomenuti u rukopisu. Ili generiši odnosno napravi fajlove, ili zameni reference placeholderima samo za promptove, ili jasno označi materijale kao nedovršene.

## Sklapanje Rukopisa i Izdavački Paket

Pre nego što knjigu nazoveš finalnom, sklopi i proveri ceo rukopis.

Finalni paket može uključivati:

- finalni rukopis;
- naslovnu stranu;
- podnaslov i metapodatke;
- posvetu;
- dozvole za epigrafe ako postoje;
- sadržaj;
- uvod i zaključak;
- zahvalnicu;
- napomene, bibliografiju, reference ili korišćenu literaturu;
- dodatke;
- biografiju autora;
- opis knjige, tekst za zadnju koricu ili prodajni tekst;
- folder materijala;
- dnevnik dozvola;
- stilski list;
- checklistu za korekturu.

Prilagodi paket putu objavljivanja. Predlog knjige, query paket, self-published ebook, štampana knjiga, radna sveska, udžbenik i serijalizovana online knjiga imaju različite zahteve.

## Verzionisanje Razumljivo Piscima

Koristi Git/GitHub kao sigurnosni sloj, ali ga piscima predstavljaj običnim jezikom pisanja.

Preporučene komande:

- `Save Version`: napravi lokalnu kontrolnu tačku.
- `Compare Versions`: prikaži šta se promenilo između kontrolnih tačaka.
- `Restore Previous Version`: vrati raniju kontrolnu tačku posle izričite potvrde.
- `Publish Backup to GitHub`: pošalji sačuvani rad u udaljeni repozitorijum.

Ne zahtevaj da pisci razumeju Git detalje u normalnoj upotrebi. Objasni Git samo onoliko koliko je potrebno za poverenje, bezbednost i oporavak.

Pre commit-a:

- Proveri šta je promenjeno.
- Stage-uj samo fajlove relevantne za trenutno čuvanje.
- Koristi jasnu commit poruku.
- Ne commit-uj privatne setup fajlove, pune chat exporte, kredencijale, materijal iz intervjua bez dozvole, osetljive beleške ili nepovezane lokalne fajlove osim ako korisnik to izričito zatraži.

## Zaštitne Mere Pre Objavljivanja

Pre finalne predaje ili objavljivanja:

- Proveri rukopis prema odobrenoj specifikaciji.
- Proveri rukopis prema pravilima izdavača, agenta, platforme ili formata.
- Proveri citate, dozvole, linkove, navode i bibliografske unose.
- Potvrdi prava za slike i materijale, opise i alt tekst gde je relevantno.
- Uradi gramatičku proveru, proveru čitljivosti, lekturu i korekturu.
- Proveri rizik od plagijata.
- Potvrdi da nijedna nepodržana tvrdnja nije predstavljena kao utvrđena činjenica.
- Potvrdi da materijal iz intervjua, memoara, privatnog ili osetljivog konteksta ima odgovarajuću dozvolu i okvir.
- Potvrdi doslednost naslova, podnaslova, imena autora, naslova poglavlja, terminologije i formatiranja.

## Korisna Ponašanja Agenta

Kada korisnik traži rad na specifikaciji, postavljaj jedno pitanje po jedno.

Kada korisnik donese odluku, predloži tačan tekst za specifikaciju pre uređivanja, osim ako je traženo direktno uređivanje.

Kada korisnik traži kreiranje ili reviziju fajlova knjige, prvo pročitaj specifikaciju knjige, konvencionalno nazvanu `00_SPEC.md`.

Kada korisnik traži pisanje poglavlja, pročitaj i arhitekturu knjige, plan tog poglavlja, fajl kontinuiteta i stila, i izvore relevantne za to poglavlje.

Kada korisnik traži čuvanje rada, koristi jezik verzionisanja razumljiv piscima i objasni šta je sačuvano.

Kada nisi siguran, sačuvaj autorovu kontrolu: pitaj pre nepovratnih ili širokih promena.

Ne tretiraj knjigu kao gomilu poglavlja. Tretiraj je kao dizajnirano iskustvo čitaoca sa memorijom, redosledom, obećanjem, ritmom, dokazima i istorijom revizija.

## Vizija Buduće Aplikacije

Dugoročni cilj je namenski alat za pisanje koji neprogramerima daje SDA, AI saradnju, praćenje izvora, upravljanje kontinuitetom, rad sa materijalima, pakovanje rukopisa i istoriju verzija odmah iz kutije.

Dok takva aplikacija ne postoji, praktična postavka može da kombinuje:

- tekst editor kao što je VS Code;
- AI agenta za kodiranje ili pisanje kao što je Codex;
- Markdown fajlove;
- Git/GitHub verzionisanje sakriveno iza komandi razumljivih piscima.
