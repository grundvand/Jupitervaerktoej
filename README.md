# Jupitervaerktoej
Dette projektet indeholder excel-filer der kan vise analyseresultater for drikkevand, råvand og miljøfremmede stoffer i forbindelse med BNBO-screening (ikke opdateret til stancode), bemærkningsfelter samt pejlinger.\
Projektet er oprindelig udviklet til brug ved kommunal sagsbehandling men vil muligvis kunne bruges af andre.\
Projektindehaverne fraskriver sig alt ansvar ved download og brug af programmerne.\
Programmerne er gratis tilgængelige og må modificeres som man ønsker.

Udviklet af:
- Mads S. Christensen, Geolog v. Esbjerg Kommune
- Karsten B. Rud , Geolog v. Sorø Kommune

***
Opsætning af værktøjet:


1) Download Jupiterdatabasen:\
Gå på GEUS' hjemmeside og download en "PC Jupiter XL" database for det område du ønsker information omkring. Dette kan gøres fra:
- Hjemmesiden: geus.dk
- Fanen: Produkter ydelser og faciliteter > Punktet: National boringsdatabase (Jupiter)
- Punktet: Adgang til data
- Punktet: Data gennem PCjupiter og PCjupiterXL format
- Tryk på linket "Download PC Jupiter XL formatet"
- Udfyld informationerne og vælg "Access 2000" under Databaseformat\
Du modtager herefter en bekræftende email og senere en email med et link hvorfra databasen kan downloades.

2) Hent Jupiterværktøj:
- Tryk på den grønne knap her på hjemmesiden med teksten "Clone or download" og derefter "Download ZIP".
- Find placeringen af zip-filen på din computer (sandsynligvis i mappen "Overførsler").
- Højreklik på zip-filen (sandsynligvis navngivet "Jupitervaerktoej-master") og tryk "Udpak alle..."
- Åben den udpakkede mappe med samme navn som zip-filen.
- Marker alle filerne, højreklik på filen og tryk klip.
- Lav en mappe hvor du ønsker at have værktøjet liggende. Navngivningen er ikke vigtig, men kunne være "Jupiterværktøj".
Det er vigtigt at mappen er placeret lokalt, og ikke i OneDrive/Sharepoint. Bemærk, ved nogle kommuner er skrivebordet koblet til OneDrive og mappen kan derfor ikke ligge der. Eksempler hvor det kan virke at placere mappen kan være f.eks. C:\Users\BRUGERNAVN\ eller F, G, H, I-drev (mv.).
- Gå ind i mappen, højreklik og tryk "Sæt ind".

3) Flyt og navngiv Jupiterdatabasen:
- Find placeringen af databasen når "PC Jupiter XL" databasen er downloadet (sandsynligvis i mappen "Overførsler").
- Højreklik på filen og tryk klip.
- Gå til mappen med excel-filerne og videre ind i mappen "JUP_database".
- Højreklik og tryk "Sæt ind".
- Højreklik og tryk "Omdøb". Filen skal navngives "JUPITER"

4) Fjern blokering:\
Excel- og Accessprogrammerne benytter sig af macroer, computerkode der kører i programmets baggrund.
Nogle brugere oplever at Microsoft Office har blokeret muligheden for at køre macroer i baggrunden.
For at fjerne blokeringen skal man gøre følgende for hver Excelfil og Access-filen "JUP_forespørgsler":
- Højreklik på filen i stifinder, og tryk Egenskaber
- Afkryds "Fjern blokering" (Se evt. filen [Fjern blokering.PNG](Fjern%20blokering.PNG))
- Tryk OK
- Gentag for hver fil

5) Opsætning af link mellem Excel-filerne og jupiterdatabasen:\
Åben Microsoft Access Database filen "JUP_forespørgsler" der er placeret sammen med Excel-filerne. Det er programmet Microsoft Access du skal bruge til at åbne filen med som er en del af Microsoft Office pakken. Hvis du ikke umiddelbart har programmet installeret se i dit softwarecenter eller kontakt din lokale IT afdeling.
- Vælg "Eksterne data" i øverste menu
- Vælg "Ny datakilde">"Fra database">Access i rubrikken "Importér og sammenkæd".
- Under "Angiv datakilden" vælg "Gennemse..." og find mappen med excel-filerne og gå ind i undermappen "JUP_database".
  Vælg databasen "JUPITER".
- Vælg punktet "Opret en kæde til datakilden ved at oprette en sammenkædet tabel" og tryk OK.
- Tryk knappen "Marker alt" og derefter OK.
- Luk filen du er i.\
Koblingerne mellem excel-filerne og den downloadede udgave af Jupiterdatabasen skulle nu gerne være sat op så excel-filerne kan bruges.

6) Nyt download af Jupiter:\
Da det er en downloadet udgave af Jupiter vil nyt data ikke komme ind. Derfor kan man vælge at downloade en ny udgave af Jupiter-databasen hver eller hver anden måned.
- Start med at omdøbe den forældede Jupiter-database til fx "JUPITER_01_01_2018".
- Følg ovenstående punkt 1) "Download Jupiterdatabasen".
- Følg ovenstående punkt 3) "Flyt og navngiv Jupiterdatabasen".
- Det er IKKE nødvendigt at følge punkt 5) "Opsætning af link mellem Excel-filerne og jupiterdatabasen" da "JUP_forespørgsler" linker til filen med navnet "JUPITER", som nu er navnet på den nye udgave af Jupiter-databasen.

7) Ny version af excelfilerne:\
Hvis der kommer en ny version af en eller flere excel-filer kan de downloades som beskrevet i punkt 2) "Hent Jupiterværktøj".\
Ved blot at klippe de nye excel-filer fra den udpakkede zip-fil over i mappen Jupiterværktøj (og overskrive de gamle excel-filer) undgår man at skulle lave en ny opsætning af "JUP_forespørgsler".

***
Følgende mangler:
- Opdatering af forespørgslerne i JUP_forespørgsler. Disse kører stadig på de gamle standat-kodelister og giver derfor forkert resultat.
- Beskrivelse af brugen af de enkelte excel-filer.
