# Commit melding

En commit melding er en kort beskrivelse av hva du har gjort i commiten. Det er viktig at commit meldingen er kort og beskrivende. Det er også viktig at commit meldingen er på engelsk.

## Hvorfor er det viktig med gode commit meldinger?

Gode commit meldinger er viktig fordi det gjør det lettere for andre å forstå hva du har gjort i koden din. Det gjør det også lettere for deg å finne tilbake til tidligere versjoner av koden din.

## Hvordan skrive gode commit meldinger?

Vi bruker en standard for hvordan vi skriver commit meldinger. Denne standarden heter [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/). Denne standarden er laget for å gjøre det lettere å forstå hva som er gjort i en commit.

Nå skal vi lære dere en forenklet versjon av denne standaren. 
Man trenger da en type og en en beskrivelse.

### Type

Type er en beskrivelse av hva du har gjort i commiten. Det finnes 7 forskjellige typer:

De to viktigste er: 

- **feat:** En ny feature. En ny fil, en ny funksjon eller en ny side.

- **fix:** En bug fix. En feil i koden som er rettet.


Andre er:
- **build:** Endringer som påvirker byggesystemet eller eksterne avhengigheter (f.eks. npm, make, mvn).

- **ci:** Endringer i vår Continuous Integration (CI) konfigurasjon og scripts (f.eks. Travis, Circle, BrowserStack, SauceLabs).

- **docs:** Endringer i dokumentasjonen.

- **perf:** En kode endring som forbedrer ytelsen.

- **refactor:** En kode endring som ikke fikser en bug eller legger til en feature.

- **style:** Endringer som ikke påvirker koden (f.eks. hvit plass, formatering, manglende semikolon).

- **test:** Legger til manglende tester eller retter eksisterende tester.


#### Beskrivelse

Beskrivelsen er en kort beskrivelse av hva du har gjort i commiten. Den skal være på engelsk og skal ikke ha punktum på slutten.

