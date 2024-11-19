

## **Eksamen 1**

### **Flervalgsoppgaver**

1. **Hvilken av følgende er IKKE en funksjon til et operativsystem?**
   - A) Minnehåndtering
   - B) Prosesshåndtering
   - C) Applikasjonsutvikling
   - D) Filsystemhåndtering

2. **I en mikrokjerne-arkitektur, hvilke komponenter kjøres typisk i brukermodus?**
   - A) Enhetsdrivere
   - B) Minnehåndtering
   - C) Filsystemer
   - D) Alle de ovennevnte

3. **Hva er formålet med et systemkall i et operativsystem?**
   - A) Å bytte mellom brukermodus og kjernemodus
   - B) Å la brukerprogrammer be om tjenester fra kjernen
   - C) Å håndtere maskinvareavbrudd
   - D) Å utføre kontekstbytter

4. **Hvilken av følgende planleggingsalgoritmer er ikke-preemptiv?**
   - A) Round Robin
   - B) First-Come, First-Served (FCFS)
   - C) Shortest Remaining Time First
   - D) Prioritetsplanlegging

5. **Hva står TLB for i minnehåndtering?**
   - A) Transfer Load Buffer
   - B) Translation Lookaside Buffer
   - C) Temporary Line Buffer
   - D) Transmission Link Buffer

### **Essayoppgaver**

1. **Forklar forskjellene mellom prosesser og tråder. Hvorfor er denne distinksjonen viktig i operativsystemer?** (10 poeng)

2. **Beskriv hvordan paging fungerer i minnehåndtering og diskuter hvordan det hjelper med å implementere virtuelt minne.** (10 poeng)

3. **Hva er de fire nødvendige betingelsene for at en deadlock skal oppstå? Gi eksempler for hver betingelse.** (8 poeng)

4. **Diskuter rollen til filsystemet i et operativsystem. Forklar ulike filallokeringsmetoder og deres fordeler og ulemper.** (12 poeng)

---

## **Eksamen 2**

### **Flervalgsoppgaver**

1. **Hvilken av følgende beskriver best en race condition?**
   - A) En tilstand hvor prosesser kjører med samme hastighet
   - B) En situasjon hvor to prosesser får samtidig tilgang til delt data, noe som fører til feil resultater
   - C) Når prosesser konkurrerer om CPU-tid
   - D) En tilstand hvor en prosess sitter fast i en uendelig løkke

2. **Hva er hovedfordelen med å bruke tråder over flere prosesser?**
   - A) Tråder bruker mer minne
   - B) Tråder er enklere å administrere
   - C) Tråder deler samme adresserom, noe som gir raskere kommunikasjon
   - D) Tråder har høyere overhead enn prosesser

3. **I konteksten av filsystemer, hva er en inode?**
   - A) En peker til neste fil i katalogen
   - B) En datastruktur som lagrer informasjon om en fil
   - C) En type filallokeringsmetode
   - D) En enhetsdriver for inn-/utdata

4. **Hvilken av følgende er en teknikk for å unngå thrashing i virtuelle minnesystemer?**
   - A) Øke sidestørrelsen
   - B) Implementere en arbeidssettmodell
   - C) Bruke FIFO-sideutskiftning
   - D) Redusere mengden fysisk minne

5. **Hva er hovedformålet med en enhetsdriver i et operativsystem?**
   - A) Å administrere systemkall
   - B) Å gi et grensesnitt mellom maskinvareenheter og OS
   - C) Å planlegge CPU-prosesser
   - D) Å administrere minneallokering

### **Essayoppgaver**

1. **Beskriv prosessens tilstandsdiagram og forklar overgangen mellom de forskjellige tilstandene til en prosess.** (10 poeng)

2. **Forklar konseptet med virtuelt minne. Hvordan forbedrer det systemets ytelse og ressursutnyttelse?** (10 poeng)

3. **Diskuter de forskjellige mekanismene for interprosesskommunikasjon (IPC) tilgjengelig i operativsystemer. Gi eksempler hvor hver ville være passende.** (8 poeng)

4. **Hva er forskjellene mellom SSD-er og HDD-er? Diskuter deres innvirkning på operativsystemdesign og ytelse.** (12 poeng)

---

## **Eksamen 3**

### **Flervalgsoppgaver**

1. **Hvilken av følgende er IKKE en type planlegger i et operativsystem?**
   - A) Langtidsplanlegger
   - B) Middelsiktig planlegger
   - C) Korttidsplanlegger
   - D) Nettverksplanlegger

2. **Hva refererer 'heisalgoritmen' til i operativsystemer?**
   - A) CPU-planlegging
   - B) Diskplanlegging
   - C) Minneallokering
   - D) Prosessynkronisering

3. **I Linux, hva er formålet med 'init'-prosessen?**
   - A) Å initialisere maskinvareenheter
   - B) Å tjene som den første prosessen og administrere systemoppstart
   - C) Å håndtere brukerinnlogginger
   - D) Å administrere filtillatelser

4. **Hvilken minneallokeringsmetode lider av ekstern fragmentering?**
   - A) Paging
   - B) Segmentering
   - C) Både paging og segmentering
   - D) Ingen av de ovennevnte

5. **Hva er en 'trap' i konteksten av operativsystemer?**
   - A) Et maskinvareavbrudd
   - B) Et programvaregenerert avbrudd
   - C) En metode for minneallokering
   - D) En type filsystem

### **Essayoppgaver**

1. **Sammenlign og kontraster monolittiske kjerner og mikrokjerner. Diskuter fordeler og ulemper ved hver arkitektur.** (10 poeng)

2. **Forklar hvordan semaforer kan brukes til å løse problemet med kritiske seksjoner. Inkluder et eksempel i din forklaring.** (10 poeng)

3. **Hva er Translation Lookaside Buffer (TLB), og hvordan forbedrer den minnetilgangstider?** (8 poeng)

4. **Diskuter trinnene involvert i håndtering av et avbrudd i et operativsystem.** (12 poeng)

---

## **Eksamen 4**

### **Flervalgsoppgaver**

1. **I et paged virtuelt minnesystem, hva er en sidefeil (page fault)?**
   - A) En feil på grunn av ugyldig minnetilgang
   - B) Når en etterspurt side ikke er i minnet
   - C) En feil i allokering av sidetabeller
   - D) En type segmenteringsfeil

2. **Hvilken av følgende algoritmer er optimal for sideutskiftning, men umulig å implementere i praksis?**
   - A) FIFO
   - B) LRU (Least Recently Used)
   - C) Optimal sideutskiftning
   - D) Klokkealgoritmen

3. **Hva er 'thrashing' i konteksten av operativsystemer?**
   - A) Høy CPU-utnyttelse
   - B) Overdreven paging som forårsaker lav CPU-utnyttelse
   - C) Diskfragmentering
   - D) Nettverksbelastning

4. **Hvilken planleggingsalgoritme kan føre til sulting (starvation)?**
   - A) Round Robin
   - B) First-Come, First-Served
   - C) Shortest Job First
   - D) Flernivå køplanlegging

5. **I Linux, hva gjør kommandoen 'chmod'?**
   - A) Endrer eieren av en fil
   - B) Endrer filtillatelser
   - C) Sletter en fil
   - D) Flytter en fil til en annen katalog

### **Essayoppgaver**

1. **Forklar konseptet med kontekstbytte. Hvilken informasjon må lagres og gjenopprettes under et kontekstbytte?** (10 poeng)

2. **Beskriv strukturen til et Linux-filsystem, inkludert rollen til superblokker, inoder og datablokker.** (10 poeng)

3. **Diskuter hvordan Direct Memory Access (DMA) fungerer og fordelene ved I/O-operasjoner.** (8 poeng)

4. **Hva er de viktigste sikkerhetsutfordringene i operativsystemer, og hvordan kan de reduseres?** (12 poeng)

---

## **Eksamen 5**

### **Flervalgsoppgaver**

1. **Hva er hovedformålet med 'fork()' systemkallet i Unix/Linux?**
   - A) Å opprette en ny tråd
   - B) Å opprette en ny prosess
   - C) Å avslutte en prosess
   - D) Å kjøre et nytt program

2. **Hvilken av følgende er en karakteristikk ved et sanntidsoperativsystem?**
   - A) Høy gjennomstrømning
   - B) Deterministiske responstider
   - C) Brukervennlige grensesnitt
   - D) Virtuell minnehåndtering

3. **I prosessynkronisering, hva betyr 'mutual exclusion'?**
   - A) Bare én prosess kan være i sin kritiske seksjon om gangen
   - B) Prosesser er gjensidig utelukkende hvis de ikke deler ressurser
   - C) Prosesser utelukker hverandre fra å kjøre
   - D) Alle prosesser kjører samtidig

4. **Hva er hovedfunksjonen til bootloaderen i et operativsystem?**
   - A) Å laste inn enhetsdrivere
   - B) Å initialisere filsystemet
   - C) Å laste operativsystemkjernen inn i minnet
   - D) Å administrere brukerinnlogginger

5. **Hvilket lag i operativsystemarkitekturen interagerer direkte med maskinvaren?**
   - A) Applikasjonslaget
   - B) Brukergrensesnittlaget
   - C) Kjernelaget
   - D) Biblioteklaget

### **Essayoppgaver**

1. **Forklar hvordan minnesegmentering fungerer og diskuter fordeler og ulemper sammenlignet med paging.** (10 poeng)

2. **Beskriv produsent-forbruker-problemet og gi en løsning ved hjelp av monitorer.** (10 poeng)

3. **Diskuter rollen til systemkall i operativsystemer. Gi eksempler på vanlige systemkall og deres funksjoner.** (8 poeng)

4. **Hva er utfordringene knyttet til multitrådet programmering, og hvordan kan synkroniseringsprimitiver bidra til å løse dem?** (12 poeng)

---

### **Flervalgsoppgaver**

1. **IKT102: Generell informasjon**  
   Hva er hovedfunksjonen til et operativsystem?  
   - A) Å administrere maskinvare og programvare  
   - B) Å utvikle nye programmer  
   - C) Å oppdatere maskinvaredrivere automatisk  
   - D) Å lage brukervennlige grensesnitt  

2. **DAT103: Hva er en node?**  
   Hva beskriver en "node" i et operativsystem?  
   - A) En prosess som kjører i bakgrunnen  
   - B) En tilkoblet enhet i et nettverk  
   - C) En del av minnehierarkiet  
   - D) En type fil i et katalogsystem  

3. **DAT103: Formålet med filer og kataloger**  
   Hva er hovedformålet med kataloger i et filsystem?  
   - A) Å lagre metadata om filer  
   - B) Å organisere filer i en strukturert måte  
   - C) Å redusere fragmentering i minnet  
   - D) Å opprette lenker mellom prosesser  

4. **DAT103: Kategorier av inn-/utdata (I/O)**  
   Hvilke kategorier av inn-/utdata opererer operativsystemer med?  
   - A) Blokkerte og ikke-blokkerte  
   - B) Synkrone og asynkrone  
   - C) Kontinuerlige og diskrete  
   - D) Alle de ovennevnte  

5. **DAT103: Når kan en deadlock oppstå?**  
   Hvilken situasjon er en forutsetning for at en deadlock kan oppstå?  
   - A) Når to prosesser deler ressursene sine  
   - B) Når alle prosesser frigis samtidig  
   - C) Når ressurser holdes og ventes på samtidig  
   - D) Når en prosess fullfører uten å frigjøre ressurser  

6. **DAT103: Paging og modifikasjoner**  
   Hvordan fungerer paging i minnehåndtering?  
   - A) Ved å dele fysisk minne inn i faste blokker  
   - B) Ved å allokere minne dynamisk basert på prosessens behov  
   - C) Ved å la alle prosesser dele samme minneområde  
   - D) Ved å flytte data mellom kjerneminne og cache  

7. **DAT103: Metoder for filallokering**  
   Hva er en fordel med indeksert filallokering?  
   - A) Det krever mindre lagringsplass for metadata  
   - B) Det gir rask tilgang til tilfeldige blokker  
   - C) Det unngår ekstern fragmentering helt  
   - D) Det sikrer sekvensiell datahåndtering  

8. **DAT103: Stack for prosess eller tråd**  
   Hva brukes stack til i en prosess eller tråd?  
   - A) For å lagre globale variabler  
   - B) For å lagre lokale variabler og funksjonskall  
   - C) For å dele data mellom prosesser  
   - D) For å administrere minnehierarkiet  

9. **DAT103: Operativsystemets kjøring**  
   I hvilken modus kjører operativsystemkjernen?  
   - A) Brukermodus  
   - B) Kjernemodus  
   - C) Bakgrunnsmodus  
   - D) Nettverksmodus  

10. **DAT103: Translation Lookaside Buffer (TLB)**  
   Hva er hovedformålet med TLB i minnehåndtering?  
   - A) Å redusere tiden for sideoversetting  
   - B) Å lagre data for senere behandling  
   - C) Å overvåke minnefragmentering  
   - D) Å håndtere paging-feil  

11. **DAT103: Heisalgoritmen**  
   Hva er formålet med heisalgoritmen i diskplanlegging?  
   - A) Å redusere søketiden ved å organisere forespørsler sekvensielt  
   - B) Å sikre rettferdig tilgang til diskressurser  
   - C) Å forhindre deadlock under diskoperasjoner  
   - D) Å maksimere overføringshastigheten for data  

