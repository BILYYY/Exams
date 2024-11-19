

## **Eksamen 1**

### **Flervalgsoppgaver**

1. **Hvilken av følgende er IKKE en funksjon til et operativsystem?**
   - **Riktig svar:** C) Applikasjonsutvikling
   - **Forklaring:** Operativsystemer administrerer maskinvare, prosesser og filer, men de utvikler ikke applikasjoner.

2. **I en mikrokjerne-arkitektur, hvilke komponenter kjøres typisk i brukermodus?**
   - **Riktig svar:** D) Alle de ovennevnte
   - **Forklaring:** En mikrokjerne kjører enhetsdrivere, minnehåndtering og filsystemer i brukermodus for bedre sikkerhet og fleksibilitet.

3. **Hva er formålet med et systemkall i et operativsystem?**
   - **Riktig svar:** B) Å la brukerprogrammer be om tjenester fra kjernen
   - **Forklaring:** Systemkall gjør det mulig for programmer å be operativsystemet utføre oppgaver som filhåndtering og prosesskontroll.

4. **Hvilken av følgende planleggingsalgoritmer er ikke-preemptiv?**
   - **Riktig svar:** B) First-Come, First-Served (FCFS)
   - **Forklaring:** FCFS lar prosesser kjøre til de er ferdige uten å bli avbrutt.

5. **Hva står TLB for i minnehåndtering?**
   - **Riktig svar:** B) Translation Lookaside Buffer
   - **Forklaring:** TLB er en hurtig cache som hjelper til med å oversette virtuelle adresser til fysiske adresser raskere.

### **Essayoppgaver**

1. **Forklar forskjellene mellom prosesser og tråder. Hvorfor er denne distinksjonen viktig i operativsystemer?** (10 poeng)

   **Svar:**
   - **Prosesser:**
     - Tenk på en prosess som en selvstendig jobb, som å lage en kopp kaffe. Den har sine egne ingredienser og verktøy.
     - Hver prosess har sitt eget minneområde, som separate kjøkken for hver jobb.
   - **Tråder:**
     - En tråd er som en delt arbeidsstasjon i samme kjøkken hvor flere kokker kan jobbe samtidig.
     - Tråder deler minne og ressurser med hverandre, noe som gjør kommunikasjonen raskere og enklere.
   - **Viktighet:** Å forstå forskjellen hjelper operativsystemet med å effektivt håndtere flere oppgaver samtidig uten at de forstyrrer hverandre.

2. **Beskriv hvordan paging fungerer i minnehåndtering og diskuter hvordan det hjelper med å implementere virtuelt minne.** (10 poeng)

   **Svar:**
   - **Paging:** Tenk på paging som å dele et stort bibliotek inn i mindre seksjoner (sider). Hver seksjon kan lagres hvor som helst i biblioteket.
   - **Virtuelt minne:** Det er som å ha et ekstra rom til lagring. Hvis et bibliotek har for mange bøker (programmer) for det fysiske rommet, kan noen bøker flyttes til det ekstra rommet og hentes tilbake når de trengs.
   - **Fordeler:** Dette gjør at systemet kan kjøre flere programmer samtidig uten å gå tom for plass.

3. **Hva er de fire nødvendige betingelsene for at en deadlock skal oppstå? Gi eksempler for hver betingelse.** (8 poeng)

   **Svar:**
   1. **Gjensidig utelukkelse:** Tenk på en printer som kun kan brukes av én person av gangen.
   2. **Hold og vent:** En person holder en kopi av et dokument og venter på en tom skriver.
   3. **Ingen forhåndsfrigiing:** Printeren kan ikke tvinges til å gi opp dokumentet før jobben er fullført.
   4. **Sirkulær venting:** To personer venter på hverandre for å få tilgang til skriveren og dokumentet samtidig.

4. **Diskuter rollen til filsystemet i et operativsystem. Forklar ulike filallokeringsmetoder og deres fordeler og ulemper.** (12 poeng)

   **Svar:**
   - **Rolle:** Filsystemet er som et bibliotekssystem som organiserer og lagrer filer på datamaskinen.
   - **Filallokeringsmetoder:**
     1. **Kontinuerlig allokering:**
        - **Fordeler:** Rask tilgang til filer, enkelt å finne filer.
        - **Ulemper:** Kan føre til fragmentering, vanskelig å utvide filer.
     2. **Koblet allokering:**
        - **Fordeler:** Enkelt å legge til mer data, ingen fragmentering.
        - **Ulemper:** Trekkes oppover raskt, vanskelig å finne filer raskt.
     3. **Indeksert allokering:**
        - **Fordeler:** Rask tilgang både sekvensielt og tilfeldig.
        - **Ulemper:** Krever ekstra plass for indekser, kan bli tungt for store filer.

---

## **Eksamen 2**

### **Flervalgsoppgaver**

1. **Hvilken av følgende beskriver best en race condition?**
   - **Riktig svar:** B) En situasjon hvor to prosesser får samtidig tilgang til delt data, noe som fører til feil resultater
   - **Forklaring:** Race conditions skjer når prosesser konkurrerer om tilgang til delte ressurser uten riktig synkronisering.

2. **Hva er hovedfordelen med å bruke tråder over flere prosesser?**
   - **Riktig svar:** C) Tråder deler samme adresserom, noe som gir raskere kommunikasjon
   - **Forklaring:** Tråder kan dele data enkelt fordi de deler minne, noe som gjør kommunikasjonen raskere enn mellom separate prosesser.

3. **I konteksten av filsystemer, hva er en inode?**
   - **Riktig svar:** B) En datastruktur som lagrer informasjon om en fil
   - **Forklaring:** Inoder inneholder metadata som eierskap, tillatelser og plassering av data på disken.

4. **Hvilken av følgende er en teknikk for å unngå thrashing i virtuelle minnesystemer?**
   - **Riktig svar:** B) Implementere en arbeidssettmodell
   - **Forklaring:** En arbeidssettmodell holder styr på hvilke sider en prosess bruker ofte, og begrenser antallet sider i minnet for å unngå for mye paging.

5. **Hva er hovedformålet med en enhetsdriver i et operativsystem?**
   - **Riktig svar:** B) Å gi et grensesnitt mellom maskinvareenheter og OS
   - **Forklaring:** Enhetsdrivere gjør det mulig for operativsystemet å kommunisere med maskinvareenheter som skrivere og disker.

### **Essayoppgaver**

1. **Beskriv prosessens tilstandsdiagram og forklar overgangen mellom de forskjellige tilstandene til en prosess.** (10 poeng)

   **Svar:**
   - **Tilstander:**
     - **Ny:** Prosessen blir opprettet.
     - **Klar:** Prosessen er klar til å kjøre.
     - **Kjører:** Prosessen utfører instruksjoner.
     - **Venter:** Prosessen venter på en hendelse eller ressurs.
     - **Terminert:** Prosessen er ferdig.
   - **Overganger:**
     - **Ny → Klar:** Når prosessen er opprettet.
     - **Klar → Kjører:** Når prosessen får CPU-tildeling.
     - **Kjører → Venter:** Når prosessen trenger å vente på noe, som I/O.
     - **Venter → Klar:** Når ventingen er ferdig.
     - **Kjører → Terminert:** Når prosessen er ferdig.

2. **Forklar konseptet med virtuelt minne. Hvordan forbedrer det systemets ytelse og ressursutnyttelse?** (10 poeng)

   **Svar:**
   - **Virtuelt minne:** Bruker diskplass som ekstra minne, slik at prosesser kan bruke mer minne enn det fysiske RAM tilgjengelig.
   - **Forbedrer ytelse:**
     - **Økt minnekapasitet:** Flere prosesser kan kjøre samtidig.
     - **Effektiv bruk av RAM:** Bare nødvendige deler av en prosess lastes inn i minnet.
     - **Isolasjon:** Hver prosess har sitt eget adresseområde, som øker sikkerheten.

3. **Diskuter de forskjellige mekanismene for interprosesskommunikasjon (IPC) tilgjengelig i operativsystemer. Gi eksempler hvor hver ville være passende.** (8 poeng)

   **Svar:**
   - **Pipes:** Enkel kommunikasjon mellom to prosesser. *Eksempel:* En kommando som `ls | grep "txt"`.
   - **Delte minneområder:** Rask datautveksling mellom flere prosesser. *Eksempel:* To prosesser som jobber med store data sett.
   - **Meldingskøer:** Strukturerte meldinger mellom prosesser. *Eksempel:* En klient-server-applikasjon.
   - **Sockets:** Kommunikasjon over nettverk. *Eksempel:* Webserver og nettleser som kommuniserer via HTTP.

4. **Hva er forskjellene mellom SSD-er og HDD-er? Diskuter deres innvirkning på operativsystemdesign og ytelse.** (12 poeng)

   **Svar:**
   - **Teknologi:**
     - **HDD-er:** Bruker magnetiske plater og bevegelige hoder.
     - **SSD-er:** Bruker flashminne uten bevegelige deler.
   - **Ytelse:**
     - **HDD-er:** Lavere hastigheter på grunn av mekaniske deler.
     - **SSD-er:** Raskere lese- og skrivehastigheter.
   - **Innvirkning på OS:**
     - **HDD-er:** Krever optimalisering for sekvensiell tilgang.
     - **SSD-er:** Kan dra nytte av raskere tilfeldig tilgang og trenger mindre buffering.
   - **Fordeler og ulemper:**
     - **HDD-er:** Billigere per GB, men tregere og mer utsatt for skader.
     - **SSD-er:** Raskere og mer pålitelige, men dyrere per GB.

---

## **Eksamen 3**

### **Flervalgsoppgaver**

1. **Hvilken av følgende er IKKE en type planlegger i et operativsystem?**
   - **Riktig svar:** D) Nettverksplanlegger
   - **Forklaring:** Vanlige planleggere er langtids-, middelsiktig- og korttidsplanlegger. Nettverksplanlegger er ikke en standard type.

2. **Hva refererer 'heisalgoritmen' til i operativsystemer?**
   - **Riktig svar:** B) Diskplanlegging
   - **Forklaring:** Heisalgoritmen brukes for å organisere diskoperasjoner for å redusere søketid.

3. **I Linux, hva er formålet med 'init'-prosessen?**
   - **Riktig svar:** B) Å tjene som den første prosessen og administrere systemoppstart
   - **Forklaring:** 'init' er den første prosessen som starter opp systemet og administrerer andre prosesser.

4. **Hvilken minneallokeringsmetode lider av ekstern fragmentering?**
   - **Riktig svar:** B) Segmentering
   - **Forklaring:** Segmentering kan føre til små, ledige minneområder som ikke kan brukes effektivt.

5. **Hva er en 'trap' i konteksten av operativsystemer?**
   - **Riktig svar:** B) Et programvaregenerert avbrudd
   - **Forklaring:** En 'trap' brukes til systemkall eller feilbehandling.

### **Essayoppgaver**

1. **Sammenlign og kontraster monolittiske kjerner og mikrokjerner. Diskuter fordeler og ulemper ved hver arkitektur.** (10 poeng)

   **Svar:**
   - **Monolittiske kjerner:**
     - **Fordeler:** Raskere ytelse fordi alle tjenester kjører sammen.
     - **Ulemper:** Mindre fleksibel, vanskeligere å vedlikeholde.
   - **Mikrokjerner:**
     - **Fordeler:** Mer modulært, lettere å oppdatere og vedlikeholde.
     - **Ulemper:** Kan være tregere på grunn av flere kommunikasjonslag.
   - **Oppsummering:** Monolittiske kjerner er raske, men mindre fleksible, mens mikrokjerner er mer modulære og sikre, men kan være tregere.

2. **Forklar hvordan semaforer kan brukes til å løse problemet med kritiske seksjoner. Inkluder et eksempel i din forklaring.** (10 poeng)

   **Svar:**
   - **Semaforer:** Kontrollerer hvem som kan bruke en delt ressurs.
   - **Løsning:** Bruk en binær semafor (mutex) for å sikre at kun én prosess kan være i den kritiske seksjonen om gangen.
   - **Eksempel:**
     - Tenk deg at to personer prøver å bruke samme skrivebord samtidig. En semafor fungerer som en lås som bare lar én person bruke skrivebordet om gangen.

3. **Hva er Translation Lookaside Buffer (TLB), og hvordan forbedrer den minnetilgangstider?** (8 poeng)

   **Svar:**
   - **TLB:** En liten, rask cache som lagrer nylige adresseoversettelser.
   - **Forbedrer ytelse:** Reduserer tiden det tar å oversette virtuelle adresser til fysiske adresser ved å gi rask tilgang til ofte brukte adresser.

---

## **Eksamen 4**

### **Flervalgsoppgaver**

1. **I et paged virtuelt minnesystem, hva er en sidefeil (page fault)?**
   - **Riktig svar:** B) Når en etterspurt side ikke er i minnet
   - **Forklaring:** En sidefeil skjer når en prosess prøver å få tilgang til en side som ikke er lastet inn i RAM.

2. **Hvilken av følgende algoritmer er optimal for sideutskiftning, men umulig å implementere i praksis?**
   - **Riktig svar:** C) Optimal sideutskiftning
   - **Forklaring:** Optimal algoritme vet fremtidige sideforespørsler, noe som ikke er mulig å forutsi.

3. **Hva er 'thrashing' i konteksten av operativsystemer?**
   - **Riktig svar:** B) Overdreven paging som forårsaker lav CPU-utnyttelse
   - **Forklaring:** Thrashing skjer når systemet bruker mesteparten av tiden på å bytte sider, noe som reduserer ytelsen.

4. **Hvilken planleggingsalgoritme kan føre til sulting (starvation)?**
   - **Riktig svar:** C) Shortest Job First
   - **Forklaring:** Korteste jobber blir ofte valgt først, noe som kan føre til at lengre jobber aldri får kjørt.

5. **I Linux, hva gjør kommandoen 'chmod'?**
   - **Riktig svar:** B) Endrer filtillatelser
   - **Forklaring:** 'chmod' brukes til å endre hvem som kan lese, skrive eller utføre en fil.

### **Essayoppgaver**

1. **Forklar konseptet med kontekstbytte. Hvilken informasjon må lagres og gjenopprettes under et kontekstbytte?** (10 poeng)

   **Svar:**
   - **Kontekstbytte:** Bytte fra én prosess til en annen på CPU.
   - **Informasjon som lagres:** Programtelleren (hvor prosessen er), registre og prosessens tilstand.
   - **Informasjon som gjenopprettes:** Programtelleren, registre og tilstanden til den nye prosessen.
   - **Prosess:** Lagre tilstanden til den gamle prosessen, laste tilstanden til den nye prosessen, og starte den nye prosessen.

2. **Beskriv strukturen til et Linux-filsystem, inkludert rollen til superblokker, inoder og datablokker.** (10 poeng)

   **Svar:**
   - **Superblokk:** Inneholder informasjon om filsystemet, som størrelse og plassering av inoder.
   - **Inoder:** Lagre metadata om filer, som eier, tillatelser og hvor dataene er lagret.
   - **Datablokker:** Faktiske steder hvor fildata lagres.
   - **Kataloger:** Spesielle filer som peker til inoder for å organisere filer.

3. **Diskuter hvordan Direct Memory Access (DMA) fungerer og fordelene ved I/O-operasjoner.** (8 poeng)

   **Svar:**
   - **DMA:** Lar maskinvareenheter overføre data direkte til/minnet uten å bruke CPU.
   - **Fordeler:**
     - Mindre CPU-belastning.
     - Raskere dataoverføringer.
     - Bedre ytelse ved samtidig prosessering.

---

## **Eksamen 5**

### **Flervalgsoppgaver**

1. **Hva er hovedformålet med 'fork()' systemkallet i Unix/Linux?**
   - **Riktig svar:** B) Å opprette en ny prosess
   - **Forklaring:** 'fork()' lager en kopi av den nåværende prosessen.

2. **Hvilken av følgende er en karakteristikk ved et sanntidsoperativsystem?**
   - **Riktig svar:** B) Deterministiske responstider
   - **Forklaring:** Sanntidsoperativsystemer må reagere innen faste tidsgrenser.

3. **I prosessynkronisering, hva betyr 'mutual exclusion'?**
   - **Riktig svar:** A) Bare én prosess kan være i sin kritiske seksjon om gangen
   - **Forklaring:** Mutual exclusion hindrer flere prosesser i å utføre kritiske operasjoner samtidig.

4. **Hva er hovedfunksjonen til bootloaderen i et operativsystem?**
   - **Riktig svar:** C) Å laste operativsystemkjernen inn i minnet
   - **Forklaring:** Bootloaderen starter oppsystemet ved å laste kjernen inn i RAM.

5. **Hvilket lag i operativsystemarkitekturen interagerer direkte med maskinvaren?**
   - **Riktig svar:** C) Kjernelaget
   - **Forklaring:** Kjernelaget håndterer direkte kommunikasjon med maskinvaren.

### **Essayoppgaver**

1. **Forklar hvordan minnesegmentering fungerer og diskuter fordeler og ulemper sammenlignet med paging.** (10 poeng)

   **Svar:**
   - **Minnesegmentering:** Deler minnet inn i variable segmenter basert på logiske enheter som funksjoner eller data.
   - **Fordeler:**
     - Logisk organisering som matcher programmet.
     - Mindre intern fragmentering enn paging.
   - **Ulemper:**
     - Ekstern fragmentering kan oppstå.
     - Mer komplisert adresseoversettelse.
   - **Sammenligning med Paging:**
     - Paging har ingen ekstern fragmentering og enkel adresseoversettelse, men kan ha intern fragmentering.
     - Segmentering gir bedre organisering, men kan fragmentere minnet eksternt.

2. **Beskriv produsent-forbruker-problemet og gi en løsning ved hjelp av monitorer.** (10 poeng)

   **Svar:**
   - **Produsent-forbruker-problemet:** En prosess (produsent) lager data og legger det i en buffer, mens en annen prosess (forbruker) tar data fra bufferet.
   - **Løsning med Monitorer:**
     - Bruk en monitor som inneholder bufferet og metoder for å produsere og konsumere data.
     - Synkroniser tilgang slik at produsenten ikke legger til data når bufferet er fullt, og forbrukeren ikke tar data når bufferet er tomt.
   - **Eksempel:**
     - Tenk deg en fabrikk der produsenter lager varer og legger dem i et lager, mens forbrukere henter varer ut. Monitoren sørger for at lageret ikke blir overfylt og at forbrukere venter hvis lageret er tomt.

3. **Diskuter rollen til systemkall i operativsystemer. Gi eksempler på vanlige systemkall og deres funksjoner.** (8 poeng)

   **Svar:**
   - **Rolle:** Systemkall lar programmer be operativsystemet om tjenester som filhåndtering, prosesskontroll og minnehåndtering.
   - **Eksempler:**
     - **fork():** Oppretter en ny prosess.
     - **exec():** Laster et nytt program inn i en prosess.
     - **read():** Leser data fra en fil eller enhet.
     - **write():** Skriver data til en fil eller enhet.
     - **open():** Åpner en fil.
     - **close():** Lukker en fil.

4. **Hva er utfordringene knyttet til multitrådet programmering, og hvordan kan synkroniseringsprimitiver bidra til å løse dem?** (12 poeng)

   **Svar:**
   - **Utfordringer:**
     - **Race Conditions:** Feil når tråder endrer delte data samtidig.
     - **Deadlocks:** Tråder venter på hverandre uten å kunne fortsette.
     - **Prioriteringsinvertering:** Lav-prioriterte tråder blokkerer høy-prioriterte tråder.
   - **Løsninger med Synkroniseringsprimitiver:**
     - **Mutexer:** Sikrer at kun én tråd kan utføre en kritisk seksjon om gangen.
     - **Semaforer:** Kan kontrollere tilgang til flere ressurser og koordinere tråder.
     - **Betingelsesvariabler:** Lar tråder vente for spesifikke betingelser og signalere når betingelsen er oppfylt.

