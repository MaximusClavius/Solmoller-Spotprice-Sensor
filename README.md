# Grønnere elforbrug spotpris DK1
7 day forecast on spot prices for electricity/7 dags prognose på spotpriser på el

En prognose udviklet af Henrik Møller Jørgensen, https://github.com/solmoller/Spotprisprognose. Vi samarbejder om at få data i Homeassistant på en ubesværet måde...
Spotpriser er i €/MWh, så i kr/kWh skal der / 1000 * 7.44 * 1.25 (1000 -> til kWh, 7.44 kurs på €, 1.25 med moms). Tiden er angivet i UTC. Bemærk der både er data for DK1 og DK2, så er man interesseret i data for DK2 skal man ændre DK1 til DK2 under json_attributes for sensoren eller tilføje begge.

TO-DO:
1) Tilføj sensor
2) Tilføj kort (Søjlediagram)

Ad 1:
Hele koden til sensor smides ind i configuration.yaml eller bruger du separat fil til sensorer, så alle linjer undtagende den første (som starter med sensor). Eventuel "TJEK KONFIGURATION" og derefter "GENSTART"! Alternativt kan man nøjes ned "GENINDLÆS KOMMANDOLINJE ENTITETER", hvis denne funktionalitet er aktiveret.

Ad 2:
"Tilføj kort" til din brugergrænseflade/dashboard, og vælg apexcharts-card. Så kopier du koden ind vinduet til venstre, så skulle diagrammet komme til syne i højre vindue. Diagramet bruger grøn, gul og rød farve for at markere forskelle pris, hvor grøn er lavest og rød højest. Nærværende diagram viser DK1 og ønsker man DK2 skal DK1 byttes med DK2 under data_generator for diagrammet (såfremt det findes under json_attributes på sensor).
Beskrevet diagram ligner dette:

![image](https://user-images.githubusercontent.com/103023823/183561276-8a567a09-59d7-4817-9c88-9c9f3ae99605.png)

PS
Viser diagrammet "Loading" i stedet for data fra sensor, så er formentlig noget gal med formattering af koden eller ikke komplet kopiering. Vælg ikon "Copy raw content" på Github, og brug Ctrl+a for at markere al tekst og indsæt/erstat med Ctrl+v...
