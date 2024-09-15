# README for Oblig 1 i IN1020

- Sebastian Wilhelm Kristian Pritchard-Davies Mandal

## PLU koder

- Jeg har PLU 405 for eple, med pris 5 og tilgjengelighet på 8

- Jeg har PLU 307 for rundstykke, med pris på 7 og tilgjengelighet på 5

- Jeg har PLU 303 for appelsin, med pris på 9 og tilgjengelighet på 10

## Versjoner og utfordringer møtt

Se versjoner på [Github](https://github.com/sebmandal/lmc-plu-management)

###### Jeg legger ut denne rett etter fristen slik at ingen kan plagiere løsningen min.

### Første versjon

Denne bare lar deg skrive en PLU (alle unntatt 0 har samme funksjonalitet) og spør om mengde av denne varen du ønsker å kjøpe.

#### Ingen utfordringer så langt, jeg måtte bare bli vant til språket og måten man skriver kode på i det.

### Andre versjon

Denne versjonen lar deg velge mellom flere produkter, hvis du velger et produkt som ikke eksisterer vil den kaste deg utfordringer

#### Jeg møtte to utfordringer her:

1. Hvordan kan jeg sjekke pris dynamisk? Svar: Jeg kunne ikke det, jeg må bare legge til en redundant funksjon for å sjekke om det er valgt en PLU også assigne prisen til pris variablen.
2. Hvordan kan jeg gjøre det lesbart? Svar: Jeg splittet alle funksjonene inn i sine respektive roller, slik at alle funksjoner er lette å forstå og at én funksjon aldri gjør mer enn én ting.

### Tredje versjon

Denne versjonen legger til funksjonalitet for error handling og stock management

#### Nå har jeg de følgende variablene for hver vare:

(eksempel 405 - eple)

- `405 - heltall 405`

- `P405 - pris for eple`

- `S405 - tilgjengelighet for eple`

#### Nå har jeg error meldinger som består av følgende:

- 501 for PLU error (produktet eksisterer ikke)
- 502 for COUNT error (antall varer ønsket er mindre enn 0)
- 503 for STOCK error (vi har ikke nok av dette produktet til å kjøpe mengden du etterspør)

Enda en ting med denne versjonen er at hvis det kommer en error-kode i OUTPUT, så betyr det alltid at du må skrive input på nytt. Den går ikke videre før den har fått en riktig kode.

Dette er med unntak av START funskjonen, der den alltid vil spørre både om PLU og COUNT uansett om PLU ikke eksisterer.

Derfor er det viktig å være kjent med error kodene.

#### Jeg møtte en utfordring her også:

1. Hvordan kan jeg gjøre error handling? Svar: Jeg måtte endre på en del kode og hvordan jeg håndterer inputs slik at jeg kan sjekke ting på slutten uten at den gjør logikk før den har sjekket.