# Guide Git og GitHub

## Installer Git og konfigurere GitHub på din maskin
Hopp over dette dersom du allerede har installert Git, laget Github konto og konfigurert GitHub på din maskin
1. Gå til [https://git-scm.com/](https://git-scm.com/)
2. Installer Git
3. Gå til [https://github.com/](https://github.com/)
4. Lag konto på GitHub
5. Åpne din foretrukne terminal
6. Skriv ``` git config --global user.name "ditt navn" ``` i terminalen
7. Skriv ``` git config --global user.email "din_email@hotmail.com" ``` i terminalen
8. Skriv ``` git config --global user.name ```  for å verifisere at du har riktig brukernavn
9. Skriv ``` git config --global user.email ``` for å verifisere at du har riktig epost adresse

## Lage repo og pushe kode til GitHub
1. På [https://git-scm.com/](https://git-scm.com/) mens du er pålogget trykk på new new
2. Gi prosjektet et navn
3. Trykke på create repository knappen helt nederst
4. I vs code lag et nytt prosjekt med en boilerplate HTML fil, legg til det du ønsker av HTML
5. Sørg for at du er på riktig sti i terminalen, du skal være i prosjektet. Du bruker cd for å navigere i deg i terminalen, eventuelt åpne riktig mappe manuelt.
6. I terminalen skriver du git init for å initialisere lokalt repo
7. Gå til prosjektet du lagde i GitHub og kopier linjen som ligner på ``` git remote add origin https://github.com/mobak88/test.git ``` for å legge til ditt eksterne repo, lim dette inn i terminalen din
8. Lim inn ``` git branch -M main ``` i terminalen for å bytte navn på din hovedgren fra master til main
9. Skriv ``` git add index.html ``` i terminalen for å legge til index.html
10. Skriv ``` git commit -m "Din melding" ``` for å comitte filen
11. Skriv ``` git push -u origin main ``` for å pushe koden din til GitHub
12. Last inn GitHub siden på nytt så ser du at index.html ligger der og du kan trykke på den for å se koden

## Mest brukte GitHub komandoer

Initialiserer et nytt lokalt Git-repository i mappen du står i.
``` git push -u origin main ``` 

Legger til alle endrede og nye filer til staging-området, klare for commit.
``` git add . ```

Lager en commit av filene i staging-området med en beskrivende melding.
``` git commit -m "Din commit-melding" ```

Legger til et eksternt repository
```git remote add origin https://github.com/brukernavn/repository.git ```

Sender endringene til den eksterne grenen
``` git push ```

Henter endringer fra det eksterne repositoryet og slår dem sammen med din lokale branch.
 ```git pull origin main ```

Se status for filer i Git. Viser endringer, nye filer og hvilke filer som er klare for commit.
``` git status ```

Se commit-historikk. Viser en liste over tidligere commits i din nåværende branch.
``` git log ```

Lager en ny gren og bytter til den.
 ```git checkout -b ny-branch ```

Klon et eksternt repository. Laster ned en kopi av et eksternt Git-repository til din lokale maskin.
``` git clone https://github.com/brukernavn/repository.git ```

Sjekke ut en eksisterende gren. Bytter til en eksisterende branch i prosjektet ditt.
 ```git checkout branch-navn ```
