# Grønnere elforbrug spotpris DK1
7 day forecast on spot prices for electricity/7 dags prognose på spotpriser på el

En prognose udviklet af Henrik Møller Jørgensen. Vi samarbejder om at få data i Homeassistant på en ubesværet måde...

Sensor skal indsættes i configuration.yaml eller den fil du bruger til sensorer i HA.
Bemærk der både er data for DK1 og DK2, så er man interesseret i data for DK2 skal man ændre DK1 til DK2 under json_attributes for sensoren eller tilføje begge.

Diagramet bruger grøn, gul og rød farve for at markere forskelle pris, hvor grøn er lavest og rød højest. Nærværende diagram viser DK1 og ønsker man DK2 skal DK1 byttes med DK2 under data_generator for diagrammet (såfremt det findes under json_attributes på sensor).
Beskrevet diagram ligner dette:

![image](https://user-images.githubusercontent.com/103023823/183420148-10577d41-54ba-41e4-a32d-a9570fd535de.png)
