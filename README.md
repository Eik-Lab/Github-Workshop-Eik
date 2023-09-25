# Git og GitHub Workshop med Eik

Velkommen til Git og GitHub workshop! Denne workshopen er ment å gi deg en grunnleggende forståelse av hvordan du kan bruke Git og GitHub til å administrere og samarbeide om prosjekter.

# Innhold

- [1. Innledning til Git og GitHub](#1-innledning-til-git-og-github)
- [2. Før vi setter ignag](#2-før-vi-setter-i-gang)
- [3 Lag et nytt repository](#3-lag-et-nytt-repository)
- [4. Grunnleggende konsepter](#4-grunnleggende-konsepter)
- [5. Jobb med prosjektet fra VS Code](#5-jobb-med-prosjektet-fra-vs-code)
- [6. Branching og merging](#6-branching-og-merging)
- [7. Jobbe sammen med andre og merge conflicts](#7-jobbe-sammen-med-andre-og-merge-conflicts)
- [8. Merge conflicts med brancher](#8-merge-conflicts-med-brancher)


# 1. Innledning til Git og GitHub

Git er et distribuert versionskontrollsystem som hjelper deg med å spore endringer i filer over tid. GitHub er en plattform for samarbeid og deling av Git-repositorier. I denne workshopen vil du lære hvordan du bruker Git til å administrere prosjekthistorikk og hvordan du samarbeider på GitHub.

# 2. Før vi setter i gang


## 2.1 Oppsett av GitHub-konto
Hvis du ikke allerede har en GitHub-konto, kan du opprette en på https://github.com/

## 2.2 Laste ned VS Code
Vi skal bruke VS Code til å jobbe med Git og GitHub. Du kan laste ned VS Code fra [https://code.visualstudio.com/](https://code.visualstudio.com/).

## 2.3 Installasjon av GIT
Før vi begynner, må du sørge for at Git er installert på datamaskinen din. Du kan laste ned Git fra [https://git-scm.com/](https://git-scm.com/) og følge instruksjonene for din plattform.

### Windows
For å sjekke om Git er installert, kan du åpne et terminalvindu, f.eks **Windows Powershell**, og kjøre følgende kommando:
```bash
git --version
```
![Bilde av git version](pictures/wp_git.png)
Hvis Git er installert, vil du se versjonsnummeret. Hvis ikke, kan du følge instruksjonene på [https://git-scm.com/download/win](https://git-scm.com/download/win) for å installere Git.

### macOS
For å sjekke om Git er installert, kan du åpne et terminalvindu og kjøre følgende kommando:
```bash
git --version
```
Hvis Git er installert, vil du se versjonsnummeret. Hvis ikke, kan du følge instruksjonene på [https://git-scm.com/download/mac](https://git-scm.com/download/mac) for å installere Git.

## 2.4 Oppsett av Git-konfigurasjon
Vi skal  nå konfigurere Git med navn og e-postadresse. Dette er viktig fordi Git bruker denne informasjonen til å identifisere forfatteren av hver endring. Du kan bruke følgende kommandoer for å konfigurere Git:

Åpne **GIT Bash** og skriv inn følgende kommandoer:

```bash
git config --global user.name "Your Name"
```
```bash
git config --global user.email "youremail@example.com"
```

![Bilde av git config](pictures/git_bash_1.png)

For å se at konfigurasjonen er lagret, kan du kjøre følgende kommandoer:

```bash
git config --global user.name
```
```bash
git config --global user.email
```
Du bør nå se navnet og e-postadressen du har konfigurert.
![Bilde av git config](pictures/git_bash_2.png)





# 3. Lag et nytt repository
Nå som du har installert Git og konfigurert brukernavn og e-postadresse, er du klar til å opprette et nytt repository og begynne å spore endringer!

## 3.1 Logg inn på GitHub:

## 3.2 Opprett et nytt repository:
   - Klikk på **New**-knappen i øverste venstre hjørne.
   ![Bilde av opprett nytt repo](pictures/new_repo.png)
   - Gi repositoriet et navn, legg til en beskrivelse om du vil og velg om du vil gjøre repositoriet offentlig eller privat.
   ![Bilde av valg ved nytt repo](pictures/create_repo.png)
    Bruk gjerne privat hvis du ikke vil at andre skal kunne se koden din.
   - Klikk på **Create repository**.  

## 3.3 Kopier URL-en til repositoriet:
   - Klikk på den grønne **Code**-knappen.
   - Velg **HTTPS** og kopier URL-en som kommer opp.
    ![Bilde av code knapp](pictures/https.png)


## 3.4 Klon repositoriet til din maskin:
   - Åpne VS Code og velg **Clone repository**.
   - Skriv inn URL-en du kopierte fra GitHub og velg hvor du vil lagre repositoriet på din maskin.
   ![Bilde av URL](pictures/clone_ssh.png)




# 4. Grunnleggende konsepter
Nå er vi klare til å begynne å bruke Git! I denne delen vil vi dekke noen grunnleggende konsepter og kommandoer som du vil bruke når du arbeider med Git og GitHub.

- **Repository**: Et sted der prosjektfilene og -historikken er lagret.
- **Commit**: En snapshot av endringer i prosjektfilene dine.
- **Branch**: En gren av prosjektet som lar deg arbeide isolert med nye funksjoner eller endringer.
- **Merge**: Sammenføyning av endringer fra en gren til en annen.
- **Pull Request**: En forespørsel om å samle endringer fra en gren til en annen (spesielt på GitHub).
- **Fork**: En kopi av et repository som du eier og kan endre.

# 5. Jobb med prosjektet fra VS Code
Nå som du har klonet repositoriet til din maskin, kan du begynne å jobbe med prosjektet. Du kan åpne prosjektet i VS Code ved å velge **Open folder** og velge mappen du klonet repositoriet til.

## 5.1 Lag en README.md fil:
- I VS Code, trykk på **New File**-knappen i venstre hjørne.
- Skriv inn navnet **README.md** og trykk enter.
- Skriv inn en beskrivelse av prosjektet ditt i README.md filen.
![Bilde av ny fil](pictures/new_file.png)


## 5.2 Commit og push filen til GitHub:
   - Du skal nå se at det har kommet opp et varsel på **Source Control**-knappen i menyen på venstre side. Trykk på denne.
   - Hold musepekeren over **README.md** og trykk på **+** for å stage filen.
   - Skriv inn en commit message, f.eks "feat: added README" og trykk på **Commit** (se commit_message.md for tips til gode commit messages).
   - Trykk på de tre prikkene i venstre hjørne og velg **Push**.
   - Nå skal README.md filen din være på GitHub.
   ![Bilde av commit](pictures/commit.png)

   Du har nå lært hvordan du sender filer fra VS Code til GitHub. Du kan nå gjøre endringer i filene dine og committe og pushe endringene til GitHub.

# 6. Branching og merging
Nå som du har opprettet et repository og lagt til en README.md fil, kan du begynne å jobbe med prosjektet ditt. En god måte å organisere arbeidet ditt på er å bruke branches. En branch er en gren av prosjektet som lar deg arbeide isolert med nye funksjoner eller endringer. Når du er ferdig med endringene dine, kan du sammenføye dem med hovedgrenen ved å gjøre en merge.

## 6.1 Opprett en ny branch:
   - Klikk på **main**-knappen helt nede i venstre hjørne. Dette er navnet på hovedgrenen. Du blir nå tatt til søkefeltet hvor du får mulighet til å trykke på **Create new branch**. Skriv inn navnet **test_branch** på den nye grenen din. Du vil nå se at du har byttet til den nye grenen når du ser på navnet helt nede i venstre hjørne.
   - Du jobber nå i en ny gren av prosjektet ditt, men andre ord en kopi. Du kan gjøre endringer i prosjektet ditt og committe dem til den nye grenen.
   - Når du er ferdig med endringene dine, kan du sammenføye dem med hovedgrenen ved å gjøre en merge.
   ![Bilde av ny branch](pictures/new_branch.png)
  
## 6.2 Legge til en ny fil i den nye grenen din:
   - Lag en ny fil ved å trykke på **New File**-knappen i venstre hjørne.
   - Skriv inn navnet **new_file.txt** og trykk enter.
   - Skriv inn en en tilfeldig tekst i new_file.txt filen.
- Commit filen ved å trykke på **Source Control** i menyen til venstre, stage filen ved å trykke på **+** og commit filen ved å skrive inn en commit messageen **feat: added a new file** og trykke på **Commit & push**.
![Bilde av ny fil](pictures/new_file_in_new_branch.png)

## 6.3 Pull request:
   - Nå som du har gjort endringer i den nye grenen din, kan du gjøre en merge med hovedgrenen.
   - Gå inn på repoet ditt på GitHub. Du vil nå se en **Compare & pull request**-knapp. Trykk på denne.
- Du vil nå se en oversikt over endringene du har gjort i den nye grenen din. Trykk på **Create pull request**.
![Bilde av pull request](pictures/pull_request.png)
![Bilde av pull request](pictures/create_pull_request.png)

## 6.4 Godkjenne pull request:
- Du vil nå se en forespørsel om å sammenføye endringene i den nye grenen din med hovedgrenen. Trykk på **Merge pull request** og deretter **Confirm merge**.
![Bilde av merge pull request](pictures/merge.png)
- Du har nå gjort en merge av endringene i den nye grenen din med hovedgrenen. Du kan nå slette den nye grenen din ved å trykke på **Delete branch**.
![Bilde av delete branch](pictures/delete.png)
- Grenen du ga navnet **test_branch** er nå blitt slettet og du er tilbake til hovedgrenen.
- I VS Code kan du nå trykke på **Pull**-knappen for å hente endringene fra GitHub.
- Du vil forsatt være i **test_brach** i VScode selv om den er slettet fra ditt repo. Du kan nå trykke på **main**-knappen helt nede i venstre hjørne og velge **main** for å bytte til hovedgrenen. Eller lage en ny branch og bytte til denne.

# 7. Jobbe sammen med andre og merge conflicts
Når to personer gjør endringer i samme fil, eller når en person gjør endringer i en fil og en annen person sletter filen, kan det oppstå merge conflicts. Når dette skjer, må du løse konflikten manuelt.

Gå sammen to og to i grupper og gjør følgende:
## 7.1 Person A inviterer person B til å jobbe på prosjektet sitt:
- Person A går inn på repoet sitt på GitHub.
- Trykk på **Settings**.
- Trykk på **Collaboraters**.
- Skriv inn passordet ditt.
- Skriv inn brukernavnet til person B og trykk på **Add collaborater**.

## 7.2 Person B cloner repoet:
- Person B går inn på repoet til person A.
- Trykk på **Code**-knappen og kopier **HTTPS** URL-en.
- Åpne VS Code og velg **Clone repository**.
- Skriv inn URL-en du kopierte fra GitHub og velg hvor du vil lagre repositoriet på din maskin.

## 7.3 Person A gjør endringer i en fil:
- Person A og B skal nå ha samme repo på sine maskiner.
- Person A kan nå gjøre endringer i filen **New_file.txt** og committe & pushe endringene.
- For å unnvike merge conflicts, kan person B nå hente endringene fra GitHub ved å trykke på **Pull**-knappen under **Source Control** i VS Code, eller trykke på det lille synkroniseringshjulet nede i venstre hjørne ved siden av der branch navnet er.
- Person B skal nå å fått den nyeste versjonen av filen **New_file.txt**.

## 7.4 Person B gjør endringer i samme fil:
- Person B skal nå gjøre endringer i filen **New_file.txt** og committe & pushe endringene.
- Person A skal nå hente endringene fra GitHub ved å trykke på **Pull**-knappen under **Source Control**i VS Code, eller trykke på det lille synkroniseringshjulet nede i venstre hjørne ved siden av der branch navnet er.
- Person A skal nå å fått den nyeste versjonen av filen **New_file.txt**.

## 7.5 Merge conflicts:
**Vi skal se hva som skjer når person A og B gjør endringer i samme fil samtidig.**
- Person A skal nå gjøre endringer i filen **New_file.txt** og committe & pushe endringene.
- Person B skal også gjøre endringer i filen **New_file.txt** og committe & pushe endringene, han skal ikke pulle endringene fra GitHub før han har gjort dette.
- Dere vil nå få en **merge conflict** hvor dere må velge hvilke endringer dere vil beholde.




# 8. Merge conflicts med brancher
Merge conflict oppstår når endringer i en gren ikke kan sammenføyes med endringer i en annen gren. Dette kan skje når to personer gjør endringer i samme fil, eller når en person gjør endringer i en fil og en annen person sletter filen. Når dette skjer, må du løse konflikten manuelt.


Forsett i samme grupper som i forrige oppgave og gjør følgende:


## 8.1 Person A gjør endringer i en fil:
- Person A lager en ny branch med navnet **person_A** og passer på at han er på denne grenen.
- Person A skal nå gjøre endringer i filen **New_file.txt** og committe & pushe endringene.


## 8.2 Person B gjør endringer i samme fil:
- Person B skal nå lage en ny branch med navnet **person_B** og passe på at han er på denne grenen.
- Person B skal nå gjøre endringer i filen **New_file.txt** og committe & pushe endringene.

## 8.3 Pull request:
- Person A skal nå gjøre en pull request slik som i punkt 6.3 og merge endringene sine med hovedgrenen slik som i punkt 6.4. Dette skal gå fint.
- Person B skal nå gjøre en pull request som i punk 6.3 og merge endringene sine med hovedgrenen som i punk 6.4. Dette skal ikke gå fint. Person B vil nå få en merge conflict.
- Dere må nå manuelt løse konflikten.
- Når konflikten er løst, kan dere gjøre en merge av endringene i den nye grenen deres med hovedgrenen.
- Dere kan nå slette de nye grenene deres ved å trykke på **Delete branch**.
- Dere skal nå ha en ny versjon av filen **New_file.txt** som inneholder endringene som ble valgt i merge conflict.
- Dere kan nå gjøre en pull av endringene fra GitHub ved å trykke på **Pull**-knappen under **Source Control** i VS Code, eller trykke på det lille synkroniseringshjulet nede i venstre hjørne ved siden av der branch navnet er.



