Første versjon, denne bare lar deg skrive en PLU (alle unntatt 0 har samme funksjonalitet) og spør om mengde av denne varen du ønsker å kjøpe.

Ingen utfordringer så langt, jeg måtte bare bli vant til språket og måten man skriver kode på i det.

Andre versjon, denne versjonen lar deg velge mellom flere produkter, hvis du velger et produkt som ikke eksisterer vil den kaste deg utfordringer

Jeg møtte to utfordringer her:
1. Hvordan kan jeg sjekke pris dynamisk? Svar: Jeg kunne ikke det, jeg må bare legge til en redundant funksjon for å sjekke om det er valgt en PLU også assigne prisen til pris variablen.
2. Hvordan kan jeg gjøre det lesbart? Svar: Jeg splittet alle funksjonene inn i sine respektive roller, slik at alle funksjoner er lette å forstå og at én funksjon aldri gjør mer enn én ting.