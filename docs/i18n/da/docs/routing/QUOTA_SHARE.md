# Quota Sharing Engine (Dansk)

🌐 **Languages:** 🇺🇸 [English](../../../../routing/QUOTA_SHARE.md) · 🇪🇹 [am](../../../am/docs/routing/QUOTA_SHARE.md) · 🇸🇦 [ar](../../../ar/docs/routing/QUOTA_SHARE.md) · 🇦🇿 [az](../../../az/docs/routing/QUOTA_SHARE.md) · 🇧🇬 [bg](../../../bg/docs/routing/QUOTA_SHARE.md) · 🇧🇩 [bn](../../../bn/docs/routing/QUOTA_SHARE.md) · 🇧🇦 [bs](../../../bs/docs/routing/QUOTA_SHARE.md) · 🇨🇿 [cs](../../../cs/docs/routing/QUOTA_SHARE.md) · 🇩🇪 [de](../../../de/docs/routing/QUOTA_SHARE.md) · 🇬🇷 [el](../../../el/docs/routing/QUOTA_SHARE.md) · 🇪🇸 [es](../../../es/docs/routing/QUOTA_SHARE.md) · 🇪🇪 [et](../../../et/docs/routing/QUOTA_SHARE.md) · 🇮🇷 [fa](../../../fa/docs/routing/QUOTA_SHARE.md) · 🇫🇮 [fi](../../../fi/docs/routing/QUOTA_SHARE.md) · 🇫🇷 [fr](../../../fr/docs/routing/QUOTA_SHARE.md) · 🇮🇪 [ga](../../../ga/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [gu](../../../gu/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [ha](../../../ha/docs/routing/QUOTA_SHARE.md) · 🇮🇱 [he](../../../he/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [hi](../../../hi/docs/routing/QUOTA_SHARE.md) · 🇭🇷 [hr](../../../hr/docs/routing/QUOTA_SHARE.md) · 🇭🇺 [hu](../../../hu/docs/routing/QUOTA_SHARE.md) · 🇦🇲 [hy](../../../hy/docs/routing/QUOTA_SHARE.md) · 🇮🇩 [id](../../../id/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [ig](../../../ig/docs/routing/QUOTA_SHARE.md) · 🇮🇹 [it](../../../it/docs/routing/QUOTA_SHARE.md) · 🇯🇵 [ja](../../../ja/docs/routing/QUOTA_SHARE.md) · 🇬🇪 [ka](../../../ka/docs/routing/QUOTA_SHARE.md) · 🇰🇭 [km](../../../km/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [kn](../../../kn/docs/routing/QUOTA_SHARE.md) · 🇰🇷 [ko](../../../ko/docs/routing/QUOTA_SHARE.md) · 🇱🇹 [lt](../../../lt/docs/routing/QUOTA_SHARE.md) · 🇱🇻 [lv](../../../lv/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [ml](../../../ml/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [mr](../../../mr/docs/routing/QUOTA_SHARE.md) · 🇲🇾 [ms](../../../ms/docs/routing/QUOTA_SHARE.md) · 🇲🇹 [mt](../../../mt/docs/routing/QUOTA_SHARE.md) · 🇲🇲 [my](../../../my/docs/routing/QUOTA_SHARE.md) · 🇳🇵 [ne](../../../ne/docs/routing/QUOTA_SHARE.md) · 🇳🇱 [nl](../../../nl/docs/routing/QUOTA_SHARE.md) · 🇳🇴 [no](../../../no/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [or](../../../or/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [pa](../../../pa/docs/routing/QUOTA_SHARE.md) · 🇵🇭 [phi](../../../phi/docs/routing/QUOTA_SHARE.md) · 🇵🇱 [pl](../../../pl/docs/routing/QUOTA_SHARE.md) · 🇵🇹 [pt](../../../pt/docs/routing/QUOTA_SHARE.md) · 🇧🇷 [pt-BR](../../../pt-BR/docs/routing/QUOTA_SHARE.md) · 🇷🇴 [ro](../../../ro/docs/routing/QUOTA_SHARE.md) · 🇷🇺 [ru](../../../ru/docs/routing/QUOTA_SHARE.md) · 🇱🇰 [si](../../../si/docs/routing/QUOTA_SHARE.md) · 🇸🇰 [sk](../../../sk/docs/routing/QUOTA_SHARE.md) · 🇸🇮 [sl](../../../sl/docs/routing/QUOTA_SHARE.md) · 🇷🇸 [sr](../../../sr/docs/routing/QUOTA_SHARE.md) · 🇸🇪 [sv](../../../sv/docs/routing/QUOTA_SHARE.md) · 🇰🇪 [sw](../../../sw/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [ta](../../../ta/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [te](../../../te/docs/routing/QUOTA_SHARE.md) · 🇹🇭 [th](../../../th/docs/routing/QUOTA_SHARE.md) · 🇹🇷 [tr](../../../tr/docs/routing/QUOTA_SHARE.md) · 🇺🇦 [uk-UA](../../../uk-UA/docs/routing/QUOTA_SHARE.md) · 🇵🇰 [ur](../../../ur/docs/routing/QUOTA_SHARE.md) · 🇺🇿 [uz](../../../uz/docs/routing/QUOTA_SHARE.md) · 🇻🇳 [vi](../../../vi/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [yo](../../../yo/docs/routing/QUOTA_SHARE.md) · 🇨🇳 [zh-CN](../../../zh-CN/docs/routing/QUOTA_SHARE.md) · 🇹🇼 [zh-TW](../../../zh-TW/docs/routing/QUOTA_SHARE.md)

---

> **Dokumentreference**: `docs/routing/QUOTA_SHARE.md`
> Del af gruppe B (plan 16 + 22).

---

## Oversigt

Kvotedelingsmotoren fordeler en udbyders tidsbaserede kvote (f.eks. Codex'
5-timersvindue, Kimi 1500 req/h) retfærdigt på tværs af flere API-nøgler, der
deler den samme forbindelse.

**Problem, den løser:** OmniRoute videresender mange API-nøgler gennem den samme
konto hos upstream-udbyderen. Uden delingslogik kan en pludselig belastning fra
nøgle A opbruge udbyderens kvote for hele timen, så nøgle B og C blokeres, indtil
vinduet nulstilles. Motoren forhindrer dette ved at:

1. Spore hver nøgles rullende forbrug pr. dimension (%, anmodninger, tokens, $).
2. Anvende en arbejdsbevarende algoritme til retfærdig fordeling: En nøgle må
   låne fra ubenyttede andele, så længe den globale pulje ikke er mættet.
3. Håndhæve resultatet i den kritiske sti (`chatCore.ts`), før anmodningen når
   upstream-eksekveringskomponenten.

---

## Algoritme: Fair-Share Work-Conserving

Implementeret i `src/lib/quota/fairShare.ts`.

### Tilstande

| Tilstand                                   | Mode        | Opførsel                                                       |
| ------------------------------------------ | ----------- | -------------------------------------------------------------- |
| `globalUsedPercent < saturationThreshold`  | **Gavmild** | Nøglen kan låne op til den globale grænse minus forbrugt i alt |
| `globalUsedPercent >= saturationThreshold` | **Streng**  | Håndhæv individuel fair andel strengt                          |

Standard `saturationThreshold = 0.5` (env `QUOTA_SATURATION_THRESHOLD`).

Disse to tilstande beskriver en pulje i standardlånetilstanden, `saturation`. En pulje i `consent` tilstand anvender altid de strenge regler, uanset mætningen. Se [Samtykkede udlån (tilvalg pr. pulje)](#consented-lending-per-pool-opt-in).

### Per-dimension beslutning

For hver aktiv dimension i poolen beregner motoren:

```
fairShareAllowed = poolLimit × (allocationWeight / 100)
consumed        = current rolling value for this key (from QuotaStore.peek)
remaining       = fairShareAllowed - consumed
```

For `percent` dimensioner kommer `consumed` fra tilskrivningsbogen i stedet (se [Procentdimensioner: tilskrivning pr. nøgle](#percent-dimensions-per-key-attribution) ).

Så:

- **`policy = hard`** : hvis `consumed > fairShareAllowed` og mode er streng →** blok** .
- **`policy = soft`** : hvis `consumed > fairShareAllowed` og mode er streng →** straffe** (nedprioriter i combo; aldrig hard-block).
- **`policy = burst`** : tillad, mens der er global frihøjde uanset rimelig andel.

### Cap absoluto

`capValue` + `capUnit` på en allokering er et hårdt loft uafhængigt af tilstand eller politik. Enhver dimension, hvor `consumed >= capValue` altid** blokke** anmodningen. For en `percent` cap er `consumed` kun den del, der tilskrives nøglen.

### Multidimensionskontrol

En anmodning blokeres, hvis** enhver** dimension i poolen ville blokere den. Dimensioner er uafhængige — en 5h% udmattelse påvirker ikke den ugentlige% dimension.

### Lån

I generøs tilstand kan en nøgle, hvis tildeling er underforbrugt, bruge overskud fra andre nøglers ikke-allokerede andele. Formlen er:

```
maxAllowed = globalLimit - consumedByOtherKeys
```

hvor `consumedByOtherKeys = consumedTotal - consumedByThisKey`. Teto global (pool `limit` for den dimension) er altid det hårde loft.

### Samtykkede udlån (tilvalg pr. pulje)

Hver pulje har en lånetilstand. `saturation` er standard og beholder reglerne ovenfor. I `consent` tilstand overfører en `hard` nøgle kun sin andel inden for den kapacitet, som andre nøgler har accepteret at udlåne. Administratoren indstiller tilstanden for hver pulje. Hver nøgleholder angiver sit eget samtykke gennem [udlånssamtykke](#lending-consent).

Et samtykke er en procentdel fra 0 til 100 og en valgfri deadline i epoke millisekunder. Nøglen låner den procentdel af sin ledige andel, mens deadline er i fremtiden.

For én dimension er `L` den effektive grænse: plangrænsen gange konti i puljen. Porten beregner for den anmodende nøgle:

```
share_k         = w_k / 100 × L
idle_k          = max(0, share_k − consumed_k)
lent            = Σ over the other keys of lend_k / 100 × idle_k
taken           = Σ over the other keys of max(0, consumed_k − share_k)
borrowAvailable = max(0, lent − taken)
```

`w_k` er nøglens vægt, eller `100 / n` for hver nøgle, når ingen vægt er over 0. `lend_k` er nøglens aktive procentdel, og 0, når dens deadline er udløbet. Den anmodende nøgles eget samtykke tæller aldrig. En `hard` nøgle afvises, når dens forbrug når sin andel plus `borrowAvailable`.

Kapacitet uden tildelingskrav (100 minus summen af vægtene) kan ikke udlånes. Ingen nøgle sagde ja til at låne den.

**Eksempel.** `L` er 1000.

| Nøgle | Vægt | Dele | Forbrugt | udlåner |
| ----- | ---- | ---- | -------- | ------- |
| EN    | 50   | 500  | 530      | 0%      |
| B     | 30   | 300  | 100      | 50%     |
| C     | 0    | 0    | 60       | 0%      |

- B låner 50% af sine ledige 200, hvilket er 100. C tog allerede 60 over sin andel. A må låne 40.
- A bliver serveret ved 530 og afvist, når dets forbrug når 540.
- Før C brugte noget, med A på eller under sin andel, kunne C låne 100.
- Før C brugte noget, med A på 530, kunne C låne 70.

**Nul vægt.** En nøgle med vægt 0 har en andel på 0. Den serveres kun, mens dens forbrug er under, hvad andre låner. Når ingen låner, bliver det afvist fra første anmodning.

**Deadlines.** Ingen baggrundsopgave udløber et samtykke. Hver anmodning sammenligner fristen med sin egen tid, og en frist svarende til den tid er udløbet. En gemt deadline, der ikke er et endeligt tal, eller er forbi den største dato, en `Date` kan holde, tæller som passeret.

**`soft` og `burst`.** Udlån begrænser dem ikke. En `soft` nøgle bliver deprioriteret, når den er forbi sin andel. En `burst` nøgle passerer, mens poolen har plads. Poolloftet afviser stadig hver nøgle, når poolens samlede beløb når sin grænse.

**Omkostninger på anmodningsstien.** En `saturation` pool læser intet mere end før. I en `consent` pulje læser en tællig dimension kun de andre nøgler for en `hard` nøgle på eller over dens andel, mens en anden nøgle udlåner. Det laver så én læsning pr. anden tast, parallelt. En mislykket læsning tæller som et forbrug på 0 for den pågældende nøgle. En `percent` dimension tilføjer ingen læsning, fordi tilskrivningsbogen indeholder alle nøgler.

**Redigering af en pool.** En redigering bevarer samtykket fra de nøgler, der bliver. Dette gælder for tildelingsredigeringer, gruppeomfattende udskiftninger og `ensure` opkald. En fjernet nøgle mister sit samtykke, og en nøgle tilføjet tilbage starter ved 0. Admin-ruterne returnerer hver nøgles samtykke og skriver det aldrig. Skifter en pulje tilbage til `saturation` bevarer alle gemte samtykker, hvilket ikke har nogen effekt i den tilstand. Skifter puljen til `consent` igen, genaktiveres de gemte samtykker, hvis deadline ikke er overskredet. En nøgleholder kan slette et gemt samtykke i begge tilstande.

**Opgradering.** Hvis kolonnerne `lending_percent` og `lending_until` allerede eksisterer, tilføjer migreringen kun `borrow_mode`, og lagrede procenter forbliver som de er. Hver pulje starter i `saturation` tilstand. Slå `consent` til pr. pulje i pool-guiden. Intet udledes af de lagrede værdier.

**Begrænsninger.**

- En långiver kan finde poolen ved loftet, før den bruger sin egen andel. Kapacitet, som andre har lånt, tæller med i puljens total.
- Checken kører før anmodningen og forbeholder sig intet. Samtidige anmodninger læser forbruget, før nogen registreres, så udlånt kapacitet kan bruges mere end én gang, begrænset af anmodningerne under flyvning. Deltjekket af `saturation` tilstand har samme egenskab.

---

## Tæller med glidende vindue

Implementeret i `src/lib/quota/sqliteQuotaStore.ts` og `redisQuotaStore.ts`.

To buckets pr. `(apiKeyId, dimensionKey)`:

- `curr`: aktuel bucket (`floor(nowMs / windowMs)`)
- `prev`: forrige bucket (`curr - 1`)

Effektiv rullende værdi:

```
effectiveBucketIndex = floor(nowMs / windowMs)
bucketStartMs        = effectiveBucketIndex × windowMs
elapsed              = nowMs - bucketStartMs
weight               = 1 - elapsed / windowMs

effective = prev × weight + curr
```

**Præcision**: ~99 % nøjagtig. Fejlen er højst 1 % af vinduets størrelse ved
grænsen mellem buckets (iboende i tilnærmelsen med 2 buckets).

### Samtidighed

SQLite-driver: En mutex i hukommelsen pr. `(apiKeyId | dimensionKey)`-nøgle
forhindrer en read-modify-write-race condition. Mønsteret svarer til
anti-thundering-herd-mønstret i `src/sse/services/auth.ts`.

Redis-driver: Lua EVAL-script til atomisk inkrementering — køres som en enkelt
Redis-kommando.

---

## Drivere

### SQLite (standard, 0-installation)

- Tabel: `quota_consumption` (se migrering `073_quota_pools.sql` / `074_quota_consumption.sql`).
- Bedst til installationer med én instans.
- Al persistens findes i den eksisterende OmniRoute SQLite-database (`DATA_DIR/storage.sqlite`).

### Redis (valgfri, flere instanser)

- Kræver npm-pakken `ioredis`.
- Tællere gemmes i Redis; metadata (puljer/tildelinger) gemmes stadig i SQLite.
- Bedst til installationer med flere replikaer, hvor tællere skal deles.

### Skift af driver

Via indstillingsgrænsefladen (`/dashboard/settings` → Kvotelager) eller via miljøvariabler:

```bash
QUOTA_STORE_DRIVER=redis
QUOTA_STORE_REDIS_URL=redis://localhost:6379
```

Databaseindstillingen har forrang frem for miljøvariabler. Hvis `driver=redis`, men URL'en mangler, eller
`ioredis` ikke er installeret, falder fabrikken tilbage til SQLite og logger en advarsel.

Rækkefølge for valg af driver:

1. Databaseindstillingen `quotaStore.driver`
2. Miljøvariablen `QUOTA_STORE_DRIVER`
3. Standard: `sqlite`

---

## Multi-Dimension

En pool kan have flere dimensioner. Hver dimension er uafhængig:

```ts
QuotaDimension {
  unit: "percent" | "requests" | "tokens" | "usd",
  window: "5h" | "hourly" | "daily" | "weekly" | "monthly",
  limit: number,  // global pool ceiling for this dimension
}
```

**Eksempel: Codex plan** (5h% + ugentligt%):

```json
[
  { "unit": "percent", "window": "5h", "limit": 100 },
  { "unit": "percent", "window": "weekly", "limit": 100 }
]
```

En anmodning skal opfylde alle dimensioner for at være tilladt.

### Procentdimensioner: tilskrivning pr. nøgle

En procentplan rapporterer et forbrugstal pr. konto og planvindue. Udbyderen giver ingen tæller pr. API nøgle.

For at opdele dette tal mellem nøgler fører hver pulje en tilskrivningsbog pr. konto og planvindue. `src/lib/quota/percentLedger.ts` holder bogens regler. `src/lib/quota/percentAttribution.ts` gør bogen til de tal, som håndhævelsen bruger. Resultatet er et estimat bygget ud fra de tokens, hver nøglerute.

#### Læsninger, der flytter bogen

Bogen flytter kun på udbyderens egen figur for det ønskede planvindue. Disse forbindelser rapporterer en:

| Udbyder                             | Planlæg vinduer |
| ----------------------------------- | --------------- |
| Claude, gennem en OAuth forbindelse | `5h`, `weekly`  |
| Codex                               | `5h`, `weekly`  |

Disse tæller ikke som en læsning:

- et svar, som udbyderklienten markerer som forældet
- et Claude vindue, hvis procentdel udbyderen ikke rapporterede
- et andet vindues figur, eller det værste tilfælde på tværs af vinduer
- hastighedsgrænse header fallback
- en mislykket læsning

Andre udbydere, inklusive Claude med en API nøgle, har ingen bog. Hver nøgle debiteres 0 på deres procentdimensioner, som før denne ændring.

En læsning deler 30-sekunders cache for mætningssignalet. En Claude -aflæsning er dateret med, hvornår tallet blev observeret i svaroverskrifter eller læst fra brugsslutpunktet, når det tidspunkt er kendt. Andre aflæsninger er dateret efter, hvornår denne cache-indgang blev bygget.

#### Hvad bogen gemmer

Hver registreret anmodning tilføjer sine tokens én gang til en tæller pr. pulje, konto og nøgle. En tæller vokser kun. Bogen indeholder tre ting:

- basislinjen: tallet, da bogen åbnede eller vinduet sidst vendte
- det sidst anvendte tal
- pr. nøgle, dens token-tæller i samme øjeblik, kaldet dens mærke

Bogen opdateres, når håndhævelsen eller brugsruten beregner tilskrivningen. Skrifter sammenlignes og sættes på et revisionsnummer. En forfatter, der taber genforsøg én gang på en ny læsning.

#### Hvordan en nøgles del beregnes

Hver nøgles del beregnes, når bogen læses. Væksten i figuren, siden grundlinjen er delt mellem nøglerne i forhold til de tokens, som hver er rutet siden dens mærke.

Together, disse tokens forklarer højst ét punkt af tallet pr. `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` -tokens (standard 1.000). Den vækst, de ikke forklarer, er ekstern. Grundlinjen er også ekstern.

For eksempel åbner en bog ved 0. Nøgle A dirigerer derefter 900.000 tokens og nøgle B ruter 100.000. Ved et tal på 60 er A's del 54 point og B's del er 6.

En tæller under nøglens mærke er genstartet og tæller fuldt ud. En nøgle uden et mærke, såsom en nøgle, der slutter sig til poolen midt i et vindue, tæller alle dens tokens. Et tal, der halter efter tokens, forårsager en fejl, der forsvinder ved næste læsning. Det akkumuleres ikke.

`QUOTA_PERCENT_MIN_TOKENS_PER_POINT` læses ved hver tilskrivning. En værdi, der ikke er et endeligt tal på mindst 1, falder tilbage til 1.000.

#### Hvordan en læsning ændrer bogen

Den første matchningsregel gælder:

1. **Ingen bog endnu:** læsningen åbner bogen. Dens figur er basislinjen, og hver tæller er markeret.
2. **Ældre læsning:** en aflæsning, der er dateret før den sidst anvendte, ignoreres. Det samme er en aflæsning, hvis nulstillingstid er mere end 30 minutter tidligere end den gemte.
3. **Nyt udbydervindue:** en nulstillingstid mere end 30 minutter senere end den gemte vender bogen. Figuren bliver basislinjen, og hver tæller markeres igen. Nøgler uden skranke forlader bogen.
4. **Afsluttet vindue:** en gemt nulstillingstid, der ikke er efter aflæsningens datatid, betyder, at vinduet er afsluttet. Læsningen vender bogen, uanset dens figur.
5. **Højere tal:** kun den sidste figur bevæger sig. Grundlinjen og mærkerne bliver.
6. **Samme figur:** figuren, basislinjen og mærkerne bliver. Der skrives kun en nulstillingstid, bogen mangler.
7. **Nederste tal:** et lavere tal anvendes aldrig som sådan. Det vender først bogen, når tre ting holder. Den er mindst to minutter nyere end den sidst anvendte aflæsning. Intet siger, at vinduet er det samme åbne. Det er mere end et point lavere.

Vinduet tæller som det samme åbne, når tre ting holder. Begge nulstillingstider er kendt. De er inden for 30 minutter fra hinanden. Den gemte er stadig foran læsningen. Et lavere tal inde i vinduet ændrer intet.

En nulstillingstid gemmes kun, mens den er forud for datatiden for den aflæsning, der bærer den. Et højere tal gemmer sin aflæsnings nulstillingstid, når denne er brugbar, og beholder den gemte ellers. Et lige tal registrerer kun sin læsnings nulstillingstid, når bogen ikke har nogen. Det ændrer intet andet. Et lavere tal, der ikke vender bogen, registrerer ingen nulstillingstid.

#### Når bogen er brugt

Efter en læsning bruges bogen, medmindre dens gemte nulstillingstid ikke er efter det aktuelle tidspunkt. Det tilfælde opstår, når en læsning, der er taget lige før nulstillingen, såsom en visning fra cachen, observeres lige efter den.

Uden en brugbar læsning bruges den lagrede bog kun, mens den stadig kan være det aktuelle vindues bog. Det gælder i to tilfælde:

- dens nulstillingstid er kendt og stadig forude
- den har ingen nulstillingstid, og den sidste aflæsning, der ændrede den, er højst 15 minutter gammel

Ellers tilskrives intet, som når der ikke er nogen bog. En bog, hvis gemte nulstillingstid er gået, debiteres aldrig.

#### Håndhævelse

En nøgles forbrug på en procentdimension er dens tildelte del plus en andel af den eksterne del. Den eksterne del bruger først kapaciteten ingen tildelingskrav (100 minus summen af vægtene). Kun det overskydende deles mellem nøglerne efter vægt.

Dette forbrug sammenlignes med nøglens rimelige andel som for enhver anden dimension. Strict mode starter stadig, når mætningssignalet når `QUOTA_SATURATION_THRESHOLD` (standard 0,5). Hvert tal skaleres efter den effektive grænse: grænsen pr. konto gange antallet af konti i puljen.

En absolut cap med `capUnit: "percent"` tæller kun den del, der tilskrives nøglen, skaleret på samme måde. Tag en grænse pr. konto på 100 og k konti. Et loft på N nås så, når nøglens del af serveringskontoens tal når N/k point. Hver konto kontrolleres mod sin egen bog. For eksempel, med to konti, nås et loft på 10 ved 5 point af en kontos tal.

Når butikken ikke kan læses, tilskrives intet, og hver nøgle debiteres 0 på den dimension. Når en bogskrivning mislykkes, bruger denne tilskrivning bogen, som den blev læst. En mislykket tokenskrivning efterlader denne anmodnings tokens ude af bogen. Ingen af disse fejl blokerer en anmodning.

I en `consent` pulje bruger udlånsformlen hver nøgles forbrug på procentdimensionen som beskrevet ovenfor. Når en anden nøgle udlåner, læses bogen én gang og tilskrives hver nøgle. Uden en brugbar bog bliver hver nøgle opkrævet 0. En nøgle med vægt passerer så, og en nøgle med vægt 0 passerer kun, når en anden nøgle udlåner.

#### Brugsrute

`GET /api/quota/pools/{id}/usage` rapporterer de samme tal gennem den samme funktion. En procentdimension har én indgang pr. poolforbindelse i `accounts`. Dens topniveau `consumedTotal` og `perKey` afspejler den første indgang.

Ruten anvender også den aktuelle læsning, så den kan fremføre bogen, som en anmodning gør. `internal + external` kan afvige fra `consumedTotal` når der ikke er nogen brugbar aflæsning, eller når et lavere tal ikke anvendes.

#### Opbevaring og opbevaring

Begge kvotebutikker holder bogen. På SQLite fjerner den automatiske databaseoprydning, når den er aktiveret, rækker, der ikke er opdateret i 60 dage. På Redis deler bøgerne og tællerne i en poolforbindelse én nøgle. Den udløber 60 dage efter dens sidste token-skrivning eller bogændring. En bog, der ikke ændrer sig, omskrives ikke, så afskæringen er sat over det længste planvindue. Den manuelle nulstilling af brugshistorik rydder også bøgerne om SQLite (se Begrænsninger).

#### Begrænsninger

- Al vækst i kontotallet siden basislinjen er delt af de tokens, hver nøgle har rutet siden da. Hvornår den vækst skete, betyder ikke noget.
- Så brug lavet uden for OmniRoute debiteres nøglerne op til hvad deres tokens tillader. Det inkluderer brug foretaget før en nøgles første anmodning om vinduet, når bogen allerede var åben.
- For eksempel hæver brug udenfor kontoen 60 point, mens ingen nøgleruter. En nøgle dirigerer derefter 30.000 tokens, og tallet når 60,6.
- Hvis bogen var åben før den brug, er nøglens del 30 point. Den bærer også 7,65 eksternt brug med fire nøgler med en vægt på 25.
- Hvis bogen åbnes efter denne brug, er de 60 punkter baseline. Nøglens del er 0,6 point, og den bærer 15 ekstern brug.
- En forespørgsel eller et besøg på brugsruten åbner bogen. Så om en sådan brug tæller som baseline afhænger af, hvornår bogen åbnede.
- Med standardgulvet hæver en nøgle, der dirigerer 60.000 tokens, mens brug udenfor, kontoen med 60 point og får alle 60 som sin egen del.
- Med gulvet på 50.000 er dens egen del 1,2 point. De andre 58.8 er eksterne og opladet efter vægt, ligesom enhver ekstern brug.
- Indstil `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` tæt på, hvad ét point koster på din plan. Udendørs brug omfatter trafik på samme konto fra nøgler uden for poolen.
- Et procentloft gælder i hver tilstand. En lukket nøgle kan afvises, mens kontoen er langt under mætningsgrænsen.
- Tag en hætte på 10 og 12 punkter til udendørs brug tidligere i vinduet. En nøgle, der ruter 20.000 tokens, afvises derefter med et kontotal på 12,4%.
- Opdelingen er et estimat efter tokenvolumen. En anmodning tæller som dens prompt-tokens plus dens færdiggørelsestokens. Cache-rabatter og modelpriser ændrer ikke på dette antal.
- En anmodning, der ikke ender med status 200, registrerer ingen tokens. Eksempler er en stream, som klienten afbryder forbindelsen, og en upstream-fejl, efter at brugen er blevet brugt.
- Den brug, en sådan anmodning forårsagede, debiteres de nøgler, der registrerede tokens, op til hvad deres tokens tillader. Resten er eksternt. Den bevæger sig ikke tilbage. Et svar, der rapporterer ingen token-brug, registrerer heller ingen tokens.
- Brugen af en igangværende anmodning kan dukke op i en anden aktiv nøgles del for hele anmodningen. Den flyttes kun tilbage, når anmodningen slutter med status 200.
- Brug allerede på kontoen, når en bog åbnes, tæller som eksternt. Dette dækker over en opgradering, en ny pulje og en ny konto. Brug i et nyt vindue før første læsning tæller også som eksternt.
- Hver nøgle starter med sin vægtandel af det pågældende forbrug, efter kapaciteten ingen tildelingskrav. Med én konto på 85 % og fem nøgler med vægt 20 starter hver med 17 af sine 20 brugte.
- I en pulje med flere konti påføres serveringskontoens tal på det summerede budget. Dette er uændret af bogen.
- Et lavere tal inde i et vindue, som udbyderen rapporterer som åbent, anvendes ikke. En nulstillingstid, der flyttes tilbage med mere end 30 minutter, behandles som en gammel aflæsning.
- I begge tilfælde beholder bogen sin tilstand, indtil den gemte nulstillingstid går. Derefter oplades bogen ikke, før en læsning vender den.
- Løsningen er den manuelle nulstilling af brugshistorik (`POST /api/settings/purge-usage-history`). Det rydder tilskrivningsbøgerne og deres token-tællere i SQLite databasen.
- `all` perioden rydder hver bog og tæller. En kortere periode rydder først de bøger, der ikke er skrevet i den. Den rydder derefter tællerne, der ikke er skrevet i den, men kun for en poolforbindelse, der ikke har nogen bog tilbage. En ført bog markerer stadig hver nøgle mod dens tæller.
- En bog, hvis figur ikke har flyttet sig, bliver ikke omskrevet, så en kortere periode kan også rydde det aktuelle vindues bog. Den næste læsning åbner så en frisk bog ved den aktuelle figur.
- Nulstillingen berører ikke en Redis -kvotebutik. Der ender en bog med sit vindue eller udløber 60 dage efter dens sidste skrivning.
- Når udbyderen ikke sender nogen nulstillingstid, ligner et vindue, der nulstiller og genopfylder over det gamle tal mellem to aflæsninger, et højere tal. Bogen beholder den gamle grundlinje og mærker.
- Aflæsninger dateres af det lokale ur. Når den løber forud for udbyderens, eller en kilde rapporterer en nulstillingstid lidt tidligt, kan bogen vise den forskel tidligt.
- Væksten i det korte spænd opdeles af de tokens, der føres i den. Det næste vindues første læsning retter det. Når den drejede bog ikke har nogen nulstillingstid, skal den korrektion have et lavere tal, der er mindst to minutter nyere end den sidst anvendte aflæsning.
- Forekomster, der deler en Redis -butiks datoaflæsninger med deres egne ure, så hold disse ure synkroniseret. Aflæsninger af en instans, hvis ur løber bagud, ser ældre ud og ignoreres.
- Når der ikke kommer nogen brugbar læsning efter den gemte nulstillingstid, håndhæves procentandele og procentgrænser pr. nøgle ikke, før en aflæsning vender tilbage. Uden en nulstillingstid starter dette 15 minutter efter den sidste læsning, der ændrede bogen.
- I Redis butikken kan en bog, der har været inaktiv i 60 dage, udløbe mellem en skribentcheck og dens udskrivning. Det genskabes derefter ved en revision over 1, hvilket er en gyldig tilstand.

---

## Abonnementsresolver

Implementeret i `src/lib/quota/planResolver.ts`.

Prioritet (højeste til laveste):

1. **Manuel tilsidesættelse i databasen** — tabellen `provider_plans`, pr. `connectionId`.
2. **Kendt katalog** — `src/lib/quota/planRegistry.ts` (kun data).
3. **Tomt abonnement** — ingen dimensioner; manuel konfiguration er påkrævet.

### Kendt katalog

| Udbyder               | Dimensioner                                                   |
| --------------------- | ------------------------------------------------------------- |
| `codex`               | `percent/5h/100`, `percent/weekly/100`                        |
| `glm`                 | `tokens/5h` (limit=0, ukendt), `tokens/weekly`                |
| `minimax`             | `tokens/5h`, `tokens/weekly`                                  |
| `bailian`             | `percent/5h/100`, `percent/weekly/100`, `percent/monthly/100` |
| `kimi`                | `requests/hourly/1500`                                        |
| `alibaba`             | `requests/monthly/90000`                                      |
| `openai`, `anthropic` | Ingen standard — manuel konfiguration er påkrævet             |

---

## Pipeline integration

### PRE krog (`open-sse/handlers/chatCore.ts`)

Kører før opstrøms eksekveren, efter godkendelses- og politiktjek:

```
resolveComboTargets / handleSingleModel
  → enforceQuotaShare(apiKeyId, connectionId, provider, estimatedCost)
      → getQuotaStore().peek() per dimension
      → fairShare.decideFairShare()
      → if block → return 429 (buildErrorBody, Hard Rule #12)
      → if allow + deprioritize → set quotaSoftPenalty=true on candidate
  → executor.execute()
```

**Fejl-åben** : hvis `enforceQuotaShare` kaster, tillades anmodningen igennem med en `pino.warn` log. Dette forhindrer en quota-motor-fejl i at blokere al trafik.

**Når kapaciteten vender tilbage.** Et afslag ved nøglens andel eller ved poolloftet ender med en af to sætninger i begge lånetilstande:

- `percent` vindue: `. The <window> window resets at <time>.` Klokken er den nulstilling, som udbyderen rapporterer.
- Tællbar enhed: `. Enough <window> usage is expected to clear by <time>.` Tiden er en øvre grænse fra det glidende vindue, hvis nøglen ikke sender andet.

`<time>` er en ISO 8601 instant i UTC. Afslaget bærer derefter `Retry-After`: hele sekunder indtil det øjeblik, plus én. En klient, der venter så længe, prøver igen højst et sekund efter øjeblikkeligt. Når tidspunktet ikke er kendt, bærer afslaget hverken sætningen eller overskriften. Et absolut afslag på loftet har ingen af delene. Den offentlige kode forbliver `quota_share_blocked`.

Et delingsafslag berører ikke den delte forbindelse. Den indstiller ingen nedkøling, ingen modellås og ingen udbyderafbryderfejl, og de andre nøgler til poolen bliver ved med at blive serveret. Når hvert mål i en kombination afviser nøglen for sin andel, svarer kombinationen 429 uden at vente. Dens svar bærer antydningen som `Retry-After`. Indlejringsstien afslutter sit afslag med den samme sætning og sender ingen `Retry-After`.

### POST krog (rekordforbrug)

Efter et vellykket svar:

```
executor returns success
  → spendRecorder.recordConsumption(apiKeyId, connectionId, provider, actualCost)
      → getQuotaStore().consume() per dimension
      → fail-open: errors logged as pino.warn, never propagated to client
```

**Driftsnote** : hvis `consume` mislykkes efter svar, tæller den rullende tæller under. Mætningssignalet fra udbyderen (f.eks. `anthropic-ratelimit-unified-5h-utilization`) korrigerer det globale estimat ved næste anmodning.

### Combo blød straf (`open-sse/services/combo.ts`)

Når `decision.deprioritize === true`:

```ts
if (candidate.quotaSoftPenalty) {
  score *= QUOTA_SOFT_DEPRIORITIZE_FACTOR; // default 0.7
}
```

Straffen pålægges efter alle andre scoringsfaktorer. Det sænker autokombinationssandsynligheden for at vælge en mættet nøgle uden at blokere den hårdt.

---

## UI gennemgang

### `/dashboard/costs/quota-share` — Hoved pools side

Komponenter (alle i `src/app/(dashboard)/dashboard/costs/quota-share/`):

| Komponent              | Formål                                                                  |
| ---------------------- | ----------------------------------------------------------------------- |
| `QuotaConceptCard`     | Introduktionskort, der forklarer kvotedeling til nye brugere            |
| `CreatePoolModal`      | Opret en ny kvotepulje (connection + name + initial allocations)        |
| `PoolCard`             | Per-pulje oversigt: navn, forbindelse, tildelingstal                    |
| `DimensionBar`         | Stablet bjælke pr. dimension: hver nøgles andel + globalt brug          |
| `AllocationTable`      | Bord med forbrugt, fair share, deficit/surplus, låneflag                |
| `BurnRateChart`        | EMA burn-rate linjediagram (doven Recharts via `dynamic()`)             |
| `EditAllocationsModal` | Rediger tildelingsvægte, lofter og politikker for en pulje              |
| `BorrowModeField`      | Lånetilstandsvælger (`saturation` eller `consent`) i guiden             |
| `LendingBadge`         | Skrivebeskyttet badge på en nøgle, der låner ud, kun i `consent` puljer |

Udlånsmærket viser procentdelen og, når den er sat, fristen i UTC med zonen angivet. Den bedømmer deadline på tidspunktet for brugsøjebliksbilledet. En udløbet eller ulæselig deadline vises som `lending expired`.

Siden kroger:

- `usePools` — henter `GET /api/quota/pools` hver 30.
- `usePoolUsage` — henter `GET /api/quota/pools/[id]/usage` efter behov.
- `useLocalStoragePoolMigration` — kører én gang på mount for at migrere ældre LS data.

Pool-guidens nøgletrin har en `Show usage by member to key holders` boks. Den indstiller puljens `memberBreakdown` indstilling (se [Medlemsbrug](#member-usage) ). Under den advarer guiden om, at en person, der ved, hvad en nøgle brugte, kan matche en bjælke med den pågældende nøgle. Med feltet afkrydset, står det sådan, når trinnet viser færre end tre eller mere end 20 nøgler, da søjlerne så forbliver skjulte. Den tæller nøglerne i trinnet og kan ikke fortælle, hvem af dem der kan fremsætte anmodninger.

### `/dashboard/costs/quota-share/plans` — Udbyder plan config

- `ProviderPlanConfigClient.tsx`: rullemenu for at vælge en udbyder, se løst plan (automatisk fra katalog eller manuel tilsidesættelse) og redigere dimensioner.
- Ændringer skrives til `PUT /api/quota/plans/[connectionId]`.
- Sletning vender tilbage til katalog eller tom plan.

---

## Selvbetjeningskvote API (tilvalg)

`GET /api/v1/me/quota/{provider}` (også serveret på `/v1/me/quota/{provider}`) lader en API -nøgleholder med deres egen nøgle læse, hvor meget af et delt abonnement der er deres, og hvad der blokerer dem. Ruten er en tynd skal over `src/server/selfService/quotaHandler.ts`; visningen er bygget af `src/lib/quota/selfView.ts`, og dens svarkontrakt er `src/shared/schemas/selfQuota.ts` (`SelfQuotaView` i `docs/openapi.yaml`).

### Aktivering og godkendelse

- Funktionsflag `QUOTA_SELF_PANEL`, standard `false`. Mens den er slået fra, får en anmodning, der når ruten, 404. Med `REQUIRE_API_KEY=true` afviser klientens API politik en manglende eller ugyldig nøgle med 401 før ruten kører, uanset flaget. En anmodning uden nøgle, men en logget på dashboard-session, passerer denne politik og får rutens eget svar. Flaget løses som alle andre flag (dashboard eller REST tilsidesættelse, derefter miljøvariablen af samme navn); se [`FEATURE_FLAGS.md`](../reference/FEATURE_FLAGS.md).
- Hver pools visningsnavn og hver tidsplans etiket returneres til poolens nøgleholdere nøjagtigt som administratoren skrev dem. Før du tænder for flaget, skal du kontrollere, at de er egnede til at blive læst af disse nøgleholdere.
- Nøglen læses kun fra overskrifter: `Authorization: Bearer <key>` eller `x-api-key: <key>`. Når begge sendes, bruges den første, der validerer. En nøgle i forespørgselsstrengen eller en cookie ignoreres. Serverens miljønøgle afvises (401).
- Nøglen skal bruge `self:usage` scope (403 uden).
- Udbydersegmentet trimmes, med små bogstaver og tjekkes mod `^[a-z0-9][a-z0-9._-]{0,63}$` (ellers 400), og løses derefter gennem udbyderregistret, så et alias som `cc` læser `claude` puljerne. `claude` og `anthropic` læser de samme puljer.

### Hvad hver synlighed viser

| Sigtbarhed  | Kræver                                                                             | Felter                                                                                                                                                                                                                                               |
| ----------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Egen andel  | `self:usage`                                                                       | `pools[]` (ref, navn, udbyder, politik, vægt, cap), `dimensions[].yourShare`, `accounts[]` med `yourShare` (på et `percent` vindue uden `attributed` og `external`), `blocks`, `availableModels`, `expiresAt`, `apiBaseUrl`                          |
| Kontoniveau | `self:usage` + `self:account-quota`, og udbyderen i nøglens `sharedQuotaProviders` | tilføjer `dimensions[].total`, `accounts[].dimensions[].account` og `accounts[].modelWindows`, `attributed` og `external` på `yourShare` i et `percent` vindue og `members` på en pulje med medlemsbrug slået til (se [medlemsbrug](#member-usage) ) |

- `sharedQuotaProviders` er en indstilling pr. nøgle (`PUT /api/keys/[id]/self-service`): `null`, standarden, betyder hver udbyder nøglen når; `[]` betyder ingen. Hver pools `accountVisible` siger, hvilken synlighed der gjaldt for den.
- Kontobjælker og modelvinduer vises kun for konti, hvis forbindelse nøglen kan bruge. Når nøglen har en liste over tilladte forbindelser, beholder en konto uden for den sin `Account N` post uden `account` eller `modelWindows`. En tom liste betyder ingen begrænsning, som for `/v1/me/status`. Den samlede pulje (`dimensions[].total`) afhænger ikke af den liste.
- To figurer vist med `self:usage` alene kommer fra andre nøglers brug. Et skemabudgets `exhausted` afspejler forbruget af hver nøgle under den tidsplan. I en pulje, hvis vægt alle er nul, er nøglens `weight` `100 / number of members`. Begge er, hvad håndhævelsen gælder for nøglen.
- En pulje identificeres kun af `ref`, en uigennemsigtig værdi bundet til den kaldende nøgle. Dens visningsnavn (`name`) er inkluderet, som administratoren skrev det. En `ref` er afledt af nøglen og puljen med serverens API-nøglehemmelighed (`API_KEY_SECRET`). Klienter må ikke fortsætte med det: det ændrer sig, hvis denne hemmelighed roteres.
- Konti er angivet som `Account 1`, `Account 2`, … i puljerækkefølge. Ingen pool-id, forbindelses-id, konto-e-mail eller kontonavn returneres, og svaret går gennem kontraktskemaet, som sletter ethvert felt uden for det.
- Tællbare enheder (`requests`, `tokens`, `usd`) rapporteres som den puljespand, som kvoteporten håndhæver: `limit` = plangrænse × konti i puljen, `fairShare` = vægt / 100 × `limit` (lige fordelt `consumed` når hver vægt er 0), `consumed` = nøglens egen zq tæller, `remaining` = `fairShare` −, gulvbelagt ved 0.
- `blocks.schedules` viser nøglens skemavinduer (`open`/`closed`, `blackout` eller `outside-window`, `retryAfterSeconds`, reservegulve, og om vinduets budget er brugt); `blocks.modelCaps` viser sine timelofter pr. model med forbrug.
- En nøgle uden for hver pulje hos udbyderen får 200 med `pools: []`; `availableModels` ( `qtSd/` id'erne, som nøglen ser i `/v1/models`), `expiresAt` og `apiBaseUrl` er stadig udfyldt.
- `apiBaseUrl` er `OMNIROUTE_PUBLIC_API_BASE_URL`, derefter `OMNIROUTE_PUBLIC_BASE_URL`, ellers `null`. Det er aldrig anmodningens egen oprindelse.

### `status` og `reason`

| `status`      | Mening                                                                                                                                                                                                                                                                                                                                                  |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `ok`          | En aktuel læsning.                                                                                                                                                                                                                                                                                                                                      |
| `stale`       | En cachelagret kontolæsning er markeret som forældet, eller en hvis nulstillingstid er gået, siden den blev læst. Tal opbevares. Et modelvindue, hvis nulstillingstid er gået, markerer hele `modelWindows` gruppen `stale`. For nøglens egen andel af et `percent` vindue: bogen blev læst uden at en konto læste i portens cache for at bekræfte det. |
| `unavailable` | Ingen læsning; tallene er `null`, aldrig `0`. `reason` siger hvorfor.                                                                                                                                                                                                                                                                                   |

| `reason`                          | Når                                                                                                                                            |
| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| `store_unavailable`               | Kvotebutikken kunne ikke læses, eller den kan ikke læse tilskrivningsbøger.                                                                    |
| `percent_attribution_unavailable` | Nøglens egen andel af et `percent` vindue: der eksisterer endnu ingen tilskrivningsbog for den konto og vindue, eller bogen viser ikke nøglen. |
| `percent_window_ended`            | Nøglens egen andel af et `percent` vindue: bogen tilhører et planvindue, der er afsluttet.                                                     |
| `account_not_used_by_key`         | Nøglens egen andel af et `percent` vindue: Kontoens forbindelse er uden for nøglens tilladte forbindelser. Dens bog er ikke læst.              |
| `window_not_reported`             | Provider-grænsecachen har ingen læsning for det planvindue.                                                                                    |
| `connection_lookup_failed`        | Kontoens forbindelse kunne ikke læses.                                                                                                         |
| `not_supported`                   | OmniRoute kan ikke læse brugsgrænser for kontoens udbyder.                                                                                     |
| `fetch_failed`                    | Ingen cachelagret læsning var brugbar, og opdatering af udbydergrænser mislykkedes.                                                            |
| `not_available`                   | Aflæsningen har ingen brugsvinduer, eller kontoen har slet ingen læsning.                                                                      |

Når kvotelageret ikke kan læses, er de butiksstøttede felter i `blocks` (et skemabudgets `exhausted`, en model caps `consumed` og `reached`) også `null`.

### Udlånssamtykke

`PATCH /api/v1/me/quota/{provider}` registrerer den kaldende nøgles eget samtykke for én pulje. Den bruger flag, overskrifter og udbyderregler for `GET`. `self:usage` omfanget tillader denne ene skrivning, selvom dens navn er skrivebeskyttet.

```json
{
  "pool": "qpr_0123456789abcdef0123456789abcdef",
  "lendingPercent": 30,
  "lendingUntil": 1893456000000
}
```

- `pool` er den `ref` som `GET` returnerer for den pulje.
- `lendingPercent` er et heltal fra 0 til 100. En værdi på 0 rydder samtykket og dets deadline. En krop med `lendingPercent` 0 accepteres i begge tilstande.
- `lendingUntil` er valgfrit: epoke millisekunder eller `null` uden deadline. Det skal være i fremtiden og højst 8640000000000000. En værdi under 100000000000 læses som sekunder og afvises.
- Ethvert andet felt afvises. En krop længere end 4096 bytes afvises. Aflæsningen stopper ved den størrelse, så en længere krop holdes aldrig hel.

Kontrollerne kører i rækkefølgen i denne tabel. Ethvert afslag bruger standardfejlteksten med en fast besked. Et afslag fra en af disse checks skriver intet.

| Status | Besked                                                                                             | Når                                                               |
| ------ | -------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| 404    | `Not found`                                                                                        | `QUOTA_SELF_PANEL` flaget er slukket.                             |
| 401    | `Valid API key required`                                                                           | Nøglen mangler eller er ugyldig, eller er serverens miljønøgle.   |
| 403    | `API key lacks the self:usage scope`                                                               | Nøglen mangler `self:usage`.                                      |
| 400    | `Invalid provider`                                                                                 | Udbydersegmentet er ugyldigt.                                     |
| 429    | `Too many lending changes. Retry later.`                                                           | Nøglen passerede sin grænse. Svaret bærer `Retry-After`.          |
| 400    | `Body must be { pool, lendingPercent, lendingUntil }. lendingPercent is an integer from 0 to 100.` | Brødteksten er ikke JSON, er for lang eller matcher ikke skemaet. |
| 400    | `lendingUntil must be a Unix time in milliseconds`                                                 | Fristen lyder som sekunder.                                       |
| 400    | `lendingUntil must be in the future`                                                               | Fristen er på eller før anmodningstidspunktet.                    |
| 404    | `Pool not found`                                                                                   | `ref` navngiver ingen pulje af denne nøgle for denne udbyder.     |
| 403    | `Lending is not enabled for this pool`                                                             | Puljen er i `saturation` tilstand, og `lendingPercent` er over 0. |
| 500    | `Failed to build quota view`                                                                       | Enhver anden fiasko. Dens årsag er logget på serveren.            |

Grænsen er 20 anmodninger pr. 60 sekunder for hver nøgle. Hver anmodning, der består udbyderkontrollen, tæller, selv en afvist senere eller en, der ikke ændrer noget. Den har sin egen tæller, bortset fra nøglens anmodningshastighedsgrænse.

En anmodning, der ændrer det gemte samtykke, skriver én `quota.pool.lending.updated` -revisionspost. Det navngiver nøglen med de gamle og nye værdier. Det samme organ sendte to gange skriver én gang og revision én gang. Svaret er 200 med den fulde `GET` visning, bygget efter skrivningen.

`GET` visningen rapporterer udlån som følger:

- Hver pulje bærer `borrowMode` (`saturation` eller `consent`), og nøglens egne `lendingPercent` og `lendingUntil`.
- `lendingActive` er kun `true` i en `consent` pulje, med en procentdel over 0 og en deadline, der ikke er nået.
- I en `consent` pulje bærer hver tællelig `dimensions[].yourShare` `borrowAvailable`. Det er, hvad nøglen kan bruge over sin andel nu, udlånt af de andre nøgler.
- `borrowAvailable` bruger portens formel. Den læser hver anden nøgle, også mens nøglen er under sin del. For en `hard` nøgle, der er én ekstra læsning pr. anden nøgle og tællelig dimension, parallelt.
- `borrowAvailable` er `null` for en `soft` eller `burst` nøgle og `null`, når en læsning mislykkes.
- `borrowAvailable` er ét tal for alle andre nøgler tilsammen. I en pulje med to nøgler er det den anden nøgles egen figur.
- `borrowAvailable` er ikke rapporteret for `percent` windows eller i `accounts[]` endnu.
- I en `saturation` pulje rapporterer visningen det lagrede samtykke med `lendingActive: false` og ingen `borrowAvailable`.

### Fejl

Hvert svar på denne rute, succes eller fejl, bærer `Cache-Control: no-store`. Et afslag, der sker før ruten kører, bærer det ikke, f.eks. klientens API politiks 401 eller IP -filterets 403. Fejl på ruten bruger standardfejlteksten med en fast besked: 400 (ugyldig udbyder), 401 (manglende eller ugyldig nøgle), 403 (mangler `self:usage`(5f ), 0 lag fra (`Failed to build quota view`)e). 500 dækker enhver fejl, når anmodningen når ruten, inklusive selve nøgleopslaget; dens årsag er logget på serveren og returneres aldrig. Fejlene i `PATCH` er angivet i [Udlånssamtykke](#lending-consent).

### Begrænsninger

- `remaining` er den del af nøglens rimelige andel, den ikke har brugt. Det er ikke en garanti. En nøgle kan stadig serveres ud over den, mens poolen har plads. Når puljens totalværdi når `limit`, afvises hver nøgle i puljen, uanset dens egen `remaining`, og en nøgle uden `self:account-quota` kan ikke se denne total.
- `remaining` tager ikke hensyn til allokeringens absolutte `cap`. Håndhævelse afviser nøglen, når dets eget forbrug i et vindue i hættens enhed når hættens værdi.
- Baren på kontoniveau kommer fra udbydergrænsecachen og kan forsinke håndhævelsesbeslutningen med et par minutter. En aflæsning, hvis nulstillingstid er gået, rapporteres som `stale`.
- Vinduer pr. model (`modelWindows`) rapporteres kun for udbydere, der har en plan-vindue-mapping: Claude og Codex i dag. For andre udbydere er `modelWindows` stadig til stede, når kontodata vises, med en tom `windows` liste.
- Nøglens egen andel af et `percent` vindue er et skøn. Den kommer fra tilskrivningsbogen og har alle begrænsninger, der er angivet under "Procentdimensioner: tilskrivning pr. nøgle" ovenfor.
- `consumed` er antallet af håndhævelse sammenlignet med den rimelige andel. Det er `attributed` plus `external`, præcis. `attributed` er den del, som bogen giver nøglen til de tokens, den dirigerede. `external` er nøglens del af kontoens brug, som puljens nøgler ikke tager højde for.
- Begge dele sendes kun, når poolens `accountVisible` er sand: nøglen har `self:account-quota`, og udbyderen er i sin `sharedQuotaProviders`. En nøgle uden den får `consumed` alene, med den samme `status` og `reason`.
- Med både dele og egen vægt kan en holder regne ud den brug, der gøres uden for poolen, der oplades til poolens nøgler. En indehaver med kontoomfanget ser allerede kontototalen.
- En nøgle, der ikke dirigerede noget i vinduet, kan stadig læse dens eksterne ladning fra `consumed`, fordi dens tilskrevne del så er 0.
- For eksempel åbner en bog ved 0, med tasterne A og B med en vægt på 50 hver. Nøgle A fører 900.000 tokens og nøgle B 100.000. Kontoen når så 60 % af en grænse på 100. Så er `attributed` 54 for nøgle A og 6 for nøgle B, og `external` er 0 for begge.
- Udsigten læser bogen og skriver aldrig dens tilstand. Den åbner ikke en bog, og den beder aldrig udbyderen om en læsning. Med Redis -butikken fjerner en læsning erstattede revisionsfelter i baggrunden, som portens læsninger gør.
- Andelen er kun `ok`, mens portens cache indeholder en aflæsning af kontoen. Uden en er den `stale`, så i en pulje uden nogen nylig anmodning vises den som muligvis forældet.
- Indtil en anmodning går gennem puljen, er andelen ikke tilgængelig. Den anmodning åbner bogen, og kontoens tal på det tidspunkt tæller som brug uden for puljen.
- I en pulje med flere konti bruger hver kontopost den pågældende kontos egen bog og grænsen på én konto. Håndhævelse skalerer begge sider efter antallet af konti, så andelen er den samme.
- Vinduer pr. model bærer ingen del for nøglen. Bogen opbevarer ingen data pr. model.
- Reservegulve i en tidsplan evalueres ikke af visningen: en tidsplan kan vises som `open` mens en anmodning afvises med årsagen `schedule-reserve`.
- Når to puljer med den samme nøgle deler en forbindelse, anvender håndhævelsen en af dem, og visningen viser begge.
- Der er ingen begrænsning pr. adresse på mislykkede nøgleforsøg: bag en omvendt proxy kan opkaldere dele én adresse (det afhænger af, om videresendte klientadresser er tillid til), så en lockout kan afvise ruten til hver nøgleholder. Med `REQUIRE_API_KEY=true` afvises en ugyldig nøgle af klientens API -politik, før ruten kører, med denne policys 401 body i stedet for denne rutes.

### Medlemsbrug

En administrator kan lade nøgleindehavere se, hvordan et vindues brug fordeler sig mellem puljens medlemmer. Indstillingen er poolens `memberBreakdown`, deaktiveret som standard. Det er indstillet i pool-guiden eller med `PATCH /api/quota/pools/{id}`. `GET /api/quota/pools` og `GET /api/quota/pools/{id}` rapporterer det.

En dimension af visningen bærer kun `members`, når alle disse holder:

- poolens mulighed er slået til
- puljen har højst 20 tildelte nøgler, og mindst tre af dem kan lave anmodninger: aktive, ikke tilbagekaldt, ikke forbudt og ikke udløbet
- poolens `accountVisible` er sand: nøglen har `self:account-quota`, og udbyderen er i sin `sharedQuotaProviders`
- i et `percent` vindue er kontoens forbindelse en, nøglen kan bruge
- nøglens egen andel af det vindue blev læst: dens `status` er ikke `unavailable`

Ellers er `members` fraværende. Det er aldrig en tom liste.

- Hver skive er `{ slot, consumed, isYou }`. Svarskemaet afviser enhver anden egenskab på et udsnit og en liste med mere end 20 udsnit. Skiver er opført i rækkefølge.
- Der er et udsnit pr. allokeret nøgle, inklusive en nøgle, der ikke længere kan foretage anmodninger. Et medlem uden brug viser et rigtigt nul.
- Slot 1 er altid den spørgende nøgle, med `isYou` sand. De andre slotnumre er rækker af en nøglehash. Den er tastet med `API_KEY_SECRET` og dækker poolen, spørgenøglen og medlemmet.
- Så tallene står ikke på linje mellem indehavere. For en indehaver forbliver de de samme mellem besøgene. De kan ændre sig, når en nøgle slutter sig til eller forlader poolen, eller når den hemmelighed roteres.
- På et tælleligt vindue er en skive medlemmets tæller i kvotebutikken, den samme tæller som dens egen `consumed`.
- På et `percent` vindue er en skive medlemmets `attributed` del, fra samme bog læst som nøglens egen andel. Brug uden for poolen opdeles aldrig i skiver. Denne ladning er opdelt efter vægt, så skiver, der bar den, ville vise vægtene.
- Hver visning læser en værdi pr. andet medlem og tælleligt vindue parallelt. På et `percent` vindue koster skiverne ingen læsning ud over aktiens egen læste bog. Når en værdi ikke kan læses, har det vindue ingen `members`, og nøglens egen share forbliver.
- Indstillingen og antallet af anvendelige nøgler læses én gang pr. pulje, og kun for en nøgle, der muligvis kan se kontodata. En fejllæsning af indstillingen eller antallet af brugbare nøgler slår søjlerne fra for den pågældende pulje. Serveren logger en advarsel, og resten af visningen bygges.

Barerne bærer ingen navne eller id'er. De fortæller stadig en nøgleindehaver ting om de andre medlemmer:

- Indehavere kan stadig matche skiver efter deres værdier.
- En stabil nummerering lader en indehaver følge et medlem over tid.
- Antallet af skiver viser, hvor mange nøgler der er tildelt i puljen.
- I en pulje med tre nøgler kan en, der ved, hvad en nøgle brugte, fortælle, hvad den sidste nøgle brugte.
- Når en pool falder til under tre brugbare nøgler, forsvinder søjlerne. Visninger taget tidligere viser stadig, hvad hvert medlem brugte.
- På et tælleligt vindue kan den samlede pulje minus skiverne vise brugen af nøgler, der ikke længere er tildelt.
- Et medlem, der viser nul på én konto og bruger på en anden, kan vise, hvilket medlem der bruger hvilken konto.
- I en tællelig pulje med `hard` politikken antyder en skive, der holder op med at vokse ved et medlems rimelige andel, på det pågældende medlems vægt.

### Brugsserie (`GET /api/v1/me/usage`)

`GET /api/v1/me/usage?range=<range>` (også serveret på `/v1/me/usage`) returnerer brugen og prisen for den kaldende nøgles egne anmodninger: totaler, én indtastning pr. UTC dag, pr. dag og model, pr. model og pr. udbyder. Det deler flaget, autentificeringsreglerne, `self:usage` omfanget, `Cache-Control: no-store` og fejladfærden for kvoteruten ovenfor. Nøglen kontrolleres før `range`. Fejl er 400 (`Invalid range`), 401, 403, 404 og 500 (`Failed to build usage`).

- `range` er en af `1d`, `7d`, `30d` (standardindstillingen) eller `90d`. Enhver anden værdi, en tom værdi eller en gentaget parameter er en 400. Sættet stopper ved `90d` for at afgrænse prisen for et opkald. Visningen læser kun rå brugshistorik, aldrig de daglige oversigter, som ikke har nogen nøgle.
- Rækker vælges af den kaldende nøgles id. Kolonnen med nøglenavn matches aldrig, og rækker, der er optaget uden et nøgle-id, tælles aldrig.
- Opbygning af en serie kører fem grupperede forespørgsler over nøglens rækker i vinduet. Den indbyggede serie genbruges i 60 sekunder pr. tast og rækkevidde, og et genbrugt opkald kører ingen. Dens `generatedAt` giver dens alder.
- Vinduet slutter, når serien er bygget. En række, der er stemplet senere, f.eks. med urskævhed, tælles ikke med.
- `coverage.retentionDays` er operatørens rå brugshistorik-opbevaringsindstilling (`retention.usageHistory` i databaseindstillingerne). `coverage.truncatedByRetention` er sandt, når det anmodede område er længere end denne indstilling. Den sammenligner de to tal og kontrollerer ikke, om der faktisk mangler rækker.
- Udbyder returneres som registreret for nøglens egne anmodninger. Model er det registrerede navn efter dets sidste `/`, og rækker er grupperet efter det. En kombinationsanmodning, hvis hvert mål blev afvist, registreres med routingetiketten som udbyder (kombinationsnavnet, `auto` eller `combo`) og den modelstreng, som klienten sendte. Andre afviste anmodninger, for eksempel af en åben afbryder, en modelafkøling eller et kvoteparkeret spring, beholder måludbyderen og modellen.
- Udover tæller og omkostninger, har svaret gennemsnitlig latenstid, succesrater og tidspunkterne for den første og sidste anmodning.
- `byModel` lister de 50 udbyder-og-model-par med flest anmodninger. Med flere par tæller dens indtastninger ikke op til `summary`, og `summary.uniqueModels` tæller hver registreret modelstavning. `byModelTruncated` er da sandt, og en model, hvis par falder på begge sider af snittet, viser delvise totaler.
- Der indberettes to omkostninger. `costUsd` er den fakturerede pris, som brugsanalysen viser det. Fastpris-abonnementsudbydere, såsom Claude Code-planen, tæller $0 der. `listPriceUsd` er den samme brug prissat til listepris, abonnementer inkluderet. En anmodning, hvis model ikke har nogen prisrække, tæller dens lagrede omkostninger: en omkostning, som udbyderen rapporterede, eller en, der blev beregnet, da anmodningen blev registreret. Kun en anmodning uden nogen af dem tæller 0, uden markør, så en total kan være delvis.
- Svarkontrakten er `src/shared/schemas/selfUsage.ts` (`SelfUsageSeries` i `docs/openapi.yaml`).

### Selvbetjeningsside

Med `QUOTA_SELF_PANEL` tændt er `/quota/{provider}` en offentlig side. En nøgleholder skriver en API nøgle der og ser nøglens puljer for udbyderen. Hver pulje viser et kort per puljevindue, med poolens brug for alle og nøglens egen andel. Hver konto i puljen har sine egne kort med kontoens brug og nøglens andel. Kontoens brug vises kun, når nøglen muligvis kan se kontodata. Siden viser også grænserne pr. model for hver konto og nøglens eget brug. En meddelelse vises, når en tidsplan blokerer nøglen lige nu. Et kort viser hver nøgle-hætte pr. model med dens brug og markerer dem, der er nået. `{provider}` er et udbyder-id eller dets alias (`/quota/claude`, `/quota/cc`). En ukendt udbyder, og hver `/quota/*` sti, mens flaget er slået fra, svarer 404. Puljer på en brugerdefineret OpenAI- eller Anthropic-kompatibel node har ingen side. API svarer stadig for dem.

Siden har ingen session. Nøglen sendes kun i `Authorization` headeren af `GET /api/v1/me/quota/{provider}`, `PATCH /api/v1/me/quota/{provider}` og `GET /api/v1/me/usage`, aldrig i en URL. En nøgle, som serveren accepterer, opbevares i fanens `sessionStorage`. Med "Husk på denne enhed" holdes den i `localStorage` i stedet, og "Glem nøgle" fjerner den fra begge. En nøgle, som serveren afviser, fjernes fra lageret.

En pulje i `consent` tilstand viser et lånekort. Der sætter nøgleholderen en hel procentdel fra 0 til 100 af nøglens ledige andel til udlån. Indehaveren vælger også, hvor længe samtykket varer: indtil det slukkes, 1 time, 8 timer, 24 timer, 7 dage eller 30 dage. En varighed tæller fra tidspunktet for lagring. Mens en frist er gældende, kan indehaveren holde den i stedet. Hvis denne frist passerer før Gem, sender kortet intet og beder om et andet valg. Med 0% sendes ingen deadline. Kortet viser den gemte deadline med dens tidszone navngivet. Et samtykke, hvis frist er overskredet, vises som afsluttet.

For en `hard` nøgle viser kortet også, pr. puljevindue, hvilke andre nøgler, der kan låne til nøglen lige nu. Hver række er én figur for alle andre nøgler tilsammen. I en pulje med to nøgler er det den anden nøgles egen figur. Et tal, som visningen ikke rapporterer, læses som ikke tilgængeligt, ikke som nul. For en `soft` eller `burst` nøgle siger kortet, at der ikke gælder noget tal.

En pulje i `saturation` tilstand, hvis nøgle gemmer en procentdel over 0, viser kun en udbetaling. Der står, at den gemte procentdel ikke har nogen effekt der. Dens tilbagetrækningsknap sender 0 uden deadline. En pulje i `saturation` tilstand med et gemt 0 viser intet lånekort. Efter en lagring forbliver et kort, som den returnerede visning ikke længere har brug for, med sin besked, indtil sidens visning ændres igen.

Intet gemmes, før indehaveren trykker på Gem eller Udtag. Hvert tryk sender en `PATCH /api/v1/me/quota/{provider}` anmodning, og et andet tryk sender intet, mens det første afventer. Kroppen bærer poolens uigennemsigtige `ref` fra udsigten, procentdelen og deadline. Svaret er den genopbyggede kvotevisning, og siden viser den uden anden læsning. Når to lagringer overlapper hinanden, læser siden kvoten én gang efter det sidste svar. Siden opbevarer ikke samtykket i browserens opbevaring.

En afvist ændring forklares på kortet med en tekst valgt fra HTTP statussen. Fejlteksten læses ikke. En 401 siger, at nøglen ikke blev accepteret og genindlæser kvoten. En 403 siger, at puljen ikke tager udlånsændringer, og en 404 siger, at puljen er væk. Begge tilbyder en knap, der genindlæser kvoten. Et 400 eller et andet 4xx-svar beder indehaveren om at kontrollere procentdelen og deadline. En 429 beder indehaveren om at vente med sekunderne af `Retry-After`, når svaret giver dem. Et 5xx-svar, et 408 eller en netværksfejl siger, at ændringen muligvis ikke er blevet gemt, og beholder de indtastede værdier. Et svar uden for kontrakten genindlæser kvoten. En mislykket lagring fjerner ikke nøglen af sig selv. Når genindlæsningen efter den er afvist, fjerner siden nøglen som ved enhver afvist læsning.

Når en nøgle er accepteret, viser siden også et "Set up your tools"-kort med tre faner. "Claude Code" giver `env` blokken for `~/.claude/settings.json`. "Shell" giver de samme variabler som `export` linjer. "Claude Desktop" giver værdierne for dets tredjeparts inferensvindue. Modellerne er de kvotedelingsmodeller, nøglen kan kalde for den pågældende udbyder. Når der ikke følger en sådan liste med nøglen, aktiverer blokken gateway-modelopdagelse i stedet. Gateway-adressen er den offentlige API oprindelse, som serveren rapporterer (`OMNIROUTE_PUBLIC_API_BASE_URL`, derefter `OMNIROUTE_PUBLIC_BASE_URL`). Når ingen af dem er indstillet, viser kortet en pladsholder og beder indehaveren om at spørge administratoren. Nøglen vises som en pladsholder. "Inkluder min nøgle" sætter hele nøglen i teksten på skærmen og i hvad en kopiknap kopierer. Det varer indtil kassen er ryddet, nøglen er glemt eller udskiftet, eller siden er tilbage. Kortet sender ingen anmodning og tilbyder ingen fildownload.

En læsning af API markerer `stale` vises som muligvis forældet. En aflæsning, den markerer `unavailable` vises med dens årsag, aldrig som nul.

På procentplaner tegner siden nøglens egen andel, når API rapporterer det. Den siger, at tallet er et skøn og navngiver dets to dele. Grænser pr. model viser kun kontoen.

Når et vindue bærer `members`, viser dets kort også en bjælke med et segment pr. medlem, i rækkefølge. Den spørgende nøgles segment bruger accentfarven. De andre segmenter går gennem temaets diagramfarver. En tekstforklaring viser hvert segment med dets værdi, så intet afhænger af farven. Segmenter er mærket `You` eller `Member N`, hvor N er slot.

### Dedikeret port til siden

`QUOTA_PANEL_PORT` åbner en anden lytter, der kun betjener selvbetjeningssiden. Den er slået fra, medmindre variablen er indstillet. `QUOTA_PANEL_HOST` er bindeadressen og er standard til `127.0.0.1`.

Lytteren videresender disse stier til hovedporten og svarer 404 for hver anden sti:

| Sti                                                                      | Tjener                                        |
| ------------------------------------------------------------------------ | --------------------------------------------- |
| `/quota/{provider}`                                                      | Siden                                         |
| `/api/v1/me/quota/{provider}`, `/v1/me/quota/{provider}`                 | Den kvotevisning, siden læser                 |
| `/api/v1/me/usage`, `/v1/me/usage`                                       | Brugsserien siden læser                       |
| `/_next/static/`                                                         | Scripts, stilarter og skrifttyper i bygningen |
| `/favicon.ico`, `/favicon.svg`, `/icon-512.png`, `/apple-touch-icon.png` | Ikoner                                        |

`GET` og `HEAD` videresendes uden krop. En anmodning med en krop videresendes også: en `PATCH` af kvotevisningsstien, som siden sender for at gemme et udlånsvalg. Enhver anden metode svarer 404, undtagen en CONNECT -anmodning, hvis forbindelse er lukket uden svar. Enhver anden anmodning, der erklærer et organ, besvarer 404, og dets forbindelse er lukket. Opgraderingsanmodninger afvises, og deres forbindelse er lukket. En sti med et priksegment eller en fragmentmarkør afvises, som på API porten. Det samme er et anmodningsmål med et tegn uden for udskrivbar ASCII. Et rå kontroltegn i målet besvares 400 af HTTP parseren, før denne ports egen kontrol. Anmod om overskrifter, som rammen reserverer til eget brug, ikke videresendes: navne, der begynder med `x-middleware-`, `x-invoke-`, `x-nextjs-`, `x-now-` eller `x-next-`, og navnene `x-matched-path` og `next-resume`. Anmodningen videresendes uden dem. Dashboardet, login-siden, administrations- API og slutningsruterne kan ikke nås gennem denne port.

`PATCH` skal bære `Content-Type: application/json` uden parameter eller kun med `charset=utf-8`. Den skal have en `Content-Length` fra 1 til 4096, skrevet som almindelige cifre, og ingen `Transfer-Encoding`. En `PATCH`, der bryder en af disse regler, svarer 404. Nogle misformede længder, såsom en fortegnet eller en gentaget, besvares 400 af HTTP parseren før denne ports egen kontrol. Porten læser de erklærede bytes, før den kontakter hovedporten, og venter højst 5 sekunder på dem. En krop, der ikke er færdig på det tidspunkt, svarer 404, og dens forbindelse er lukket. Intet når hovedporten i det tilfælde, eller når klienten forlader først. Porten videresender nøjagtigt de erklærede bytes med den samme `Content-Length`. Bytes efter dem læses som den næste anmodning på forbindelsen. En TLS omvendt proxy foran skal videresende `Content-Length` og må ikke geninddele anmodningens tekst. Hovedporten tjekker API nøglen i `Authorization` headeren, som for `GET`.

404-kroppen er `{"error":"not_found","message":"Not found."}`. Et mislykket relæ svarer 502 (`api_bridge_unavailable`) eller 504 (`api_bridge_timeout`) uden `detail` felt.

Lytteren læser ikke `QUOTA_SELF_PANEL`, og den slår ikke siden til. Mens flaget er slukket, svarer siden og dens API 404 på hovedporten, og lytteren videregiver dette svar.

Under udviklingsserveren (`next dev`) bliver siden ikke interaktiv gennem denne port. Udviklings-hot-reload-socket er en opgraderingsanmodning, og porten afviser det. Brug hovedporten, mens du udvikler.

Porten serverer almindelig HTTP, og siden sender API nøgler. Behold standardbindingsadressen og sæt en omvendt proxy med TLS foran den. En anden bindingsadresse end loopback logger denne meddelelse:

```text
[Quota Panel] Bound to <host>. This port serves plain HTTP and the page sends API keys. Put a TLS reverse proxy in front of it.
```

En loopback-peer, der ikke sender nogen videresendelsesheader, tæller som lokal på hovedporten. Så en proxy på den samme vært skal sende `X-Forwarded-For`. En proxy på en privat adresse er kun tillid til denne header med `OMNIROUTE_TRUST_PROXY=private` (eller `lan`). Enhver anden peer rapporteres af adressen på dens forbindelse, og de videresendelsesheadere, den sendte, slettes.

Lytteren har højst 256 forbindelser ad gangen. En klient har 10 sekunder til at sende anmodningshovederne og 30 sekunder til at sende hele anmodningen. En inaktiv forbindelse, der holdes i live, lukker efter ca. 5 sekunder. En forbindelse uden aktivitet i 60 sekunder lukkes. Disse værdier er faste. Indstil også forbindelses- og hastighedsgrænser på den omvendte proxy foran. En omvendt proxy foran bør holde sine inaktive opstrømsforbindelser i mindre end 5 sekunder eller ikke genbruge dem. Relæet til hovedporten bruger opstrøms timeouts for API porten (`API_BRIDGE_*`).

Lytteren starter også, når `API_PORT` ikke er indstillet. `QUOTA_PANEL_PORT` skal være en port fra 1 til 65535, kun skrevet med cifre. Den skal adskille sig fra dashboard-porten og API porten. Mens live WebSocket serveren er tændt, skal den også afvige fra `LIVE_WS_PORT` (standard 20132). Enhver anden værdi åbner intet og logger en advarsel. En advarsel om en afvist værdi navngiver variablen og gentager ikke værdien. En port, der allerede er i brug, åbner intet og logger denne advarsel:

```text
[Quota Panel] Port <port> is already in use. The quota panel port stays off.
```

Med `OMNIROUTE_BASE_PATH` indstillet forventer lytteren hver vej over under det præfiks. Brug den samme `OMNIROUTE_BASE_PATH` på byggetidspunkt og på køretid. Skriv det med en indledende skråstreg og ingen efterfølgende skråstreg, for eksempel `/omniroute`. En anden form, inklusive `/` og `/omniroute/`, forlader porten med en advarsel, selvom bygningen accepterer disse former. Det samme gør en basissti, hvis første segment navngiver en applikationsrute: `api`, `v1`, `v1beta`, `_next`, `quota`, `dashboard`, `docs`, `login`, `codex`, `responses`, `anthropic`, `openai`, `v0` eller `connect`, under alle omstændigheder.

Begrænsninger:

- `/quota/{provider}/` med en efterfølgende skråstreg svarer 404 på denne port.
- Serviceworkeren og webapp-manifestet vises ikke på denne port.
- Et brugerdefineret favicon-sæt i dashboardet vises ikke på denne port.
- Ikoner vises ikke, når programmet kører under en basissti.
- Havnen taler almindeligt HTTP/1.1.
- En binding, der mislykkes, forsøges ikke igen, før processen genstartes.
- Lytteren har ingen forbindelse eller hastighedsgrænse pr. klientadresse.
- Containeropsætninger er ikke omfattet af dette afsnit.

---

## Miljøvariabler

| Variabel                             | Misligholdelse | Beskrivelse                                                             |
| ------------------------------------ | -------------- | ----------------------------------------------------------------------- |
| `QUOTA_STORE_DRIVER`                 | `sqlite`       | Driver til brug: `sqlite` eller `redis`                                 |
| `QUOTA_STORE_REDIS_URL`              | _(tom)_        | Redis URL, fx `redis://localhost:6379`                                  |
| `QUOTA_SATURATION_THRESHOLD`         | `0.5`          | 0..1; `>= threshold` aktiverer streng tilstand                          |
| `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` | `1000`         | Tokens, der forklarer højst ét punkt af et procentplanvindue            |
| `QUOTA_SOFT_DEPRIORITIZE_FACTOR`     | `0.7`          | 0..1; multiplikator for soft-policy combo score                         |
| `QUOTA_CONSUMPTION_RETENTION_DAYS`   | `14`           | Dage før GC fjerner gamle `quota_consumption` spande                    |
| `QUOTA_PANEL_PORT`                   | _(frakoblet)_  | Dedikeret port til selvbetjeningssiden. Frakoblet betyder ingen lytter. |
| `QUOTA_PANEL_HOST`                   | `127.0.0.1`    | Bind adresse for den port                                               |

DB indstillinger (`quotaStore.*`) tilsidesætter env vars.

---

## Fejlfinding

### Redis er konfigureret, men opretter ikke forbindelse

Kontrollér, at `ioredis` er installeret (`npm ls ioredis`), og at
`QUOTA_STORE_REDIS_URL` kan nås. Hvis forbindelsen mislykkes, falder factoryen
tilbage til SQLite (logges på niveauet `warn`).

### `peek` returnerer forældede data / fail-open

Hvis `peek` udløser en fejl, behandler `enforceQuotaShare` resultatet som
"tillad" (fail-open). Kontrollér `pino`-logfilerne for posterne `quota:enforce`
og `quota:factory` for at identificere den grundlæggende årsag.

### Afvigelse i forbrugstæller

Hvis udbyderens faktiske forbrug afviger fra tællerne, er det forventeligt —
det glidende vindue med 2 buckets har en fejl på ~1 % ved vinduesgrænserne, og
`consume` køres som fire-and-forget efter svaret. Mætningssignalet
(`saturationSignals.ts`) aflæser udbyderens reelle udnyttelse med en TTL på
30 sekunder og justerer `globalUsedPercent` tilsvarende.

### Puljen viser "ingen data" for forbrugsrate

`computeBurnRate` kræver mindst 2 historiske målinger. Nye puljer uden tidligere
kald til `consume` vil vise `tokensPerSecond: 0` og `timeToExhaustionMs: null`.

---

## Migrering fra localStorage

Når `/dashboard/costs/quota-share` indlæses første gang, kontrollerer hooken `useLocalStoragePoolMigration`:

1. `localStorage.getItem("omniroute:quota-share:pools")` er ikke tom.
2. `GET /api/quota/pools` returnerer `[]` (DB'en er tom).

Hvis begge betingelser er opfyldt, sender den hver ældre pulje samlet til `POST /api/quota/pools` og fjerner derefter localStorage-nøglen. Migreringen er idempotent: Betingelse 2 forhindrer gentagen migrering.

---

## Intern strategiklassificering

`quota-share` er en routingstrategi, der **kun er intern** (`INTERNAL_ROUTING_STRATEGY_VALUES` i `src/shared/constants/routingStrategies.ts`). Den bruges udelukkende af systemgenererede `qtSd/`-puljekombinationer og er bevidst udeladt fra `ROUTING_STRATEGY_VALUES`, så den aldrig vises som en valgmulighed for brugeren i brugergrænsefladen eller API'et.

---

## Testdækning

To lag af automatiseret dækning sendes med kvotedelingsmotoren:

| Suite              | Kommando                                                               | Hvad det dækker over                                                                                                                                                                                   |
| :----------------- | :--------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Enhed (29 test)    | `node --import tsx/esm --test tests/unit/quota-share-strategy.test.ts` | DRR skemalægger, saturation gating, concurrency caps, fairShare math, backlog kø                                                                                                                       |
| Integrationsmatrix | `npm run test:combo:matrix`                                            | End-to-end routing-beslutning gennem den rigtige combo pipeline; DRR fairness + saturation deprioritering via live-sømme (`registerQuotaFetcher`, `setLKGP`, `__setHeadroomSaturationFetcherForTests`) |

Integrationsmatricen kører i CI sammen med alle 22 offentlige strategier. Enhedspakken kan køres selvstændigt.

---

## DB skemaoversigt

Tre tabeller tilføjet af migrationer `078`, `079` og `085`:

- `quota_pools` + `quota_allocations` — puljedefinitioner og tildelinger pr. nøgle.
- `quota_consumption` — rullende 2-spand tællere pr `(apiKeyId, dimensionKey)`.
- `provider_plans` — manuelle udbyderplantilsidesættelser (dimensioner JSON pr. connectionId).

Alle tabeller tilføjet via idempotente `CREATE TABLE IF NOT EXISTS` migreringer.

Samtykkede udlån tilføjer tre kolonner: `quota_allocations.lending_percent` (heltal, standard 0), `quota_allocations.lending_until` (epoke millisekunder eller `NULL` uden deadline) og `quota_pools.borrow_mode` (standard `saturation`). Dens migrering tilføjer kun disse kolonner og skriver ingen eksisterende række.

Procenttilskrivningsbogen tilføjer `quota_percent_ledger` (én række pr. pulje, konto og planvindue) og `quota_percent_ledger_tokens` (én tokentæller pr. pulje, konto og API nøgle). `src/lib/db/quotaPercentLedger.ts` læser og skriver dem.
