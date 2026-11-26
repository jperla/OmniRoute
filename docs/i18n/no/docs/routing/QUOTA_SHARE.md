# Quota Sharing Engine (Norsk)

🌐 **Languages:** 🇺🇸 [English](../../../../routing/QUOTA_SHARE.md) · 🇪🇹 [am](../../../am/docs/routing/QUOTA_SHARE.md) · 🇸🇦 [ar](../../../ar/docs/routing/QUOTA_SHARE.md) · 🇦🇿 [az](../../../az/docs/routing/QUOTA_SHARE.md) · 🇧🇬 [bg](../../../bg/docs/routing/QUOTA_SHARE.md) · 🇧🇩 [bn](../../../bn/docs/routing/QUOTA_SHARE.md) · 🇧🇦 [bs](../../../bs/docs/routing/QUOTA_SHARE.md) · 🇨🇿 [cs](../../../cs/docs/routing/QUOTA_SHARE.md) · 🇩🇰 [da](../../../da/docs/routing/QUOTA_SHARE.md) · 🇩🇪 [de](../../../de/docs/routing/QUOTA_SHARE.md) · 🇬🇷 [el](../../../el/docs/routing/QUOTA_SHARE.md) · 🇪🇸 [es](../../../es/docs/routing/QUOTA_SHARE.md) · 🇪🇪 [et](../../../et/docs/routing/QUOTA_SHARE.md) · 🇮🇷 [fa](../../../fa/docs/routing/QUOTA_SHARE.md) · 🇫🇮 [fi](../../../fi/docs/routing/QUOTA_SHARE.md) · 🇫🇷 [fr](../../../fr/docs/routing/QUOTA_SHARE.md) · 🇮🇪 [ga](../../../ga/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [gu](../../../gu/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [ha](../../../ha/docs/routing/QUOTA_SHARE.md) · 🇮🇱 [he](../../../he/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [hi](../../../hi/docs/routing/QUOTA_SHARE.md) · 🇭🇷 [hr](../../../hr/docs/routing/QUOTA_SHARE.md) · 🇭🇺 [hu](../../../hu/docs/routing/QUOTA_SHARE.md) · 🇦🇲 [hy](../../../hy/docs/routing/QUOTA_SHARE.md) · 🇮🇩 [id](../../../id/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [ig](../../../ig/docs/routing/QUOTA_SHARE.md) · 🇮🇹 [it](../../../it/docs/routing/QUOTA_SHARE.md) · 🇯🇵 [ja](../../../ja/docs/routing/QUOTA_SHARE.md) · 🇬🇪 [ka](../../../ka/docs/routing/QUOTA_SHARE.md) · 🇰🇭 [km](../../../km/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [kn](../../../kn/docs/routing/QUOTA_SHARE.md) · 🇰🇷 [ko](../../../ko/docs/routing/QUOTA_SHARE.md) · 🇱🇹 [lt](../../../lt/docs/routing/QUOTA_SHARE.md) · 🇱🇻 [lv](../../../lv/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [ml](../../../ml/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [mr](../../../mr/docs/routing/QUOTA_SHARE.md) · 🇲🇾 [ms](../../../ms/docs/routing/QUOTA_SHARE.md) · 🇲🇹 [mt](../../../mt/docs/routing/QUOTA_SHARE.md) · 🇲🇲 [my](../../../my/docs/routing/QUOTA_SHARE.md) · 🇳🇵 [ne](../../../ne/docs/routing/QUOTA_SHARE.md) · 🇳🇱 [nl](../../../nl/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [or](../../../or/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [pa](../../../pa/docs/routing/QUOTA_SHARE.md) · 🇵🇭 [phi](../../../phi/docs/routing/QUOTA_SHARE.md) · 🇵🇱 [pl](../../../pl/docs/routing/QUOTA_SHARE.md) · 🇵🇹 [pt](../../../pt/docs/routing/QUOTA_SHARE.md) · 🇧🇷 [pt-BR](../../../pt-BR/docs/routing/QUOTA_SHARE.md) · 🇷🇴 [ro](../../../ro/docs/routing/QUOTA_SHARE.md) · 🇷🇺 [ru](../../../ru/docs/routing/QUOTA_SHARE.md) · 🇱🇰 [si](../../../si/docs/routing/QUOTA_SHARE.md) · 🇸🇰 [sk](../../../sk/docs/routing/QUOTA_SHARE.md) · 🇸🇮 [sl](../../../sl/docs/routing/QUOTA_SHARE.md) · 🇷🇸 [sr](../../../sr/docs/routing/QUOTA_SHARE.md) · 🇸🇪 [sv](../../../sv/docs/routing/QUOTA_SHARE.md) · 🇰🇪 [sw](../../../sw/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [ta](../../../ta/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [te](../../../te/docs/routing/QUOTA_SHARE.md) · 🇹🇭 [th](../../../th/docs/routing/QUOTA_SHARE.md) · 🇹🇷 [tr](../../../tr/docs/routing/QUOTA_SHARE.md) · 🇺🇦 [uk-UA](../../../uk-UA/docs/routing/QUOTA_SHARE.md) · 🇵🇰 [ur](../../../ur/docs/routing/QUOTA_SHARE.md) · 🇺🇿 [uz](../../../uz/docs/routing/QUOTA_SHARE.md) · 🇻🇳 [vi](../../../vi/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [yo](../../../yo/docs/routing/QUOTA_SHARE.md) · 🇨🇳 [zh-CN](../../../zh-CN/docs/routing/QUOTA_SHARE.md) · 🇹🇼 [zh-TW](../../../zh-TW/docs/routing/QUOTA_SHARE.md)

---

> **Dokumentreferanse**: `docs/routing/QUOTA_SHARE.md`
> Del av gruppe B (plan 16 + 22).

---

## Oversikt

Kvotedelingsmotoren fordeler en leverandørs tidsbaserte kvote (f.eks. Codex'
5-timersvindu, Kimi 1500 forespørsler/t) rettferdig mellom flere API-nøkler som
deler samme tilkobling.

**Problemet den løser:** OmniRoute videresender mange API-nøkler til den samme
oppstrøms leverandørkontoen. Uten delingslogikk kan en trafikktopp fra nøkkel A
bruke opp leverandørkvoten for timen, slik at nøklene B og C blokkeres frem til
vinduet tilbakestilles. Motoren forhindrer dette ved å:

1. Spore hver nøkkels løpende forbruk per dimensjon (%, forespørsler, tokener, $).
2. Bruke en arbeidsbevarende algoritme for rettferdig fordeling: En nøkkel kan
   låne fra ubrukte andeler så lenge den globale kapasiteten ikke er mettet.
3. Håndheve resultatet i den kritiske kjørebanen (`chatCore.ts`) før forespørselen
   når den oppstrøms eksekveringskomponenten.

---

## Algoritme: Fair-Share Work-Conserving

Implementert i `src/lib/quota/fairShare.ts`.

### Modi

| Betingelse                                 | Modus        | Oppførsel                                                           |
| ------------------------------------------ | ------------ | ------------------------------------------------------------------- |
| `globalUsedPercent < saturationThreshold`  | **Sjenerøs** | Nøkkelen kan låne opp til den globale grensen minus forbrukt-totalt |
| `globalUsedPercent >= saturationThreshold` | **Streng**   | Håndhev individuell rettferdig andel strengt                        |

Standard `saturationThreshold = 0.5` (env `QUOTA_SATURATION_THRESHOLD`).

Disse to modusene beskriver en pool i standard lånemodus, `saturation`. Et basseng i `consent` modus bruker alltid de strenge reglene, uansett metning. Se [Samtykkede utlån (opt-in per pool)](#consented-lending-per-pool-opt-in).

### Beslutning per dimensjon

For hver aktive dimensjon i bassenget, beregner motoren:

```
fairShareAllowed = poolLimit × (allocationWeight / 100)
consumed        = current rolling value for this key (from QuotaStore.peek)
remaining       = fairShareAllowed - consumed
```

For `percent` dimensjoner kommer `consumed` fra attribusjonsboken i stedet (se [Prosentdimensjoner: attribusjon per nøkkel](#percent-dimensions-per-key-attribution) ).

Da:

- **`policy = hard`** : hvis `consumed > fairShareAllowed` og modus er streng →** blokkere** .
- **`policy = soft`** : hvis `consumed > fairShareAllowed` og modus er streng →** straffe** (nedprioriter i kombinasjon; aldri hard-block).
- **`policy = burst`** : tillat mens global takhøyde eksisterer uavhengig av rettferdig andel.

### Cap absoluto

`capValue` + `capUnit` på en allokering er et hardt tak uavhengig av modus eller policy. Enhver dimensjon der `consumed >= capValue` alltid** blokker** forespørselen. For en `percent` cap er `consumed` bare delen som tilskrives nøkkelen.

### Flerdimensjonssjekk

En forespørsel blokkeres hvis** noen** dimensjon i bassenget ville blokkere det. Dimensjonene er uavhengige — en 5t % utmattelse påvirker ikke den ukentlige %-dimensjonen.

### Låne

I generøs modus kan en nøkkel hvis tildeling er underforbrukt bruke overskudd fra andre nøklers ikke-allokerte andeler. Formelen er:

```
maxAllowed = globalLimit - consumedByOtherKeys
```

hvor `consumedByOtherKeys = consumedTotal - consumedByThisKey`. Teto global (pool `limit` for den dimensjonen) er alltid det harde taket.

### Samtykkede utlån (påvalg per gruppe)

Hvert basseng har en lånemodus. `saturation` er standard og beholder reglene ovenfor. I `consent` modus overfører en `hard` nøkkel sin andel bare innenfor kapasiteten som andre nøkler gikk med på å låne ut. Administratoren angir modusen for hvert basseng. Hver nøkkelinnehaver gir sitt eget samtykke gjennom [utlånssamtykke](#lending-consent).

Et samtykke er en prosentandel fra 0 til 100 og en valgfri frist i epoke millisekunder. Nøkkelen låner ut den prosentandelen av sin ledige andel mens fristen er i fremtiden.

For én dimensjon er `L` den effektive grensen: plangrensen ganger kontoene i bassenget. Porten beregner for nøkkelen som ber om:

```
share_k         = w_k / 100 × L
idle_k          = max(0, share_k − consumed_k)
lent            = Σ over the other keys of lend_k / 100 × idle_k
taken           = Σ over the other keys of max(0, consumed_k − share_k)
borrowAvailable = max(0, lent − taken)
```

`w_k` er nøkkelens vekt, eller `100 / n` for hver nøkkel når ingen vekt er over 0. `lend_k` er nøkkelens aktive prosentandel, og 0 når fristen har passert. Den som ber om nøkkelens eget samtykke teller aldri. En `hard` nøkkel blir avvist når forbruket når sin andel pluss `borrowAvailable`.

Kapasitet som ingen tildeling krever (100 minus summen av vektene) er ikke utlånbar. Ingen nøkkel gikk med på å låne den ut.

**Eksempel.** `L` er 1000.

| Nøkkel | Vekt | Dele | Forbrukt | Låner ut |
| ------ | ---- | ---- | -------- | -------- |
| EN     | 50   | 500  | 530      | 0%       |
| B      | 30   | 300  | 100      | 50%      |
| C      | 0    | 0    | 60       | 0%       |

- B låner ut 50 % av sine ledige 200, som er 100. C tok allerede 60 over sin andel. A kan låne 40.
- A blir servert på 530 og nektet når forbruket når 540.
- Før C brukte noe, med A på eller under sin andel, kunne C låne 100.
- Før C brukte noe, med A på 530, kunne C låne 70.

**Null vekt.** En nøkkel med vekt 0 har en andel på 0. Den serveres kun mens forbruket er under det andre låner ut. Når ingen låner ut, blir det avslått fra første forespørsel.

**Frister.** Ingen bakgrunnsoppgave utløper et samtykke. Hver forespørsel sammenligner fristen med sin egen tid, og en frist lik den tiden har gått. En lagret frist som ikke er et endelig tall, eller som er forbi den største datoen en `Date` kan holde, regnes som passert.

**`soft` og `burst`.** Utlån begrenser dem ikke. En `soft` nøkkel blir deprioritert en gang forbi sin del. En `burst` nøkkel passerer mens bassenget har plass. Bassengtaket nekter fortsatt hver nøkkel når bassengets totalbeløp når grensen.

**Kostnad på forespørselsbanen.** Et `saturation` basseng leser ingenting mer enn før. I en `consent` pool leser en tellbar dimensjon de andre nøklene bare for en `hard` nøkkel på eller over sin andel mens en annen nøkkel gir utlån. Den gjør så en lesing per annen nøkkel, parallelt. En mislykket lesing teller som et forbruk på 0 for den nøkkelen. En `percent` dimensjon legger ikke til lesing, fordi attribusjonsboken inneholder hver nøkkel.

**Redigere et basseng.** En redigering beholder samtykket fra nøklene som blir værende. Dette gjelder for allokeringsredigeringer, gruppeomfattende erstatninger og `ensure` anrop. En fjernet nøkkel mister sitt samtykke, og en nøkkel lagt tilbake starter på 0. Administratorrutene returnerer hver nøkkels samtykke og skriver det aldri. Å bytte en pool tilbake til `saturation` beholder alle lagrede samtykker, som ikke har noen effekt i den modusen. Ved å bytte bassenget til `consent` igjen aktiveres de lagrede samtykkene hvis fristen ikke har passert. En nøkkelholder kan slette et lagret samtykke i begge modusene.

**Oppgradering.** Hvis kolonnene `lending_percent` og `lending_until` allerede eksisterer, legger migreringen bare til `borrow_mode`, og lagrede prosenter forblir som de er. Hvert basseng starter i `saturation` modus. Slå på `consent` per basseng i bassengveiviseren. Ingenting utledes fra de lagrede verdiene.

**Begrensninger.**

- En utlåner kan finne bassenget i taket før det bruker sin egen andel. Kapasitet som andre lånte teller mot bassengets totalsum.
- Sjekken kjører før forespørselen og reserverer ingenting. Samtidige forespørsler leser forbruket før det registreres, så utlånt kapasitet kan brukes mer enn én gang, begrenset av forespørslene under flyvning. Delingssjekken til `saturation` modus har samme egenskap.

---

## Teller med glidende vindu

Implementert i `src/lib/quota/sqliteQuotaStore.ts` og `redisQuotaStore.ts`.

To segmenter per `(apiKeyId, dimensionKey)`:

- `curr`: gjeldende segment (`floor(nowMs / windowMs)`)
- `prev`: forrige segment (`curr - 1`)

Effektiv løpende verdi:

```
effectiveBucketIndex = floor(nowMs / windowMs)
bucketStartMs        = effectiveBucketIndex × windowMs
elapsed              = nowMs - bucketStartMs
weight               = 1 - elapsed / windowMs

effective = prev × weight + curr
```

**Presisjon**: ~99 % nøyaktig. Feilen er maksimalt 1 % av vindusstørrelsen ved
grensen mellom segmenter (iboende i tilnærmingen med to segmenter).

### Samtidighet

SQLite-driver: En mutex i minnet per `(apiKeyId | dimensionKey)`-nøkkel forhindrer
kappløp ved lesing–endring–skriving. Mønsteret gjenspeiler beskyttelsen mot samtidige
identiske forespørsler i `src/sse/services/auth.ts`.

Redis-driver: Lua EVAL-skript for atomær økning — kjøres som én enkelt Redis-kommando.

---

## Drivere

### SQLite (standard, ingen installasjon)

- Tabell: `quota_consumption` (se migrering `073_quota_pools.sql` / `074_quota_consumption.sql`).
- Best egnet for distribusjoner med én instans.
- All persistens lagres i den eksisterende OmniRoute SQLite-databasen (`DATA_DIR/storage.sqlite`).

### Redis (valgfritt, flere instanser)

- Krever npm-pakken `ioredis`.
- Tellere lagres i Redis. Metadata (pooler/tildelinger) lagres fortsatt i SQLite.
- Best egnet for distribusjoner med flere replikaer der tellere må deles.

### Bytte av driver

Via innstillingsgrensesnittet (`/dashboard/settings` → Kvotelager), eller via miljøvariabler:

```bash
QUOTA_STORE_DRIVER=redis
QUOTA_STORE_REDIS_URL=redis://localhost:6379
```

Databaseinnstillingen har forrang over miljøvariabler. Hvis `driver=redis`, men URL-en mangler eller
`ioredis` ikke er installert, faller fabrikken tilbake til SQLite og logger en advarsel.

Rekkefølge for valg av driver:

1. Databaseinnstillingen `quotaStore.driver`
2. Miljøvariabelen `QUOTA_STORE_DRIVER`
3. Standard: `sqlite`

---

## Multi-Dimensjon

Et basseng kan ha flere dimensjoner. Hver dimensjon er uavhengig:

```ts
QuotaDimension {
  unit: "percent" | "requests" | "tokens" | "usd",
  window: "5h" | "hourly" | "daily" | "weekly" | "monthly",
  limit: number,  // global pool ceiling for this dimension
}
```

**Eksempel: Codex plan** (5t% + ukentlig%):

```json
[
  { "unit": "percent", "window": "5h", "limit": 100 },
  { "unit": "percent", "window": "weekly", "limit": 100 }
]
```

En forespørsel må tilfredsstille alle dimensjoner for å tillates.

### Prosentdimensjoner: attribusjon per nøkkel

En prosentplan rapporterer ett brukstall per konto og planvindu. Leverandøren gir ingen teller per API nøkkel.

For å dele dette tallet mellom nøkler, fører hver pool en attribusjonsbok per konto og planvindu. `src/lib/quota/percentLedger.ts` holder bokens regler. `src/lib/quota/percentAttribution.ts` gjør boken til tallene som håndhevelsen bruker. Resultatet er et estimat bygget fra tokens hver nøkkelrute.

#### Lesninger som beveger boken

Boken flytter kun på leverandørens egen figur for det forespurte planvinduet. Disse forbindelsene rapporterer en:

| Leverandør                          | Plan vinduer   |
| ----------------------------------- | -------------- |
| Claude, gjennom en OAuth tilkobling | `5h`, `weekly` |
| Codex                               | `5h`, `weekly` |

Disse teller ikke som lesning:

- et svar leverandørklienten markerer som foreldet
- et Claude vindu hvis prosentandel leverandøren ikke rapporterte
- et annet vindus figur, eller i verste fall på tvers av vinduer
- fallback-overskriften for rategrense
- en mislykket lesing

Andre leverandører, inkludert Claude med en API nøkkel, har ingen bok. Hver nøkkel belastes 0 på sine prosentmål, som før denne endringen.

En lesing deler 30-sekunders cachen til metningssignalet. En Claude -avlesning dateres etter når tallet ble observert i svaroverskrifter eller lest fra bruksendepunktet, når dette tidspunktet er kjent. Andre avlesninger er datert etter når cache-oppføringen ble bygget.

#### Hva boken holder

Hver registrert forespørsel legger til sine tokens, én gang, til en teller per pool, konto og nøkkel. En teller bare vokser. Boken inneholder tre ting:

- grunnlinjen: tallet da boken åpnet eller vinduet sist snudde
- det sist brukte tallet
- per nøkkel, dens token-teller i samme øyeblikk, kalt dens merke

Boken oppdateres når håndhevelse eller bruksruten beregner attribusjonen. Skrivinger sammenlignes og settes på et revisjonsnummer. En forfatter som taper forsøk på nytt én gang på fersk lesning.

#### Hvordan en nøkkels del beregnes

Hver nøkkels del beregnes når boken leses. Veksten av figuren siden grunnlinjen er delt mellom nøklene i forhold til tokenene som hver har rutet siden merket.

Together, disse tokenene forklarer maksimalt ett punkt av tallet per `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` -tokens (standard 1000). Veksten de ikke forklarer er ekstern. Grunnlinjen er også ekstern.

For eksempel åpner en bok ved 0. Nøkkel A ruter deretter 900 000 tokens og nøkkel B ruter 100 000. Ved et tall på 60 er A sin del 54 poeng og B sin del er 6.

En teller under nøkkelens merke har startet på nytt og teller fullt ut. En nøkkel uten et merke, for eksempel en nøkkel som slutter seg til bassenget midt i et vindu, teller alle symbolene. Et tall som ligger etter tokens forårsaker en feil som forsvinner ved neste lesing. Det hoper seg ikke opp.

`QUOTA_PERCENT_MIN_TOKENS_PER_POINT` leses på hver attribusjon. En verdi som ikke er et endelig tall på minst 1 faller tilbake til 1000.

#### Hvordan en lesning endrer boken

Den første samsvarsregelen gjelder:

1. **Ingen bok ennå:** lesingen åpner boken. Figuren er grunnlinjen og hver teller er merket.
2. **Eldre lesning:** en avlesning datert før den sist brukte blir ignorert. Det samme er en avlesning hvis tilbakestillingstid er mer enn 30 minutter tidligere enn den lagrede.
3. **Nytt leverandørvindu:** en tilbakestillingstid mer enn 30 minutter senere enn den lagrede snur boken. Figuren blir grunnlinjen og hver teller markeres igjen. Nøkler uten disk forlater boken.
4. **Avsluttet vindu:** en lagret tilbakestillingstid som ikke er etter avlesningens datatid betyr at vinduet er avsluttet. Lesingen snur boken, uansett figur.
5. **Høyere tall:** bare den siste figuren beveger seg. Grunnlinjen og merkene forblir.
6. **Samme figur:** figuren, grunnlinjen og merkene forblir. Kun en tilbakestillingstid boken mangler er skrevet.
7. **Nedre figur:** et lavere tall brukes aldri som sådan. Det snur boken først når tre ting holder. Den er minst to minutter nyere enn den sist brukte avlesningen. Ingenting sier at vinduet er det samme åpne. Det er mer enn ett poeng lavere.

Vinduet teller som det samme åpne når tre ting holder. Begge tilbakestillingstidene er kjent. De er innen 30 minutter fra hverandre. Den lagrede er fortsatt i forkant av lesingen. En lavere figur inne i vinduet endrer ingenting.

En tilbakestillingstid lagres bare mens den er foran datatiden for avlesningen som bærer den. Et høyere tall lagrer avlesningens tilbakestillingstid når den er brukbar, og beholder den lagrede ellers. Et likt tall registrerer lesningens tilbakestillingstid bare når boken ikke har noen. Det endrer ingenting annet. Et lavere tall som ikke snur boken registrerer ingen tilbakestillingstid.

#### Når boken brukes

Etter en lesing brukes boken med mindre den lagrede tilbakestillingstiden ikke er etter gjeldende tid. Dette tilfellet oppstår når en avlesning tatt rett før tilbakestillingen, for eksempel en som ble servert fra hurtigbufferen, observeres like etter den.

Uten en brukbar lesing brukes den lagrede boken bare mens den fortsatt kan være boken til det gjeldende vinduet. Det gjelder i to tilfeller:

- tilbakestillingstiden er kjent og ligger fortsatt foran
- den har ingen tilbakestillingstid, og den siste avlesningen som endret den er maksimalt 15 minutter gammel

Ellers tilskrives ingenting, som når det ikke er noen bok. En bok hvis lagrede tilbakestillingstid har gått, belastes aldri.

#### Håndhevelse

En nøkkels forbruk på en prosentdimensjon er dens tilordnede del pluss en andel av den eksterne delen. Den eksterne delen bruker først kapasiteten ingen tildelingskrav (100 minus summen av vektene). Bare det overskytende deles mellom nøklene etter vekt.

Dette forbruket sammenlignes med nøkkelens rimelige andel som for enhver annen dimensjon. Strenge modus starter fortsatt når metningssignalet når `QUOTA_SATURATION_THRESHOLD` (standard 0,5). Hvert tall skaleres med den effektive grensen: grensen per konto ganger antall kontoer i bassenget.

En absolutt topp med `capUnit: "percent"` teller bare delen som tilskrives nøkkelen, skalert på samme måte. Ta en grense per konto på 100 og k kontoer. Et tak på N nås når nøkkelens del av serveringskontoens tall når N/k poeng. Hver konto kontrolleres mot sin egen bok. For eksempel, med to kontoer, nås et tak på 10 ved 5 poeng av en kontos tall.

Når butikken ikke kan leses, tilskrives ingenting, og hver nøkkel belastes 0 på den dimensjonen. Når en bokskriving mislykkes, bruker den attribusjonen boken slik den ble lest. En mislykket token-skriving etterlater forespørselens tokens ute av boken. Ingen av disse feilene blokkerer en forespørsel.

I en `consent` pool bruker utlånsformelen hver nøkkels forbruk på prosentdimensjonen som beskrevet ovenfor. Når en annen nøkkel låner ut, leses boken én gang og tilskrives hver nøkkel. Uten en brukbar bok belastes hver nøkkel med 0. En nøkkel med vekt passerer da, og en nøkkel med vekt 0 passerer bare når en annen nøkkel låner ut.

#### Bruksrute

`GET /api/quota/pools/{id}/usage` rapporterer de samme tallene gjennom samme funksjon. En prosentdimensjon har én oppføring per bassengtilkobling i `accounts`. Toppnivået `consumedTotal` og `perKey` speiler den første oppføringen.

Ruten bruker den gjeldende lesingen også, slik at den kan fremme boken som en forespørsel gjør. `internal + external` kan avvike fra `consumedTotal` når det ikke er noen brukbar avlesning, eller når et lavere tall ikke brukes.

#### Lagring og oppbevaring

Begge kvotebutikkene holder boken. På SQLite fjerner den automatiske databaseoppryddingen, når den er aktivert, rader som ikke er oppdatert på 60 dager. På Redis deler bøkene og tellerne til en bassengforbindelse én nøkkel. Den utløper 60 dager etter siste tokenskriving eller bokbytte. En bok som ikke endres skrives ikke om, så avskjæringen settes over det lengste planvinduet. Den manuelle tilbakestillingen av brukshistorikken sletter også bøkene på SQLite (se Begrensninger).

#### Begrensninger

- All vekst av kontotallet siden grunnlinjen er delt av tokens hver nøkkel rutet siden da. Når den veksten skjedde spiller ingen rolle.
- Så bruk som gjøres utenfor OmniRoute belastes nøklene opp til det deres tokens tillater. Dette inkluderer bruk gjort før en nøkkels første forespørsel om vinduet, når boken allerede var åpen.
- For eksempel øker bruk utenfor kontoen 60 poeng mens ingen nøkkelruter. En nøkkel ruter deretter 30 000 tokens og tallet når 60,6.
- Hvis boken var åpen før bruk, er nøkkelens del 30 poeng. Den har også 7,65 ekstern bruk, med fire nøkler med vekt 25.
- Hvis boken åpnet etter den bruken, er de 60 poengene grunnlinjen. Nøkkelens del er 0,6 poeng, og den har 15 ekstern bruk.
- En forespørsel eller et besøk på bruksruten åpner boken. Så om slik bruk teller som baseline avhenger av når boken åpnet.
- Med standardgulvet, en nøkkel som ruter 60 000 tokens mens bruk utenfor gir kontoen 60 poeng får alle 60 som sin egen del.
- Med gulvet på 50.000 er egen del 1,2 poeng. De andre 58.8 er eksterne og lades etter vekt, som all ekstern bruk.
- Sett `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` nær det ett poeng koster på planen din. Utendørs bruk inkluderer trafikk på samme konto fra nøkler utenfor bassenget.
- Et prosenttak gjelder i hver modus. En begrenset nøkkel kan nektes mens kontoen er langt under metningsgrensen.
- Ta et tak på 10 og 12 poeng for utendørs bruk tidligere i vinduet. En nøkkel som ruter 20 000 tokens blir deretter avvist med et kontotall på 12,4 %.
- Delingen er et estimat etter tokenvolum. En forespørsel teller som dens prompt-tokens pluss dens fullførings-tokens. Cache-rabatter og modellpriser endrer ikke dette antallet.
- En forespørsel som ikke ender med status 200 registrerer ingen tokens. Eksempler er en strøm som klienten kobler fra og en oppstrømsfeil etter at bruken ble konsumert.
- Bruken en slik forespørsel forårsaket belastes nøklene som registrerte tokens, opp til hva deres tokens tillater. Resten er ekstern. Den beveger seg ikke tilbake. Et svar som rapporterer ingen tokenbruk registrerer heller ingen tokens.
- Bruken av en pågående forespørsel kan vises i en annen aktiv nøkkels del for hele forespørselen. Den flyttes bare tilbake når forespørselen avsluttes med status 200.
- Bruk som allerede er på kontoen når en bok åpnes, regnes som ekstern. Dette dekker en oppgradering, en ny pool og en ny konto. Bruk i et nytt vindu før første lesing teller også som eksternt.
- Hver nøkkel starter med sin vektandel av denne bruken, etter kapasiteten ingen tildeling krever. Med én konto på 85 % og fem nøkler med vekt 20, starter hver med 17 av sine 20 brukte.
- I en pulje med flere konti påføres serveringskontoens tall på det summerte budsjettet. Dette er uendret av boken.
- Et lavere tall inne i et vindu leverandøren rapporterer som åpent, brukes ikke. En tilbakestillingstid som går tilbake med mer enn 30 minutter, behandles som en gammel avlesning.
- I begge tilfeller beholder boken statusen til den lagrede tilbakestillingstiden går. Etter det lades ikke boken før en lesning snur den.
- Løsningen er manuell tilbakestilling av brukshistorikk (`POST /api/settings/purge-usage-history`). Den sletter attribusjonsbøkene og deres token-tellere i SQLite databasen.
- `all` perioden sletter hver bok og teller. En kortere periode fjerner først bøkene som ikke er skrevet i den. Den sletter deretter tellerne som ikke er skrevet i den, men bare for en bassengforbindelse som ikke har noen bok igjen. En ført bok markerer fortsatt hver nøkkel mot telleren.
- En bok hvis figur ikke har flyttet seg, skrives ikke om, så en kortere periode kan også tømme gjeldende vinduets bok. Neste lesing åpner da en ny bok på gjeldende figur.
- Tilbakestillingen berører ikke en Redis -kvotebutikk. Der ender en bok med sitt vindu, eller utløper 60 dager etter siste skriving.
- Når leverandøren ikke sender noen tilbakestillingstid, ser et vindu som nullstiller og fyller på over det gamle tallet mellom to avlesninger ut som et høyere tall. Boken beholder den gamle grunnlinjen og merker.
- Avlesningene dateres etter den lokale klokken. Når den går foran leverandørens, eller en kilde rapporterer en tilbakestillingstid litt tidlig, kan boken dukke opp til den forskjellen tidlig.
- Veksten i det korte spennet deles av tokens som rutes i den. Det neste vinduets første lesning korrigerer det. Når den snudde boken ikke har noen tilbakestillingstid, trenger den korreksjonen et lavere tall som er minst to minutter nyere enn den sist brukte avlesningen.
- Forekomster som deler en Redis -butikk datoavlesninger med sine egne klokker, så hold disse klokkene synkronisert. Avlesninger av en forekomst hvis klokke går bak ser eldre ut og blir ignorert.
- Når ingen brukbar avlesning kommer etter den lagrede tilbakestillingstiden, håndheves ikke prosentandeler og prosenttak per nøkkel før en avlesning kommer tilbake. Uten tilbakestillingstid starter dette 15 minutter etter siste lesing som endret boken.
- På Redis butikken kan en bok som har vært tomgang i 60 dager utløpe mellom en skrivesjekk og den skrives. Den blir deretter gjenskapt ved en revisjon over 1, som er en gyldig tilstand.

---

## Abonnementsoppløser

Implementert i `src/lib/quota/planResolver.ts`.

Prioritet (høyest til lavest):

1. **Manuell databaseoverstyring** — tabellen `provider_plans`, per `connectionId`.
2. **Kjent katalog** — `src/lib/quota/planRegistry.ts` (kun data).
3. **Tomt abonnement** — ingen dimensjoner, manuell konfigurasjon kreves.

### Kjent katalog

| Leverandør            | Dimensjoner                                                   |
| --------------------- | ------------------------------------------------------------- |
| `codex`               | `percent/5h/100`, `percent/weekly/100`                        |
| `glm`                 | `tokens/5h` (limit=0, ukjent), `tokens/weekly`                |
| `minimax`             | `tokens/5h`, `tokens/weekly`                                  |
| `bailian`             | `percent/5h/100`, `percent/weekly/100`, `percent/monthly/100` |
| `kimi`                | `requests/hourly/1500`                                        |
| `alibaba`             | `requests/monthly/90000`                                      |
| `openai`, `anthropic` | Ingen standard — manuell konfigurasjon kreves                 |

---

## Rørledningsintegrasjon

### PRE krok (`open-sse/handlers/chatCore.ts`)

Kjører før oppstrømsutøveren, etter godkjennings- og policysjekker:

```
resolveComboTargets / handleSingleModel
  → enforceQuotaShare(apiKeyId, connectionId, provider, estimatedCost)
      → getQuotaStore().peek() per dimension
      → fairShare.decideFairShare()
      → if block → return 429 (buildErrorBody, Hard Rule #12)
      → if allow + deprioritize → set quotaSoftPenalty=true on candidate
  → executor.execute()
```

**Feil åpen** : hvis `enforceQuotaShare` kaster, tillates forespørselen med en `pino.warn` logg. Dette forhindrer en kvotemotorfeil fra å blokkere all trafikk.

**Når kapasiteten kommer tilbake.** Et avslag på nøkkelens andel eller ved bassengtaket ender med en av to setninger, i begge lånemodusene:

- `percent` vindu: `. The <window> window resets at <time>.` Klokken er tilbakestillingen leverandøren rapporterer.
- Tellbar enhet: `. Enough <window> usage is expected to clear by <time>.` Tiden er en øvre grense fra skyvevinduet, hvis nøkkelen ikke sender noe annet.

`<time>` er en ISO 8601 instant i UTC. Avslaget bærer deretter `Retry-After`: hele sekundene til det øyeblikket, pluss én. En klient som venter så lenge prøver på nytt maksimalt ett sekund etter øyeblikket. Når øyeblikket ikke er kjent, har avslaget verken setningen eller overskriften. Et absolutt tak-nekt har ingen av delene. Den offentlige koden forblir `quota_share_blocked`.

Et delingsavslag berører ikke den delte forbindelsen. Den setter ingen nedkjøling, ingen modelllås og ingen feil på leverandørbryteren, og de andre nøklene til bassenget blir stadig servert. Når hvert mål i en kombinasjon nekter nøkkelen for sin del, svarer kombinasjonen 429 uten å vente. Svaret har hintet som `Retry-After`. Innebyggingsbanen avslutter avslaget med samme setning og sender ingen `Retry-After`.

### POST -krok (rekordforbruk)

Etter et vellykket svar:

```
executor returns success
  → spendRecorder.recordConsumption(apiKeyId, connectionId, provider, actualCost)
      → getQuotaStore().consume() per dimension
      → fail-open: errors logged as pino.warn, never propagated to client
```

**Driftsnotat** : hvis `consume` mislykkes etter respons, teller den rullende telleren under. Metningssignalet fra leverandøren (f.eks. `anthropic-ratelimit-unified-5h-utilization`) korrigerer det globale estimatet ved neste forespørsel.

### Combo myk straff (`open-sse/services/combo.ts`)

Når `decision.deprioritize === true`:

```ts
if (candidate.quotaSoftPenalty) {
  score *= QUOTA_SOFT_DEPRIORITIZE_FACTOR; // default 0.7
}
```

Straffen brukes etter alle andre scoringsfaktorer. Det reduserer sannsynligheten for autokombinasjon for å velge en mettet nøkkel uten å blokkere den hardt.

---

## UI gjennomgang

### `/dashboard/costs/quota-share` — Hovedside for bassenger

Komponenter (alt i `src/app/(dashboard)/dashboard/costs/quota-share/`):

| Komponent              | Hensikt                                                                    |
| ---------------------- | -------------------------------------------------------------------------- |
| `QuotaConceptCard`     | Introduksjonskort som forklarer kvotedeling til nye brukere                |
| `CreatePoolModal`      | Opprett en ny kvotepool (connection + name + initial allocations)          |
| `PoolCard`             | Per-pool oppsummering: navn, tilknytning, tildelingstall                   |
| `DimensionBar`         | Stablet stolpe per dimensjon: hver nøkkels andel + global bruk             |
| `AllocationTable`      | Bord med konsumert, rettferdig andel, deficit/surplus, låneflagg           |
| `BurnRateChart`        | EMA burn-rate linjediagram (lat Recharts via `dynamic()`)                  |
| `EditAllocationsModal` | Rediger tildelingsvekter, tak og retningslinjer for en pool                |
| `BorrowModeField`      | Lånemodusvelger (`saturation` eller `consent`) i veiviseren                |
| `LendingBadge`         | Skrivebeskyttet merke på en nøkkel som låner ut, kun i `consent` bassenger |

Utlånsmerket viser prosentandelen og, når den er satt, fristen i UTC med sonen oppgitt. Den bedømmer fristen på tidspunktet for bruksøyeblikksbildet. En utløpt eller uleselig frist vises som `lending expired`.

Siden hekter:

- `usePools` — henter `GET /api/quota/pools` hver 30.
- `usePoolUsage` — henter `GET /api/quota/pools/[id]/usage` på forespørsel.
- `useLocalStoragePoolMigration` — kjører én gang på mount for å migrere eldre LS data.

Tastetrinnet til bassengveiviseren har en `Show usage by member to key holders` boks. Den angir bassengets `memberBreakdown` alternativ (se [Medlemsbruk](#member-usage) ). Under den advarer veiviseren om at noen som vet hvilken nøkkel som ble brukt, kan matche en stolpe til den nøkkelen. Med boksen huket av, står det slik når trinnet viser færre enn tre eller mer enn 20 nøkler, da stolpene da forblir skjult. Den teller nøklene i trinnet og kan ikke fortelle hvem av dem som kan sende forespørsler.

### `/dashboard/costs/quota-share/plans` — Leverandørplankonfig

- `ProviderPlanConfigClient.tsx`: rullegardin for å velge en leverandør, se løst plan (automatisk fra katalog eller manuell overstyring), og redigere dimensjoner.
- Endringer skrives til `PUT /api/quota/plans/[connectionId]`.
- Sletting går tilbake til katalog eller tom plan.

---

## Selvbetjeningskvote API (opt-in)

`GET /api/v1/me/quota/{provider}` (serveres også på `/v1/me/quota/{provider}`) lar en API -nøkkelholder lese, med sin egen nøkkel, hvor mye av et delt abonnement som er deres og hva som blokkerer dem. Ruten er et tynt skall over `src/server/selfService/quotaHandler.ts`; visningen er bygget av `src/lib/quota/selfView.ts` og responskontrakten er `src/shared/schemas/selfQuota.ts` (`SelfQuotaView` in `docs/openapi.yaml`).

### Aktivering og autentisering

- Funksjonsflagg `QUOTA_SELF_PANEL`, standard `false`. Mens den er av, får en forespørsel som når ruten 404. Med `REQUIRE_API_KEY=true` nekter klientens API policy en manglende eller ugyldig nøkkel med 401 før ruten kjører, uansett flagg. En forespørsel uten nøkkel, men en pålogget dashbordøkt, passerer denne policyen og får rutens eget svar. Flagget løser seg som alle andre flagg (dashboard eller REST overstyring, deretter miljøvariabelen med samme navn); se [`FEATURE_FLAGS.md`](../reference/FEATURE_FLAGS.md).
- Hvert bassengs visningsnavn og hver tidsplans etikett returneres til bassengets nøkkelinnehavere nøyaktig slik administratoren skrev dem. Før du slår på flagget, sjekk at de er i stand til å leses av disse nøkkelholderne.
- Nøkkelen leses kun fra overskrifter: `Authorization: Bearer <key>` eller `x-api-key: <key>`. Når begge sendes, brukes den første som validerer. En nøkkel i søkestrengen eller en informasjonskapsel ignoreres. Serverens miljønøkkel blir avvist (401).
- Nøkkelen trenger `self:usage` skopet (403 uten).
- Leverandørsegmentet trimmes, små bokstaver og sjekkes mot `^[a-z0-9][a-z0-9._-]{0,63}$` (ellers 400), deretter løst gjennom leverandørregisteret, slik at et alias som `cc` leser `claude` poolene. `claude` og `anthropic` leser de samme bassengene.

### Hva hver synlighet viser

| Synlighet  | Krever                                                                                  | Felter                                                                                                                                                                                                                                          |
| ---------- | --------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Egen andel | `self:usage`                                                                            | `pools[]` (ref, navn, leverandør, policy, vekt, cap), `dimensions[].yourShare`, `accounts[]` med `yourShare` (på et `percent` vindu uten `attributed` og `external`), `blocks`, `availableModels`, `expiresAt`, `apiBaseUrl`                    |
| Kontonivå  | `self:usage` + `self:account-quota`, og leverandøren i nøkkelens `sharedQuotaProviders` | legger til `dimensions[].total`, `accounts[].dimensions[].account` og `accounts[].modelWindows`, `attributed` og `external` på `yourShare` i et `percent` -vindu, og `members` på en pool med medlemsbruk på (se [medlemsbruk](#member-usage) ) |

- `sharedQuotaProviders` er en innstilling per nøkkel (`PUT /api/keys/[id]/self-service`): `null`, standarden, betyr at hver leverandør nøkkelen når; `[]` betyr ingen. Hvert bassengs `accountVisible` sier hvilken synlighet som gjaldt for den.
- Kontolinjer og modellvinduer vises kun for kontoer hvis tilkobling nøkkelen kan bruke. Når nøkkelen har en liste over tillatte tilkoblinger, beholder en konto utenfor den sin `Account N` oppføring uten `account` eller `modelWindows`. En tom liste betyr ingen begrensning, som for `/v1/me/status`. Poolsummen (`dimensions[].total`) avhenger ikke av den listen.
- To figurer vist med `self:usage` alene kommer fra andre nøklers bruk. Et planbudsjetts `exhausted` gjenspeiler forbruket av hver nøkkel under den tidsplanen. I en pool hvis vekter alle er null, er nøkkelens `weight` `100 / number of members`. Begge er hva håndhevelsen gjelder for nøkkelen.
- En pool identifiseres bare av `ref`, en ugjennomsiktig verdi bundet til den anropende nøkkelen. Visningsnavnet (`name`) er inkludert slik administratoren skrev det. En `ref` er avledet fra nøkkelen og bassenget med serverens API-nøkkelhemmelighet (`API_KEY_SECRET`). Klienter må ikke vedvare det: det endres hvis hemmeligheten roteres.
- Kontoer er oppført som `Account 1`, `Account 2`, … i poolrekkefølge. Ingen pool-ID, tilkoblings-ID, konto-e-post eller kontonavn returneres, og svaret går gjennom kontraktskjemaet, som sletter ethvert felt utenfor det.
- Tellelige enheter (`requests`, `tokens`, `usd`) rapporteres som bassenget kvoteporten håndhever: `limit` = plan limit × kontoer − bassenget, `fairShare` = vekt / 100 × `limit` (lik delt når hver vekt er 0), `consumed` = nøkkelens egen zq-teller, `remaining` quota = `fairShare` `consumed` gulv til 0.
- `blocks.schedules` viser nøkkelens tidsplanvinduer (`open`/`closed`, `blackout` eller `outside-window`, `retryAfterSeconds`, reservegulv og om vinduets budsjett er brukt); `blocks.modelCaps` viser sine timetak per modell med forbruk.
- En nøkkel utenfor hver pool hos leverandøren får 200 med `pools: []`; `availableModels` ( `qtSd/` -IDene nøkkelen ser i `/v1/models`), `expiresAt` og `apiBaseUrl` er fortsatt fylt ut.
- `apiBaseUrl` er `OMNIROUTE_PUBLIC_API_BASE_URL`, deretter `OMNIROUTE_PUBLIC_BASE_URL`, ellers `null`. Det er aldri forespørselens eget opphav.

### `status` og `reason`

| `status`      | Betydning                                                                                                                                                                                                                                                                                                                                          |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `ok`          | En aktuell lesning.                                                                                                                                                                                                                                                                                                                                |
| `stale`       | En bufret kontolesing merket som foreldet, eller en hvis tilbakestillingstid har gått siden den ble lest. Tall beholdes. Ett modellvindu hvis tilbakestillingstid har gått markerer hele `modelWindows` gruppen `stale`. For nøkkelens egen andel av et `percent` vindu: boken ble lest uten at en konto leste i portens cache for å bekrefte det. |
| `unavailable` | Ingen lesing; tallene er `null`, aldri `0`. `reason` sier hvorfor.                                                                                                                                                                                                                                                                                 |

| `reason`                          | Når                                                                                                                                            |
| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| `store_unavailable`               | Kvotebutikken kunne ikke leses, eller den kan ikke lese attribusjonsbøker.                                                                     |
| `percent_attribution_unavailable` | Nøkkelens egen andel av et `percent` vindu: ingen attribusjonsbok eksisterer ennå for den kontoen og vinduet, eller boken viser ikke nøkkelen. |
| `percent_window_ended`            | Nøkkelens egen andel av et `percent` vindu: boken tilhører et planvindu som er avsluttet.                                                      |
| `account_not_used_by_key`         | Nøkkelens egen andel av et `percent` vindu: Kontoens tilkobling er utenfor nøkkelens tillatte tilkoblinger. Boken er ikke lest.                |
| `window_not_reported`             | Providergrensebufferen har ingen lesing for det planvinduet.                                                                                   |
| `connection_lookup_failed`        | Kontoens tilkobling kunne ikke leses.                                                                                                          |
| `not_supported`                   | OmniRoute kan ikke lese bruksgrenser for kontoens leverandør.                                                                                  |
| `fetch_failed`                    | Ingen bufret lesing var brukbar, og oppdateringen av leverandørgrenser mislyktes.                                                              |
| `not_available`                   | Lesingen har ingen bruksvinduer, eller kontoen har ingen lesing i det hele tatt.                                                               |

Når kvotelageret ikke kan leses, er de butikkstøttede feltene til `blocks` (et tidsplanbudsjetts `exhausted`, en modellgrense `consumed` og `reached`) også `null`.

### Utlånssamtykke

`PATCH /api/v1/me/quota/{provider}` registrerer den oppringende nøkkelens eget samtykke for én gruppe. Den bruker flagget, overskriftene og leverandørreglene til `GET`. `self:usage` omfanget autoriserer denne skrivingen, selv om navnet er skrivebeskyttet.

```json
{
  "pool": "qpr_0123456789abcdef0123456789abcdef",
  "lendingPercent": 30,
  "lendingUntil": 1893456000000
}
```

- `pool` er `ref` som `GET` returnerer for den puljen.
- `lendingPercent` er et heltall fra 0 til 100. En verdi på 0 fjerner samtykket og fristen. En kropp med `lendingPercent` 0 aksepteres i begge modusene.
- `lendingUntil` er valgfritt: epoke millisekunder, eller `null` for ingen tidsfrist. Det må være i fremtiden og maksimalt 8640000000000000. En verdi under 100000000000 leses som sekunder og blir avvist.
- Ethvert annet felt avvises. En kropp lengre enn 4096 byte blir avvist. Avlesningen stopper ved den størrelsen, så en lengre kropp holdes aldri hel.

Kontrollene kjøres i rekkefølgen til denne tabellen. Hvert avslag bruker standard feiltekst med en fast melding. Et avslag fra en av disse sjekkene skriver ingenting.

| Status | Beskjed                                                                                            | Når                                                                      |
| ------ | -------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| 404    | `Not found`                                                                                        | `QUOTA_SELF_PANEL` flagget er av.                                        |
| 401    | `Valid API key required`                                                                           | Nøkkelen mangler eller er ugyldig, eller er serverens miljønøkkel.       |
| 403    | `API key lacks the self:usage scope`                                                               | Nøkkelen mangler `self:usage`.                                           |
| 400    | `Invalid provider`                                                                                 | Leverandørsegmentet er ugyldig.                                          |
| 429    | `Too many lending changes. Retry later.`                                                           | Nøkkelen passerte grensen. Svaret bærer `Retry-After`.                   |
| 400    | `Body must be { pool, lendingPercent, lendingUntil }. lendingPercent is an integer from 0 to 100.` | Brødteksten er ikke JSON, er for lang eller samsvarer ikke med skjemaet. |
| 400    | `lendingUntil must be a Unix time in milliseconds`                                                 | Fristen lyder som sekunder.                                              |
| 400    | `lendingUntil must be in the future`                                                               | Fristen er på eller før forespørselstidspunktet.                         |
| 404    | `Pool not found`                                                                                   | `ref` navngir ingen pool av denne nøkkelen for denne leverandøren.       |
| 403    | `Lending is not enabled for this pool`                                                             | Bassenget er i `saturation` modus og `lendingPercent` er over 0.         |
| 500    | `Failed to build quota view`                                                                       | Enhver annen feil. Årsaken er logget på serveren.                        |

Grensen er 20 forespørsler per 60 sekunder for hver nøkkel. Hver forespørsel som består leverandørsjekken teller, selv en som ble avslått senere eller en som ikke endrer noe. Den har sin egen teller, bortsett fra nøkkelens forespørselstakstgrense.

En forespørsel som endrer det lagrede samtykket skriver én `quota.pool.lending.updated` revisjonspost. Det navngir nøkkelen med de gamle og nye verdiene. Samme organ sendte to ganger skriver én gang og revisjoner én gang. Svaret er 200 med full `GET` visning, bygget etter skrivingen.

`GET` visningen rapporterer utlån som følger:

- Hvert basseng har `borrowMode` (`saturation` eller `consent`), og nøkkelens egne `lendingPercent` og `lendingUntil`.
- `lendingActive` er kun `true` i en `consent` pool, med en prosentandel over 0 og en frist som ikke er nådd.
- I en `consent` pool bærer hver tellbare `dimensions[].yourShare` `borrowAvailable`. Det er det nøkkelen kan bruke over sin andel nå, utlånt av de andre nøklene.
- `borrowAvailable` bruker portens formel. Den leser annenhver nøkkel, også mens nøkkelen er under sin del. For en `hard` nøkkel som er én ekstra lesning per annen nøkkel og tellbar dimensjon, parallelt.
- `borrowAvailable` er `null` for en `soft` eller `burst` nøkkel, og `null` når en lesing mislykkes.
- `borrowAvailable` er ett tall for alle andre nøkler sammen. I en pool med to nøkler er det den andre nøkkelens egen figur.
- `borrowAvailable` er ikke rapportert for `percent` vinduer eller i `accounts[]` ennå.
- I en `saturation` pool rapporterer visningen det lagrede samtykket med `lendingActive: false` og ingen `borrowAvailable`.

### Feil

Hvert svar på denne ruten, suksess eller feil, bærer `Cache-Control: no-store`. Et avslag som skjer før ruten kjører, bærer det ikke, for eksempel klientens API policys 401 eller IP filterets 403. Feil i ruten bruker standard feiltekst med en fast melding: 400 (ugyldig leverandør), 401 (manglende eller ugyldig nøkkel), 403 (mangler `self:usage` 5 ), 0lag (av) (f) (`Failed to build quota view`). 500 dekker enhver feil når forespørselen når ruten, inkludert selve nøkkeloppslaget; årsaken er logget på serveren og returneres aldri. Feilene i `PATCH` er oppført i [Lånesamtykke](#lending-consent).

### Begrensninger

- `remaining` er den delen av nøkkelens rettferdige andel den ikke har brukt. Det er ingen garanti. En nøkkel kan fortsatt serveres utover den mens bassenget har plass. Når bassengets totalsum når `limit`, blir hver nøkkel i bassenget nektet, uansett dens egen `remaining`, og en nøkkel uten `self:account-quota` kan ikke se denne summen.
- `remaining` tar ikke hensyn til allokeringens absolutte `cap`. Håndhevelse nekter nøkkelen når eget forbruk i et vindu på caps enhet når caps verdi.
- Baren på kontonivå kommer fra leverandørgrensebufferen og kan forsinke håndhevelsesavgjørelsen med noen minutter. En avlesning hvis tilbakestillingstid har gått, rapporteres som `stale`.
- Vinduer per modell (`modelWindows`) rapporteres kun for tilbydere som har en planvinduskartlegging: Claude og Codex i dag. For andre leverandører er `modelWindows` fortsatt til stede når kontodata vises, med en tom `windows` liste.
- Nøkkelens egen andel av et `percent` vindu er et estimat. Den kommer fra attribusjonsboken og har alle begrensninger som er oppført under «Prosentdimensjoner: attribusjon per nøkkel» ovenfor.
- `consumed` er antall håndhevelse sammenlignet med rettferdig andel. Det er `attributed` pluss `external`, nøyaktig. `attributed` er delen boken gir nøkkelen til tokens den rutet. `external` er nøkkelens del av kontoens bruk som bassengets nøkler ikke står for.
- Begge deler sendes bare når poolens `accountVisible` er sann: nøkkelen har `self:account-quota` og leverandøren er i sin `sharedQuotaProviders`. En nøkkel uten den får `consumed` alene, med samme `status` og `reason`.
- Med både deler og egen vekt kan en holder regne ut bruken som gjøres utenfor bassenget som lades til bassengets nøkler. En innehaver med kontoomfang ser allerede kontosummen.
- En nøkkel som ikke rutet noe i vinduet kan fortsatt lese dens eksterne ladning fra `consumed`, fordi dens tilskrevne del da er 0.
- For eksempel åpner en bok ved 0, med tastene A og B med vekt 50 hver. Nøkkel A ruter 900 000 tokens og nøkkel B 100 000. Kontoen når da 60 % av en grense på 100. Da er `attributed` 54 for nøkkel A og 6 for nøkkel B, og `external` er 0 for begge.
- Utsikten leser boken og skriver aldri dens tilstand. Den åpner ikke en bok, og den ber aldri leverandøren om en lesning. Med Redis butikken fjerner en lesing erstattede revisjonsfelt i bakgrunnen, slik portens avlesninger gjør.
- Andelen er kun `ok` mens portens cache holder en lesing av kontoen. Uten en er den `stale`, så i en pool uten nyere forespørsel vises den som muligens utdatert.
- Inntil en forespørsel går gjennom bassenget, er andelen utilgjengelig. Den forespørselen åpner boken, og kontoens tall i det øyeblikket teller som bruk utenfor bassenget.
- I en pool med flere kontoer bruker hver kontooppføring den kontoens egen bok og grensen for én konto. Håndheving skalerer begge sider etter antall kontoer, så andelen er den samme.
- Vinduer per modell har ingen del for nøkkelen. Boken inneholder ingen data per modell.
- Reservegulv i en tidsplan blir ikke evaluert av visningen: en tidsplan kan vises som `open` mens en forespørsel avvises med grunn `schedule-reserve`.
- Når to grupper med samme nøkkel deler en tilkobling, bruker håndhevelsen en av dem, og visningen viser begge.
- Det er ingen grense per adresse på mislykkede nøkkelforsøk: bak en omvendt proxy kan innringere dele én adresse (det avhenger av om videresendte klientadresser er klarert), så en lockout kan nekte ruten til hver nøkkelinnehaver. Med `REQUIRE_API_KEY=true` nektes en ugyldig nøkkel av klientens API -policy før ruten kjører, med denne policyens 401-kropp i stedet for denne rutens.

### Medlemsbruk

En administrator kan la nøkkelinnehavere se hvordan bruken av et vindu fordeler seg mellom bassengets medlemmer. Alternativet er bassengets `memberBreakdown`, av som standard. Det er satt i bassengveiviseren eller med `PATCH /api/quota/pools/{id}`. `GET /api/quota/pools` og `GET /api/quota/pools/{id}` rapporterer det.

En dimensjon av visningen har bare `members` når alle disse holder:

- bassengets alternativ er på
- bassenget har maksimalt 20 tildelte nøkler, og minst tre av dem kan sende forespørsler: aktive, ikke opphevet, ikke utestengt og ikke utløpt
- bassengets `accountVisible` er sann: nøkkelen har `self:account-quota` og leverandøren er i sin `sharedQuotaProviders`
- i et `percent` vindu er kontoens tilkobling en nøkkelen kan bruke
- nøkkelens egen andel av vinduet ble lest: dens `status` er ikke `unavailable`

Ellers er `members` fraværende. Det er aldri en tom liste.

- Hver skive er `{ slot, consumed, isYou }`. Svarskjemaet avviser enhver annen egenskap på en skive, og en liste med mer enn 20 skiver. Skiver er oppført i sporrekkefølge.
- Det er ett stykke per tildelt nøkkel, inkludert en nøkkel som ikke lenger kan sende forespørsler. Et medlem uten bruk viser en reell null.
- Spor 1 er alltid den spørrende nøkkelen, med `isYou` sant. De andre spornumrene er rangeringer av en nøkkelhash. Den er tastet med `API_KEY_SECRET` og dekker bassenget, spørringsnøkkelen og medlemmet.
- Så tallene står ikke på linje mellom innehavere. For én holder forblir de de samme mellom besøkene. De kan endres når en nøkkel blir med eller forlater bassenget, eller når den hemmeligheten roteres.
- På et tellbart vindu er en skive medlemmets teller i kvotebutikken, den samme telleren som sin egen `consumed`.
- På et `percent` vindu er en skive medlemmets `attributed` del, fra samme bok lest som nøkkelens egen del. Bruk utenfor bassenget deles aldri i skiver. Den ladningen er delt etter vekt, så skiver som bar den ville vise vektene.
- Hver visning leser én verdi per annet medlem og tellbart vindu, parallelt. På et `percent` vindu koster skivene ingen lesning utover aksjens egen boklest. Når en verdi ikke kan leses, har det vinduet ingen `members`, og nøkkelens egen del forblir.
- Alternativet og antallet brukbare nøkler leses én gang per pool, og kun for en nøkkel som kan se kontodata. En sviktende lesing av alternativet eller antall brukbare nøkler slår av stolpene for det bassenget. Serveren logger en advarsel, og resten av visningen bygges.

Stolpene har ingen navn eller id. De forteller fortsatt en nøkkelinnehaver ting om de andre medlemmene:

- Holdere kan fortsatt matche skiver etter verdiene deres.
- En stabil nummerering lar en innehaver følge ett medlem over tid.
- Antall skiver viser hvor mange nøkler som er tildelt i bassenget.
- I en pool med tre nøkler kan noen som vet hva en nøkkel brukte, fortelle hva den siste nøkkelen brukte.
- Når et basseng faller under tre brukbare nøkler, forsvinner stolpene. Visninger tatt tidligere viser fortsatt hva hvert medlem brukte.
- På et tellbart vindu kan totalsummen minus skivene vise bruken av nøkler som ikke lenger er tildelt.
- Et medlem som viser null på en konto og bruker på en annen kan vise hvilket medlem som bruker hvilken konto.
- I en tellbar pool med `hard` policyen, antyder en skive som slutter å vokse med et medlems rettferdige andel på det medlemmets vekt.

### Bruksserie (`GET /api/v1/me/usage`)

`GET /api/v1/me/usage?range=<range>` (også servert på `/v1/me/usage`) returnerer bruken og kostnadene for ringenøkkelens egne forespørsler: totaler, én oppføring per UTC dag, per dag og modell, per modell og per leverandør. Den deler flagget, autentiseringsreglene, `self:usage` omfanget, `Cache-Control: no-store` og feiloppførselen til kvoteruten ovenfor. Nøkkelen kontrolleres før `range`. Feilene er 400 (`Invalid range`), 401, 403, 404 og 500 (`Failed to build usage`).

- `range` er en av `1d`, `7d`, `30d` (standard) eller `90d`. Enhver annen verdi, en tom verdi eller en gjentatt parameter er en 400. Settet stopper ved `90d` for å begrense kostnaden for et anrop. Visningen leser bare rå brukshistorikk, aldri de daglige sammendragene, som ikke har noen nøkkel.
- Rader velges av anropsnøkkelens ID. Nøkkelnavnkolonnen matches aldri, og rader registrert uten nøkkel-ID telles aldri.
- Å bygge en serie kjører fem grupperte spørringer over nøkkelens rader i vinduet. Den bygde serien gjenbrukes i 60 sekunder per tast og rekkevidde, og en gjenbrukt samtale kjører ingen. Dens `generatedAt` gir dens alder.
- Vinduet slutter når serien er bygget. En rad stemplet senere, for eksempel ved klokkeskjevhet, regnes ikke med.
- `coverage.retentionDays` er operatørens oppbevaringsinnstilling for rå brukshistorikk (`retention.usageHistory` i databaseinnstillingene). `coverage.truncatedByRetention` er sant når det forespurte området er lengre enn den innstillingen. Den sammenligner de to tallene og sjekker ikke om rader faktisk mangler.
- Leverandøren returneres som registrert for nøkkelens egne forespørsler. Modell er det registrerte navnet etter dens siste `/`, og rader er gruppert etter den. En kombinasjonsforespørsel hvis hvert mål ble avvist, registreres med ruteetiketten som leverandør (kombinasjonsnavnet, `auto` eller `combo`) og modellstrengen klienten sendte. Andre avslåtte forespørsler, for eksempel av en åpen effektbryter, en modellnedkjøling eller et kvoteparkert skip, beholder målleverandøren og modellen.
- I tillegg til antall og kostnader, har svaret gjennomsnittlig ventetid, suksessrater og tidspunktene for første og siste forespørsel.
- `byModel` viser de 50 leverandør-og-modell-parene med flest forespørsler. Med flere par blir ikke oppføringene `summary`, og `summary.uniqueModels` teller hver registrerte modellstaving. `byModelTruncated` er da sant, og en modell hvis par faller på begge sider av kuttet viser deltotaler.
- To kostnader er rapportert. `costUsd` er den fakturerte kostnaden, slik bruksanalysen viser det. Flatrate abonnementsleverandører, som Claude Code-planen, teller $0 der. `listPriceUsd` er samme bruk priset til listepris, inkludert abonnement. En forespørsel hvis modell ikke har noen prisrad, teller dens lagrede kostnad: en kostnad leverandøren rapporterte, eller en som ble beregnet da forespørselen ble registrert. Bare en forespørsel uten noen av delene teller 0, uten markør, så en totalsum kan være delvis.
- Svarkontrakten er `src/shared/schemas/selfUsage.ts` (`SelfUsageSeries` in `docs/openapi.yaml`).

### Selvbetjeningsside

Med `QUOTA_SELF_PANEL` på er `/quota/{provider}` en offentlig side. En nøkkelholder skriver inn en API nøkkel der og ser nøkkelens bassenger for leverandøren. Hvert basseng viser ett kort per bassengvindu, med bassengets bruk for alle og nøkkelens egen andel. Hver konto i bassenget har sine egne kort, med kontoens bruk og nøkkelens andel. Kontoens bruk vises bare når nøkkelen kan se kontodata. Siden viser også grensene per modell for hver konto og nøkkelens egen bruk. Et varsel vises når en tidsplan blokkerer nøkkelen akkurat nå. Et kort viser hver enkelt hette på nøkkelen med dens bruk, og markerer de som er nådd. `{provider}` er en leverandør-ID eller dens alias (`/quota/claude`, `/quota/cc`). En ukjent leverandør, og hver `/quota/*` bane mens flagget er av, svarer 404. Pooler på en tilpasset OpenAI- eller Anthropic-kompatibel node har ingen side. API svarer fortsatt for dem.

Siden har ingen økt. Nøkkelen sendes bare i `Authorization` overskriften til `GET /api/v1/me/quota/{provider}`, `PATCH /api/v1/me/quota/{provider}` og `GET /api/v1/me/usage`, aldri i en URL. En nøkkel serveren godtar beholdes i fanens `sessionStorage`. Med "Husk på denne enheten" beholdes den i `localStorage` i stedet, og "Glem nøkkel" fjerner den fra begge. En nøkkel serveren avviser fjernes fra lagringen.

En pool i `consent` modus viser et utlånskort. Der setter nøkkelinnehaveren en hel prosentandel fra 0 til 100 av nøkkelens ledige andel for å låne ut. Innehaveren velger også hvor lenge samtykket varer: til det slås av, 1 time, 8 timer, 24 timer, 7 dager eller 30 dager. En varighet teller fra lagringstidspunktet. Mens en frist er i kraft, kan innehaveren holde den i stedet. Hvis denne fristen går før Lagre, sender kortet ingenting og ber om et annet valg. Med 0% sendes ingen frist. Kortet viser den lagrede fristen med navn på tidssonen. Et samtykke hvis frist er utløpt, vises som avsluttet.

For en `hard` nøkkel viser kortet også, per bassengvindu, hvilke andre nøkler som låner ut til nøkkelen akkurat nå. Hver rad er én figur for alle andre nøkler sammen. I en pool med to nøkler er det den andre nøkkelens egen figur. Et tall som visningen ikke rapporterer, leses som ikke tilgjengelig, ikke som null. For en `soft` eller `burst` nøkkel sier kortet at ingen tall gjelder.

En pool i `saturation` modus hvis nøkkel lagrer en prosentandel over 0 viser kun et uttak. Det står at den lagrede prosenten ikke har noen effekt der. Uttak-knappen sender 0 uten frist. En pool i `saturation` modus med en lagret 0 viser ingen utlånskort. Etter en lagring forblir et kort som den returnerte visningen ikke lenger trenger, med meldingen til sidens visning endres igjen.

Ingenting lagres før innehaveren trykker på Lagre eller Trekk ut. Hvert trykk sender en `PATCH /api/v1/me/quota/{provider}` forespørsel, og et annet trykk sender ingenting mens den første venter. Kroppen bærer bassengets ugjennomsiktige `ref` fra utsikten, prosentandelen og fristen. Svaret er den gjenoppbygde kvotevisningen, og siden viser den uten andre lesing. Når to lagringer overlapper hverandre, leser siden kvoten én gang etter siste svar. Siden oppbevarer ikke samtykket i nettleserlagring.

En avvist endring er forklart på kortet med en tekst valgt fra HTTP statusen. Feilteksten leses ikke. En 401 sier at nøkkelen ikke ble akseptert og laster inn kvoten på nytt. En 403 sier at bassenget ikke tar utlånsendringer, og en 404 sier at bassenget er borte. Begge tilbyr en knapp som laster inn kvoten på nytt. Et 400 eller et annet 4xx-svar ber innehaveren om å sjekke prosenten og fristen. En 429 ber innehaveren om å vente, med sekundene av `Retry-After` når svaret gir dem. Et 5xx-svar, en 408 eller en nettverksfeil sier at endringen kanskje ikke er lagret, og beholder de innskrevne verdiene. Et svar utenfor kontrakten laster kvoten på nytt. En mislykket lagring fjerner ikke nøkkelen av seg selv. Når gjenopplastingen etter at den blir nektet, fjerner siden nøkkelen som på alle nektet lesing.

Når en nøkkel er akseptert, viser siden også et "Sett opp verktøyene dine"-kort med tre faner. "Claude Code" gir `env` blokken for `~/.claude/settings.json`. "Shell" gir de samme variablene som `export` linjer. "Claude Desktop" gir verdiene for tredjeparts slutningsvinduet. Modellene er kvotedelingsmodellene nøkkelen kan kalle for den leverandøren. Når ingen slik liste følger med nøkkelen, slår blokken på gateway-modelloppdagelse i stedet. Gateway-adressen er den offentlige API opprinnelsen serveren rapporterer (`OMNIROUTE_PUBLIC_API_BASE_URL`, deretter `OMNIROUTE_PUBLIC_BASE_URL`). Når ingen av dem er angitt, viser kortet en plassholder og ber innehaveren om å spørre administratoren. Nøkkelen vises som en plassholder. "Inkluder min nøkkel" legger hele nøkkelen i teksten på skjermen og i det en kopieringsknapp kopierer. Det varer til boksen er tømt, nøkkelen er glemt eller erstattet, eller siden er igjen. Kortet sender ingen forespørsel og tilbyr ingen filnedlasting.

En lesing av API markerer `stale` vises som muligens utdatert. En lesing den markerer `unavailable` vises med sin grunn, aldri som null.

På prosentplaner trekker siden nøkkelens egen andel når API rapporterer det. Den sier at tallet er et estimat og navngir de to delene. Grenser per modell viser kun kontoen.

Når et vindu har `members`, viser kortet også en stolpe med ett segment per medlem, i sporrekkefølge. Spør-tastens segment bruker aksentfargen. De andre segmentene går gjennom temaets diagramfarger. En tekstforklaring viser hvert segment med sin verdi, så ingenting avhenger av farge. Segmenter er merket `You` eller `Member N`, der N er sporet.

### Dedikert port for siden

`QUOTA_PANEL_PORT` åpner en andre lytter som kun betjener selvbetjeningssiden. Den er av med mindre variabelen er satt. `QUOTA_PANEL_HOST` er bindingsadressen og er standard til `127.0.0.1`.

Lytteren videresender disse banene til hovedporten og svarer 404 for annenhver vei:

| Sti                                                                      | Serverer                          |
| ------------------------------------------------------------------------ | --------------------------------- |
| `/quota/{provider}`                                                      | Siden                             |
| `/api/v1/me/quota/{provider}`, `/v1/me/quota/{provider}`                 | Kvotevisningen siden leser        |
| `/api/v1/me/usage`, `/v1/me/usage`                                       | Bruksserien siden leser           |
| `/_next/static/`                                                         | Skript, stiler og fonter i bygget |
| `/favicon.ico`, `/favicon.svg`, `/icon-512.png`, `/apple-touch-icon.png` | Ikoner                            |

`GET` og `HEAD` videresendes uten kropp. En forespørsel med en kropp videresendes også: en `PATCH` av kvotevisningsbanen, som siden sender for å lagre et utlånsvalg. Enhver annen metode svarer 404, bortsett fra en CONNECT forespørsel, hvis forbindelse er lukket uten svar. Enhver annen forespørsel som erklærer et organ, svarer 404 og forbindelsen er stengt. Oppgraderingsforespørsler avvises og forbindelsen deres er stengt. En bane med et punktsegment eller en fragmentmarkør nektes, som på API porten. Det samme er et forespørselsmål med et tegn utenfor utskrivbar ASCII. Et råkontrolltegn i målet besvares 400 av HTTP parseren, før denne portens egen sjekk. Be om overskrifter som rammeverket reserverer til eget bruk ikke videresendes: navn som begynner med `x-middleware-`, `x-invoke-`, `x-nextjs-`, `x-now-` eller `x-next-`, og navnene `x-matched-path` og `next-resume`. Forespørselen videresendes uten dem. Dashbordet, påloggingssiden, management API og slutningsrutene kan ikke nås gjennom denne porten.

`PATCH` må ha `Content-Type: application/json`, uten parameter eller kun med `charset=utf-8`. Den må ha én `Content-Length` fra 1 til 4096, skrevet som vanlige sifre, og ingen `Transfer-Encoding`. En `PATCH` som bryter en av disse reglene svarer 404. Noen misformede lengder, for eksempel en signert eller en gjentatt, blir besvart 400 av HTTP parseren før denne portens egen sjekk. Porten leser de deklarerte bytene før den kontakter hovedporten, og venter maksimalt 5 sekunder på dem. En kropp som ikke er komplett innen da, svarer 404 og forbindelsen er stengt. Ingenting når hovedporten i så fall, eller når klienten går først. Porten videresender nøyaktig de deklarerte bytene, med samme `Content-Length`. Byte etter dem leses som neste forespørsel på tilkoblingen. En TLS omvendt proxy foran må videresende `Content-Length` og må ikke dele forespørselsteksten på nytt. Hovedporten sjekker API nøkkelen i `Authorization` overskriften, som for `GET`.

404-kroppen er `{"error":"not_found","message":"Not found."}`. Et mislykket relé svarer 502 (`api_bridge_unavailable`) eller 504 (`api_bridge_timeout`) uten `detail` felt.

Lytteren leser ikke `QUOTA_SELF_PANEL`, og den slår ikke på siden. Mens flagget er av, svarer siden og dens API 404 på hovedporten, og lytteren videresender svaret.

Under utviklingsserveren (`next dev`) blir ikke siden interaktiv gjennom denne porten. Utviklings-hot-reload-kontakten er en oppgraderingsforespørsel, og porten avslår det. Bruk hovedporten mens du utvikler.

Porten serverer vanlig HTTP og siden sender API nøkler. Behold standard bindingsadressen og sett en omvendt proxy med TLS foran den. En annen bindingsadresse enn loopback logger denne meldingen:

```text
[Quota Panel] Bound to <host>. This port serves plain HTTP and the page sends API keys. Put a TLS reverse proxy in front of it.
```

En loopback-peer som ikke sender noen videresendingshode, teller som lokal på hovedporten. Så en proxy på samme vert må sende `X-Forwarded-For`. En proxy på en privat adresse er klarert for den overskriften bare med `OMNIROUTE_TRUST_PROXY=private` (eller `lan`). Enhver annen peer rapporteres av adressen til tilkoblingen, og videresendingshodene den sendte blir slettet.

Lytteren har maksimalt 256 tilkoblinger om gangen. En klient har 10 sekunder på å sende forespørselshodene og 30 sekunder på å sende hele forespørselen. En tilkobling som holdes i live lukkes etter ca. 5 sekunder. En forbindelse uten aktivitet på 60 sekunder er stengt. Disse verdiene er faste. Sett også tilkoblings- og hastighetsgrenser på omvendt proxy foran. En omvendt proxy foran bør holde sine inaktive oppstrømsforbindelser i mindre enn 5 sekunder, eller ikke gjenbruke dem. Reléet til hovedporten bruker oppstrøms tidsavbrudd for API porten (`API_BRIDGE_*`).

Lytteren starter også når `API_PORT` ikke er stilt inn. `QUOTA_PANEL_PORT` må være en port fra 1 til 65535, kun skrevet med sifre. Den må avvike fra dashbordporten og API porten. Mens live WebSocket serveren er på, må den også avvike fra `LIVE_WS_PORT` (standard 20132). Enhver annen verdi åpner ingenting og logger en advarsel. En advarsel om en avvist verdi gir variabelen navn og gjentar ikke verdien. En port som allerede er i bruk åpner ingenting og logger denne advarselen:

```text
[Quota Panel] Port <port> is already in use. The quota panel port stays off.
```

Med `OMNIROUTE_BASE_PATH` sett forventer lytteren hver vei over under det prefikset. Bruk samme `OMNIROUTE_BASE_PATH` ved byggetid og under kjøretid. Skriv den med en innledende skråstrek og ingen etterfølgende skråstrek, for eksempel `/omniroute`. En annen form, inkludert `/` og `/omniroute/`, forlater porten med en advarsel, selv om konstruksjonen godtar disse formene. Det samme gjør en basisbane hvis første segment navngir en applikasjonsrute: `api`, `v1`, `v1beta`, `_next`, `quota`, `dashboard`, `docs`, `login`, `codex`, `responses`, `anthropic`, `openai`, `v0` eller `connect`, i alle fall.

Begrensninger:

- `/quota/{provider}/` med en etterfølgende skråstrek svarer 404 på denne porten.
- Tjenestearbeideren og nettappmanifestet serveres ikke på denne porten.
- Et tilpasset favorittikonsett i dashbordet vises ikke på denne porten.
- Ikoner vises ikke når applikasjonen kjører under en basisbane.
- Porten snakker vanlig HTTP/1.1.
- En binding som mislykkes prøves ikke på nytt før prosessen starter på nytt.
- Lytteren har ingen tilkobling eller hastighetsgrense per klientadresse.
- Beholderoppsett dekkes ikke av denne delen.

---

## Miljøvariabler

| Variabel                             | Misligholde   | Beskrivelse                                                         |
| ------------------------------------ | ------------- | ------------------------------------------------------------------- |
| `QUOTA_STORE_DRIVER`                 | `sqlite`      | Driver å bruke: `sqlite` eller `redis`                              |
| `QUOTA_STORE_REDIS_URL`              | _(tømme)_     | Redis URL, f.eks. `redis://localhost:6379`                          |
| `QUOTA_SATURATION_THRESHOLD`         | `0.5`         | 0..1; `>= threshold` aktiverer streng modus                         |
| `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` | `1000`        | Tokens som forklarer maksimalt ett punkt av et prosentplanvindu     |
| `QUOTA_SOFT_DEPRIORITIZE_FACTOR`     | `0.7`         | 0..1; multiplikator for soft-policy combo score                     |
| `QUOTA_CONSUMPTION_RETENTION_DAYS`   | `14`          | Dager før GC fjerner gamle `quota_consumption` bøtter               |
| `QUOTA_PANEL_PORT`                   | _(uaktivert)_ | Dedikert port for selvbetjeningssiden. Utkoblet betyr ingen lytter. |
| `QUOTA_PANEL_HOST`                   | `127.0.0.1`   | Bind adresse for den porten                                         |

DB innstillinger (`quotaStore.*`) overstyrer env vars.

---

## Feilsøking

### Redis er konfigurert, men kobler ikke til

Kontroller at `ioredis` er installert (`npm ls ioredis`), og at `QUOTA_STORE_REDIS_URL`
er tilgjengelig. Ved tilkoblingsfeil faller fabrikken tilbake til SQLite (logges på
`warn`-nivå).

### `peek` returnerer foreldede data / tillater ved feil

Hvis `peek` kaster en feil, behandler `enforceQuotaShare` resultatet som «tillat» (tillater ved feil).
Kontroller `pino`-loggene for oppføringer fra `quota:enforce` og `quota:factory` for å finne
den underliggende årsaken.

### Avvik i forbrukstelleren

Hvis den faktiske leverandørbruken avviker fra tellerne, er dette forventet — det
glidende vinduet med to perioder har en feilmargin på omtrent 1 % ved vindusgrensene, og `consume`
kjøres etter responsen uten å vente på resultatet. Metningssignalet (`saturationSignals.ts`)
leser den faktiske leverandørutnyttelsen med en TTL på 30 sekunder og justerer `globalUsedPercent`
tilsvarende.

### Puljen viser «ingen data» for forbruksrate

`computeBurnRate` krever minst 2 historiske målinger. Nye puljer uten tidligere
`consume`-kall viser `tokensPerSecond: 0` og `timeToExhaustionMs: null`.

---

## Migrering fra localStorage

Når `/dashboard/costs/quota-share` lastes inn for første gang, kontrollerer hooken `useLocalStoragePoolMigration`
følgende:

1. `localStorage.getItem("omniroute:quota-share:pools")` er ikke tom.
2. `GET /api/quota/pools` returnerer `[]` (databasen er tom).

Hvis begge er sanne, sender den hver eldre pool til `POST /api/quota/pools` samlet,
og fjerner deretter localStorage-nøkkelen. Migreringen er idempotent: betingelse 2 forhindrer
ny migrering.

---

## Intern strategiklassifisering

`quota-share` er en rutingstrategi **kun for intern bruk** (`INTERNAL_ROUTING_STRATEGY_VALUES` i
`src/shared/constants/routingStrategies.ts`). Den brukes utelukkende av systemgenererte
`qtSd/`-poolkombinasjoner og er bevisst utelatt fra `ROUTING_STRATEGY_VALUES`, slik at den aldri
vises som et brukervalg i brukergrensesnittet eller API-et.

---

## Testdekning

To lag med automatisert dekning sendes med kvotedelingsmotoren:

| Suite               | Kommando                                                               | Hva den dekker                                                                                                                                                                                                       |
| :------------------ | :--------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Enhet (29 tester)   | `node --import tsx/esm --test tests/unit/quota-share-strategy.test.ts` | DRR -planlegger, saturation gating, concurrency caps, fairShare math, backlog-kø                                                                                                                                     |
| Integrasjonsmatrise | `npm run test:combo:matrix`                                            | End-to-end-rutingsbeslutning gjennom den virkelige kombinasjonsrørledningen; DRR fairness + metningsnedprioritering via direkte sømmer (`registerQuotaFetcher`, `setLKGP`, `__setHeadroomSaturationFetcherForTests`) |

Integrasjonsmatrisen kjører i CI sammen med alle 22 offentlige strategier. Enhetspakken kan kjøres frittstående.

---

## DB Schema Summary

Tre tabeller lagt til av migreringer `078`, `079` og `085`:

- `quota_pools` + `quota_allocations` — pooldefinisjoner og tildelinger per nøkkel.
- `quota_consumption` — rullende 2-bøttetellere per `(apiKeyId, dimensionKey)`.
- `provider_plans` — manuelle leverandørplanoverstyringer (dimensjoner JSON per connectionId).

Alle tabeller lagt til via idempotente `CREATE TABLE IF NOT EXISTS` migreringer.

Samtykkede utlån legger til tre kolonner: `quota_allocations.lending_percent` (heltall, standard 0), `quota_allocations.lending_until` (epoke millisekunder, eller `NULL` uten tidsfrist) og `quota_pools.borrow_mode` (standard `saturation`). Migreringen legger bare til disse kolonnene og skriver ingen eksisterende rad.

Prosentattribusjonsboken legger til `quota_percent_ledger` (én rad per pool, konto og planvindu) og `quota_percent_ledger_tokens` (én token-teller per pool, konto og API nøkkel). `src/lib/db/quotaPercentLedger.ts` leser og skriver dem.
