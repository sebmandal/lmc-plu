README for Oblig 1 i IN1020

Navn: Sebastian Wilhelm Kristian Pritchard-Davies Mandal

Merk: Jeg klarte å bruke feil simulator og skjønte ikke det før det var alt for sent. Jeg rakk å skrive oppgaven på nytt slik at den fungerer og dekker alle kravene, men hvis dere ønsker å se de tidligere versjonene med litt mer funksjonalitet (beskrevet under) gjerne ta en titt på [Github-siden](https://github.com/sebmandal/lmc-plu) :)

Bruk Tab Size 8 for lesbarhet i `kode.txt`.

---

### PLU Koder

PLU 1 med pris på 100
PLU 2 med pris på 200

---

Versjoner og Utfordringer Møtt

Se versjoner på [Github](https://github.com/sebmandal/lmc-plu). Jeg legger ut denne rett etter fristen slik at ingen kan plagiere løsningen min.

1. Første Versjon

Funksjonalitet: Denne versjonen lar deg skrive en PLU (alle unntatt 0 har samme funksjonalitet) og spør om mengde av varen du ønsker å kjøpe.
Utfordringer: Ingen store utfordringer. Jeg måtte bare bli vant til språket og måten å skrive kode på i det.

2. Andre Versjon

Funksjonalitet: Denne versjonen lar deg velge mellom flere produkter. Hvis du velger et produkt som ikke eksisterer, vil den kaste en utfordring.
Utfordringer:
1. Hvordan kan jeg sjekke pris dynamisk? Svar: Jeg kunne ikke gjøre dette. Jeg måtte legge til en redundant funksjon for å sjekke om en PLU er valgt, og så assigne prisen til prisvariabelen.
2. Hvordan kan jeg gjøre koden lesbar? Svar: Jeg delte opp alle funksjonene i sine respektive roller, slik at alle funksjoner er lette å forstå, og én funksjon gjør bare én ting.

3. Tredje Versjon

Funksjonalitet: Denne versjonen legger til funksjonalitet for error handling og lagerstyring.

3-a. Variabler

For eksempel, for eple med PLU 405:

- `405` heltall 405
- `P405` pris for eple
- `S405` tilgjengelighet for eple

3-b. Error Meldinger

- 501 for PLU error (produktet eksisterer ikke)
- 502 for COUNT error (antall varer ønsket er mindre enn 0)
- 503 for STOCK error (vi har ikke nok av dette produktet til å kjøpe mengden du etterspør)

Spesifikasjoner: Hvis det kommer en error-kode i OUTPUT, må du skrive input på nytt. Systemet går ikke videre før det har fått en riktig kode, unntatt START-funksjonen som alltid vil spørre om både PLU og COUNT, uansett om PLU ikke eksisterer. Derfor er det viktig å være kjent med error kodene.
Utfordring: Hvordan gjøre error handling? Svar: Jeg måtte endre en del kode og håndtering av inputs slik at jeg kan sjekke ting på slutten uten å gjøre logikk før den har sjekket.

4. Versjon ved Fristen

OPPDATERING: Massiv feil fra min side, stor utfordring haha. Jeg hadde brukt feil simulator hele tiden. Koden min gir ingen errormeldinger på Peter Higginson simulatoren, men den går i en uendelig loop et eller annet sted i koden. Jeg må fikse dette ASAP og så dette når jeg leste over for å levere inn klokken 22:53 på innleveringsdagen.

Status: Den nye versjonen er veldig barebones og har bare nødvendig funksjonalitet til oppgavebeskrivelsen, men alt kjører fint.

Jeg rakk det, woo!