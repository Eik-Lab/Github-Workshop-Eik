#Commit melding

En commit melding er en kort beskrivelse av hva du har gjort i commiten. Det er viktig at commit meldingen er kort og beskrivende. Det er også viktig at commit meldingen er på engelsk.

##Hvorfor er det viktig med gode commit meldinger?

Gode commit meldinger er viktig fordi det gjør det lettere for andre å forstå hva du har gjort i koden din. Det gjør det også lettere for deg å finne tilbake til tidligere versjoner av koden din.

##Hvordan skrive gode commit meldinger?

Vi bruker en standard for hvordan vi skriver commit meldinger. Denne standarden heter [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/). Denne standarden er laget for å gjøre det lettere å forstå hva som er gjort i en commit.

En commit melding består av en header, en body og en footer. Headeren er obligatorisk, mens body og footer er valgfritt.

###Header

Headeren består av en type, en scope og en beskrivelse. Denne delen av commit meldingen er obligatorisk.

####Type

Type er en beskrivelse av hva du har gjort i commiten. Det finnes 7 forskjellige typer:

- **build:** Endringer som påvirker byggesystemet eller eksterne avhengigheter (f.eks. npm, make, mvn).

- **ci:** Endringer i vår Continuous Integration (CI) konfigurasjon og scripts (f.eks. Travis, Circle, BrowserStack, SauceLabs).

- **docs:** Endringer i dokumentasjonen.

- **feat:** En ny feature.

- **fix:** En bug fix.

- **perf:** En kode endring som forbedrer ytelsen.

- **refactor:** En kode endring som ikke fikser en bug eller legger til en feature.

- **style:** Endringer som ikke påvirker koden (f.eks. hvit plass, formatering, manglende semikolon).

- **test:** Legger til manglende tester eller retter eksisterende tester.

####Scope
Scope er 

####Beskrivelse

Beskrivelsen er en kort beskrivelse av hva du har gjort i commiten. Den skal være på engelsk og skal ikke ha punktum på slutten.

