# GitHub-veiledning

**Konseptutvikling og programmering, Vg1 IT og medieproduksjon**

Denne guiden viser deg hvordan du henter notebookene fra GitHub, jobber med dem på din egen maskin, og leverer inn svarene dine.

Du har aldri brukt GitHub før? Helt fint. Vi tar det fra bunnen.

---

## Innhold

1. [Hva er Git og GitHub?](#del-1-hva-er-git-og-github)
2. [Lag en GitHub-konto](#del-2-lag-en-github-konto)
3. [Lag din egen kopi av notebookene (fork)](#del-3-lag-din-egen-kopi-fork)
4. [Installer GitHub Desktop](#del-4-installer-github-desktop)
5. [Hent kopien ned på maskinen din (clone)](#del-5-hent-kopien-ned-på-maskinen-din-clone)
6. [Jobb med oppgavene](#del-6-jobb-med-oppgavene)
7. [Lever inn (commit og push)](#del-7-lever-inn-commit-og-push)
8. [Den daglige rutinen](#del-8-den-daglige-rutinen)
9. [Feilsøking](#feilsøking)
10. [Ordliste](#ordliste)

---

# Del 1: Hva er Git og GitHub?

## Problemet Git løser

Du kjenner sikkert dette fra før:

```
oppgave.docx
oppgave_ny.docx
oppgave_ny_FERDIG.docx
oppgave_ny_FERDIG_v2_denne_gangen_ordentlig.docx
```

Det fungerer sånn passe. Du husker ikke hva som var forskjellen, du tør ikke slette noe, og finner du ut at versjon 2 var best, er den kanskje overskrevet.

**Git** løser dette. I stedet for å lage nye filer, tar Git *øyeblikksbilder* av mappa di når du ber om det. Alle øyeblikksbildene lagres, du kan gå tilbake til et hvilket som helst av dem, og du ser nøyaktig hva som ble endret mellom hvert av dem.

## Git og GitHub er to forskjellige ting

Dette forvirrer mange i starten, så her er skillet:

| | Hva det er | Hvor det er |
|---|---|---|
| **Git** | Programmet som tar øyeblikksbilder | På din maskin |
| **GitHub** | Nettstedet som lagrer øyeblikksbildene i skyen | På internett |

Tenk på det som OneDrive: filene ligger både på maskinen din **og** i skyen, men de synkroniseres ikke automatisk. Du bestemmer selv når du vil sende noe opp.

## De fem ordene du trenger

Du kommer til å møte disse fem ordene. Lær dem nå, så blir resten enklere:

**Repository** (eller bare **repo**) — en mappe som Git holder styr på. Læreren din har et repo med notebookene.

**Fork** — å lage din egen kopi av noen andres repo på GitHub. Kopien er *din*, og det du gjør med den påvirker ikke originalen.

**Clone** — å hente et repo fra GitHub ned på maskinen din, så du kan jobbe med filene.

**Commit** — å ta et øyeblikksbilde av arbeidet ditt. Dette skjer **bare på din maskin**.

**Push** — å sende øyeblikksbildene dine opp til GitHub. **Det er her innleveringen faktisk skjer.**

## Slik henger det sammen

```
   Lærerens repo på GitHub
            |
            |  1. FORK  (én gang)
            v
     Ditt repo på GitHub  <---------------+
            |                             |
            |  2. CLONE  (én gang)        |  4. PUSH  (hver gang du er ferdig)
            v                             |
     Mappa på din maskin  ----------------+
            |                             ^
            |  3. Du jobber i JupyterLab  |
            +-----------------------------+
                     COMMIT
```

**Det viktigste å forstå:** en commit sender ingenting noe sted. Den lagrer bare lokalt. Det er **push** som gjør at læreren kan se arbeidet ditt.

Glemmer du å pushe, har du ikke levert.

---

# Del 2: Lag en GitHub-konto

**Steg 1.** Gå til **https://github.com/signup**

**Steg 2.** Skriv inn e-postadressen din. Bruk gjerne skole-e-posten.

**Steg 3.** Lag et passord. Bruk noe du husker — du skal logge inn flere ganger.

**Steg 4.** Velg et brukernavn.

> 💡 **Tenk deg litt om her.** Brukernavnet er offentlig, og det kan stå på CV-en din om noen år. `ola.nordmann` eller `olanordmann02` er fine. `xX_pro_gamer_Xx` er kanskje mindre fint i en jobbsøknad.

**Steg 5.** Fyll ut fødselsdatoen din. Du må være minst 13 år for å ha en GitHub-konto.

**Steg 6.** Løs oppgaven som sjekker at du ikke er en robot.

**Steg 7.** GitHub sender deg en kode på e-post. Åpne e-posten, kopier koden, og lim den inn.

**Steg 8.** Får du spørsmål om abonnement, velg **gratisversjonen** (Free). Den har alt du trenger.

✅ Du har nå en GitHub-konto.

---

# Del 3: Lag din egen kopi (fork)

Læreren sitt repo er felles for hele klassen — du kan ikke skrive i det. Derfor lager du din egen kopi.

**Steg 1.** Gå til lærerens repo. Læreren gir deg adressen, og den ser omtrent slik ut:

```
https://github.com/laerernavn/programmering-vg1
```

**Steg 2.** Sjekk at du er logget inn. Ser du profilbildet ditt øverst til høyre, er du det.

**Steg 3.** Finn knappen **Fork** øverst til høyre på siden.

**Steg 4.** Trykk på den. Du får opp et skjema.

**Steg 5.** La alt stå som det er, og trykk **Create fork**.

**Steg 6.** Vent noen sekunder. Siden laster på nytt, og nå står **ditt eget brukernavn** øverst i stedet for lærerens:

```
ditt-brukernavn / programmering-vg1
     forked from laerernavn/programmering-vg1
```

✅ Du har nå din egen kopi på GitHub. Det du gjør med den, påvirker ikke lærerens original.

> 📌 **Merk:** Kopien din er offentlig — hvem som helst kan se den. Ikke legg personlige opplysninger i notebookene.

---

# Del 4: Installer GitHub Desktop

Git kan styres med kommandoer i et svart vindu, men det er unødvendig tungvint i starten. Vi bruker **GitHub Desktop**, som er et vanlig program med knapper.

**Steg 1.** Gå til **https://desktop.github.com/**

**Steg 2.** Trykk på nedlastingsknappen. Nettsiden velger riktig versjon for maskinen din automatisk.

**Steg 3.** Kjør installasjonsfila.

> På Mac må du dra programmet inn i Programmer-mappa, som med JupyterLab.

**Steg 4.** Start GitHub Desktop.

**Steg 5.** Trykk **Sign in to GitHub.com**. Nettleseren åpner seg.

**Steg 6.** Logg inn med GitHub-kontoen din, og bekreft at GitHub Desktop får tilgang.

**Steg 7.** Du blir sendt tilbake til programmet. Blir du spurt om navn og e-post, fyll inn ditt eget — dette blir stemplet på øyeblikksbildene dine.

✅ GitHub Desktop er klart.

---

# Del 5: Hent kopien ned på maskinen din (clone)

Nå skal kopien din fra GitHub ned på maskinen, så du kan jobbe med filene.

**Steg 1.** I GitHub Desktop, velg **File → Clone repository**.

**Steg 2.** Velg fanen **GitHub.com**. Du ser en liste over repoene dine — der ligger `programmering-vg1`.

**Steg 3.** Klikk på det.

**Steg 4.** Under **Local path** velger du hvor mappa skal ligge på maskinen din.

> 💡 **Tips:** velg en plassering du husker, for eksempel i OneDrive-mappa di. Da blir arbeidet ditt også sikkerhetskopiert.

**Steg 5.** Trykk **Clone** og vent noen sekunder.

✅ Mappa ligger nå på maskinen din, med alle notebookene i.

> ⚠️ **Viktig:** Fra nå av jobber du **kun i denne mappa.** Har du lastet ned notebookene som ZIP tidligere, ikke bruk den mappa lenger — arbeid der blir aldri levert. Slett den gjerne, så du ikke forveksler dem.

---

# Del 6: Jobb med oppgavene

Dette er som før — GitHub endrer ingenting på hvordan du programmerer.

**Steg 1.** Åpne mappa du klonet.

**Steg 2.** Dobbeltklikk på notebooken du skal jobbe med. JupyterLab åpner seg.

**Steg 3.** Løs oppgavene.

**Steg 4.** **Lagre med `Ctrl + S`** (eller `Cmd + S` på Mac).

> ⚠️ **Dette steget er avgjørende.** GitHub Desktop ser bare det som faktisk er lagret på disken. Glemmer du å lagre i JupyterLab, tror GitHub Desktop at ingenting er endret — og du får ikke levert noe.
>
> Regel: **lagre alltid i JupyterLab før du går til GitHub Desktop.**

---

# Del 7: Lever inn (commit og push)

Nå skal arbeidet ditt opp til GitHub. Dette er to steg: først commit, så push.

**Steg 1.** Åpne GitHub Desktop.

**Steg 2.** I venstre kolonne ser du alle filene du har endret. Har du jobbet i notebook 3, står `Notebook_3_Input_logiske_operatorer.ipynb` der.

> Ser du ingenting? Da har du enten ikke lagret i JupyterLab, eller du har jobbet i feil mappe. Se [Feilsøking](#feilsøking).

**Steg 3.** Nederst til venstre er det et lite tekstfelt der det står **Summary**. Skriv en kort beskrivelse av hva du har gjort:

```
Ferdig med oppgavene i notebook 3
```

> 💡 **Skriv noe meningsfylt.** «oppdatering» og «asdf» hjelper ingen — heller ikke deg selv om tre uker når du leter etter noe. Beskriv hva du gjorde: *«Løste oppgave 3.4.1 og 3.4.2»*.

**Steg 4.** Trykk den blå knappen **Commit to main**.

✅ Øyeblikksbildet er tatt — men det ligger fortsatt bare på din maskin.

**Steg 5.** Øverst dukker det opp en knapp: **Push origin**. Trykk på den.

✅ **Nå er arbeidet ditt levert.**

## Sjekk at det faktisk kom fram

Ikke bare tro det — sjekk.

**Steg 6.** Gå til `https://github.com/ditt-brukernavn/programmering-vg1` i nettleseren.

**Steg 7.** Du skal se commit-meldingen din ved siden av filene, og et tidspunkt som «now» eller «2 minutes ago».

**Steg 8.** Klikk på notebooken du jobbet med. GitHub viser innholdet direkte i nettleseren — og du skal se svarene dine der.

Ser du svarene dine på github.com, er innleveringen i orden.

---

# Del 8: Den daglige rutinen

Del 2 til 5 gjør du **kun én gang**. Etter det er rutinen slik:

```
1. Åpne mappa og jobb i JupyterLab
2. Ctrl + S            (lagre)
3. GitHub Desktop: skriv Summary, trykk Commit
4. Trykk Push origin
5. Sjekk github.com
```

**Gjør dette på slutten av hver time.** Det tar under ett minutt, og da ligger arbeidet ditt trygt i skyen selv om maskinen skulle krasje.

Du kan gjerne committe flere ganger i løpet av en time — hver gang du blir ferdig med en oppgave, for eksempel. Mange små commits er bedre enn én stor, fordi du lettere kan gå tilbake til et bestemt punkt.

## Hvis læreren oppdaterer notebookene

Legger læreren til en ny oppgave eller retter en feil, kommer ikke endringen automatisk til deg. Slik henter du den:

**Steg 1.** Gå til ditt repo på github.com.

**Steg 2.** Står det **«This branch is X commits behind»**, trykk **Sync fork → Update branch**.

**Steg 3.** Åpne GitHub Desktop og trykk **Pull origin** for å hente endringen ned på maskinen din.

> 💡 Push alltid ditt eget arbeid **før** du henter oppdateringer. Da unngår du at endringene kolliderer.

---

# Feilsøking

**GitHub Desktop viser ingen endringer, selv om jeg har jobbet**

Tre mulige årsaker, i rekkefølgen du bør sjekke dem:

1. Du glemte å lagre i JupyterLab. Gå tilbake og trykk `Ctrl + S`.
2. Du jobber i feil mappe — sannsynligvis en gammel ZIP-nedlasting. Sjekk at stien i JupyterLab stemmer med der du klonet repoet.
3. Feil repo er valgt øverst til venstre i GitHub Desktop.

**Jeg trykket Commit, men læreren ser ingenting**

Du har ikke pushet. Commit lagrer bare lokalt. Se etter **Push origin**-knappen øverst i GitHub Desktop og trykk på den.

**Push origin-knappen er borte**

Da er alt allerede pushet. Sjekk på github.com for å være sikker.

**«Authentication failed» når jeg prøver å pushe**

Du er logget ut. I GitHub Desktop: **File → Options → Accounts**, og logg inn på nytt.

**Jeg får noe som heter «merge conflict»**

Dette skjer hvis samme fil er endret to steder samtidig — for eksempel om du har jobbet på to ulike maskiner. Spør læreren din. Ikke prøv å fikse det på egen hånd første gangen; notebook-filer er vanskelige å rydde opp i manuelt.

**Forebygging:** push alltid før du forlater en maskin, og pull alltid før du begynner å jobbe på en annen.

**Jeg slettet noe ved et uhell**

Har du committet tidligere, er ingenting tapt. I GitHub Desktop, velg fanen **History**, finn en tidligere commit, høyreklikk og velg **Revert changes in commit**.

Dette er selve poenget med Git: det er vanskelig å miste noe permanent, så lenge du committer jevnlig.

---

# Ordliste

| Ord | Betydning |
|---|---|
| **Repository / repo** | En mappe som Git holder styr på |
| **Fork** | Din egen kopi av noen andres repo på GitHub |
| **Clone** | Å hente et repo fra GitHub ned på maskinen din |
| **Commit** | Et øyeblikksbilde av arbeidet ditt, lagret lokalt |
| **Push** | Å sende commits opp til GitHub |
| **Pull** | Å hente ned endringer fra GitHub |
| **Branch** | En egen «gren» å jobbe i. Vi bruker bare `main` |
| **main** | Hovedgrenen — den eneste du trenger å forholde deg til |
| **origin** | Kallenavnet på ditt repo på GitHub |
| **Merge conflict** | Samme fil er endret to steder, og Git vet ikke hva som gjelder |

---

# For lærer

## Oppsett

Legg notebookene i et **offentlig** repo. Elevene forker det, og forken må være offentlig for at de skal slippe å betale for noe.

## Slik finner du alle besvarelsene

Gå til ditt repo → **Insights** → **Forks**. Der ligger samtlige elevforker i én liste, med lenke til hver enkelt. Det er så nær et innleveringspanel du kommer uten ekstra verktøy.

Du kan også se hvem som har levert når: klikk deg inn på en fork og velg **Commits** for å se hele historikken med tidsstempler.

## Om GitHub Classroom

GitHub Classroom var laget for akkurat dette, men tjenesten ble **pensjonert 28. august 2026** og tar ikke lenger imot nye brukere. Fork-metoden over er derfor veien å gå.

## Vurdering av arbeidet

Commit-historikken er faktisk et pedagogisk verktøy i seg selv. Du kan se:

- **Når** eleven jobbet, og om arbeidet er spredt over tid eller gjort natta før fristen
- **Hvordan** en løsning vokste fram, gjennom flere commits
- **Om** eleven faktisk har prøvd seg fram, eller limt inn noe ferdig

Du kan kommentere direkte på en linje i en fil på GitHub, som gir presis tilbakemelding.

## Personvern

Elevforkene er offentlige. Det betyr at besvarelsene er synlige for alle, og at elevene kan se hverandres arbeid. Vurder om det er greit for ditt formål.

**Vil du ha private besvarelser** i stedet, er alternativet at hver elev lager et eget privat repo og legger deg til som **collaborator**. Da mister du oversikten i Forks-lista og må ta imot én invitasjon per elev, men arbeidet blir privat.

Uansett: minn elevene på at alt de pusher til et offentlig repo, er offentlig. Ingen personopplysninger i notebookene.
