# Python-programmering for Vg1 IT og medieproduksjon

Undervisningsopplegg i ti Jupyter notebooks til faget **konseptutvikling og programmering**.

Hver notebook inneholder teori, kjørbare eksempler og oppgaver. Til slutt i hver notebook finner du ekstraoppgaver delt inn i tre nivåer: 🟢 enkelt, 🟡 middels og 🔴 vanskelig.

| Nr. | Tema |
|---|---|
| 1 | Datatyper, print og aritmetiske operasjoner |
| 2 | Å lese feilmeldinger |
| 3 | Input-funksjonen og logiske operatorer |
| 4 | Løkker (for og while) |
| 5 | Funksjoner |
| 6 | Lister og arrays |
| 7 | Importering av bibliotek |
| 8 | Graftegning |
| 9 | Dictionaries |
| 10 | Classes (klasser) |
| 11 | Filbehandling |

Notebookene bygger på hverandre, så ta dem i rekkefølge.

---

# Kom i gang — steg for steg

Du skal gjøre to ting:

1. Installere programmet **JupyterLab Desktop**
2. Laste ned filene

Så er du i gang. Dette gjør du kun én gang.

---

## Del 1: Installere JupyterLab Desktop

JupyterLab Desktop er et vanlig program du installerer, akkurat som Word eller Spotify. Programmet har Python og alle bibliotekene du trenger innebygd, så du slipper å installere noe ekstra.

### Windows

Krever Windows 10 eller 11.

**Steg 1.** Last ned installasjonsfila ved å klikke her:

**[⬇️ Last ned JupyterLab Desktop for Windows](https://github.com/jupyterlab/jupyterlab-desktop/releases/latest/download/JupyterLab-Setup-Windows-x64.exe)**

**Steg 2.** Åpne fila som lastes ned.

**Steg 3.** Får du meldingen «Windows beskyttet PC-en din», velg **Mer informasjon → Kjør likevel**. Dette skjer fordi programmet er nytt for maskinen, ikke fordi noe er galt.

**Steg 4.** Følg installasjonsveiviseren. Trykk **Next** / **Install** hele veien.

> **Merk:** Underveis dukker det opp et installasjonsvindu til. Det er Python-miljøet som installeres. Bare la det gå ferdig — det tar noen minutter.

**Steg 5.** Når installasjonen er ferdig, finner du **JupyterLab** i Start-menyen.

### Mac

Krever macOS 12 eller nyere.

**Steg 1.** Først må du finne ut hvilken type Mac du har. Klikk på eplet øverst til venstre → **Om denne maskinen**.

- Står det **Apple M1, M2, M3** eller **M4**: bruk den første lenka under
- Står det **Intel**: bruk den andre lenka

**Steg 2.** Last ned:

**[⬇️ Last ned for Mac med Apple-brikke (M1–M4)](https://github.com/jupyterlab/jupyterlab-desktop/releases/latest/download/JupyterLab-Setup-macOS-arm64.dmg)**

**[⬇️ Last ned for Mac med Intel-brikke](https://github.com/jupyterlab/jupyterlab-desktop/releases/latest/download/JupyterLab-Setup-macOS-x64.dmg)**

**Steg 3.** Åpne `.dmg`-fila som lastes ned, og dra JupyterLab-ikonet inn i Programmer-mappa.

**Steg 4.** Åpne Programmer-mappa, **høyreklikk** på JupyterLab og velg **Åpne**. Bekreft at du vil åpne den.

> Dette må gjøres med høyreklikk første gang. Dobbeltklikker du vanlig, kan macOS nekte å åpne programmet fordi utvikleren er ukjent.

---

## Del 2: Hent notebookene

Notebookene henter du via GitHub, og du leverer inn svarene dine samme vei.

👉 **Følg [GitHub-veiledningen](GitHub_veiledning.md).** Den tar deg gjennom alt fra bunnen: konto, fork, GitHub Desktop og innlevering. Du trenger ikke ha brukt GitHub før.

Kort oppsummert gjør du dette én gang:

1. Lag en GitHub-konto
2. Lag din egen kopi av lærerens repo (**fork**)
3. Installer GitHub Desktop
4. Hent kopien ned på maskinen din (**clone**)

Etterpå er rutinen: jobb i JupyterLab → lagre → commit → push.

> ⚠️ **Ikke bruk Download ZIP.** Laster du ned notebookene som ZIP, får du en mappe uten kobling til GitHub — og da blir arbeidet ditt aldri levert.

---

## Del 3: Åpne notebookene

**Steg 1.** Åpne mappa du klonet ned i del 2.

**Steg 2.** Dobbeltklikk på `Notebook_1_Datatyper_print_aritmetikk.ipynb`.

JupyterLab Desktop åpner seg med notebooken klar til bruk. Det er alt.

> Skjer det ingenting når du dobbeltklikker, kan Windows ha koblet `.ipynb`-filer til et annet program. Da åpner du JupyterLab fra Start-menyen først, og velger deretter **File → Open Folder** og finner mappa di.

---

> 📌 **Notebook 2 handler om feilmeldinger,** og der er flere celler laget for å gi feilmelding med vilje. Det er meningen — poenget er å lære å lese dem.

## Del 4: Slik jobber du i en notebook

- **Kjør en celle:** klikk i cella og trykk `Shift + Enter`
- Cellene med grå bakgrunn er kode. Du kan endre på dem og kjøre dem på nytt så mye du vil
- Oppgavene har tomme kodeceller under seg. Der skriver du svaret ditt
- **Lagre:** `Ctrl + S` (Windows) eller `Cmd + S` (Mac). Gjør dette ofte
- **Får du feilmelding?** Les den nederste linja først. Den forteller som regel hva som er galt og hvilken linje det gjelder

Til venstre har du et filpanel der du ser alle notebookene og kan bytte mellom dem.

> 💡 Synes du det blir mye på skjermen? Velg **View → Simple Interface**. Da vises ett dokument om gangen, og det blir roligere å jobbe i.

Eksperimenter gjerne med eksemplene. Å endre på kode som virker, og se hva som skjer, er en av de beste måtene å lære programmering på.

---

## Del 5: Avslutte

**Steg 1.** Lagre notebooken (`Ctrl + S`).

**Steg 2.** Lukk programmet som et hvilket som helst annet program.

**Steg 3.** Åpne GitHub Desktop, skriv en kort beskrivelse, og trykk **Commit** og deretter **Push origin**.

> ⚠️ Uten push er arbeidet ditt ikke levert. Gjør dette til en vane på slutten av hver time — det tar under ett minutt.

Neste gang dobbeltklikker du bare på notebook-fila igjen.

---

## Feilsøking

**Programmet vil ikke åpne seg på Mac**

Høyreklikk på JupyterLab i Programmer-mappa og velg **Åpne** i stedet for å dobbeltklikke. Bekreft at du vil åpne den. Dette trengs kun første gang.

**Windows blokkerer installasjonsfila**

Velg **Mer informasjon → Kjør likevel** i advarselsvinduet.

**Ingenting skjer når jeg dobbeltklikker på en .ipynb-fil**

Åpne JupyterLab fra Start-menyen, og bruk **File → Open Folder** til å finne mappa med notebookene.

**Cella ser ut til å kjøre for alltid (`[*]`)**

Koden har havnet i en evig løkke, eller den venter på at du skriver noe i et `input()`-felt. Se etter et tekstfelt i cella. Ellers: velg **Kernel → Interrupt Kernel** for å stoppe.

**ModuleNotFoundError: No module named 'numpy'**

Dette skal ikke skje, siden bibliotekene følger med programmet. Får du det likevel, sjekk øverst til høyre at det står et kjernenavn (f.eks. `Python 3`). Står det «No Kernel», klikk der og velg Python-kjernen.

**Jeg mistet arbeidet mitt**

Notebooken lagrer ikke automatisk. Trykk `Ctrl + S` jevnlig. JupyterLab lager også sikkerhetskopier — se **File → Revert Notebook to Checkpoint**.

---

# Til senere: VS Code

Vi bruker JupyterLab nå, men på et tidspunkt går vi over til VS Code. Da må Python installeres separat, fordi VS Code ikke kan bruke Python-miljøet som ligger inne i JupyterLab Desktop.

## Steg 1: Installere Python

**Windows**

1. Gå til **https://www.python.org/downloads/**
2. Trykk på den gule **«Download Python»**-knappen
3. Åpne fila som lastes ned

> ⚠️ **Huk av for «Add python.exe to PATH» nederst i vinduet FØR du trykker videre.** Denne avkrysningsboksen er lett å overse, og glemmer du den, må du avinstallere og begynne på nytt.

4. Trykk **«Install Now»** og vent til det er ferdig
5. Sjekk at det virket: trykk `Windows-tasten`, skriv `cmd`, trykk Enter, skriv `python --version` og trykk Enter. Får du opp et versjonsnummer, er du i mål

**Mac**

1. Gå til **https://www.python.org/downloads/**
2. Trykk på den gule **«Download Python»**-knappen
3. Åpne `.pkg`-fila og følg veiviseren
4. Sjekk at det virket: åpne Terminal, skriv `python3 --version` og trykk Enter

## Steg 2: Installere bibliotekene

Åpne Ledetekst (Windows) eller Terminal (Mac) og skriv:

Windows:
```
pip install numpy matplotlib
```

Mac:
```
pip3 install numpy matplotlib
```

Trykk Enter og vent til det er ferdig.

## Steg 3: Installere VS Code

1. Gå til **https://code.visualstudio.com/** og trykk på nedlastingsknappen
2. Kjør installasjonsfila og følg veiviseren
3. På Windows: huk gjerne av for **«Add to PATH»** og **«Open with Code»**
4. Start VS Code

## Steg 4: Installere utvidelsene

1. Klikk på ikonet med fire firkanter i venstremenyen (Extensions)
2. Søk opp og installer **Python** (utgitt av Microsoft)
3. Søk opp og installer **Jupyter** (utgitt av Microsoft)

## Steg 5: Åpne notebookene

1. Velg **File → Open Folder** og åpne mappa med notebookene
2. Klikk på en `.ipynb`-fil i sidepanelet
3. Øverst til høyre står det **«Select Kernel»**. Klikk der, velg **Python Environments**, og velg Python-versjonen du installerte i steg 1
4. Blir du spurt om å installere `ipykernel`, trykk **Install**

Nå kjører du cellene med `Shift + Enter`, akkurat som før.

---

### Om oppbyggingen

Hver notebook følger samme struktur: læringsmål → teori → gjennomgåtte eksempler → øvingsoppgaver med tomme kodeceller → differensierte ekstraoppgaver → oppsummering.

Eksemplene er forankret i IT- og mediefaglige situasjoner — filstørrelser, passord, besøksstatistikk, spillerdata — framfor abstrakte matematikkoppgaver.

All eksempelkode er testet og kjører feilfritt.

### Notebook 11 lager filer

Notebook 11 oppretter tekst- og CSV-filer i arbeidsmappa som en del av undervisningen (`dagbok.txt`, `spillere.csv` med flere). Det er meningen, og `.gitignore` sørger for at de ikke havner i repoet.

---

## Innhold i mappa

```
Notebook_1 ... Notebook_11.ipynb   Undervisningsopplegget
README.md                          Denne fila
GitHub_veiledning.md               Slik bruker du GitHub og leverer inn
.gitignore                         Utelater midlertidige filer fra repoet
```
