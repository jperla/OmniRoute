# Quota Sharing Engine (Bosanski)

🌐 **Languages:** 🇺🇸 [English](../../../../routing/QUOTA_SHARE.md) · 🇪🇹 [am](../../../am/docs/routing/QUOTA_SHARE.md) · 🇸🇦 [ar](../../../ar/docs/routing/QUOTA_SHARE.md) · 🇦🇿 [az](../../../az/docs/routing/QUOTA_SHARE.md) · 🇧🇬 [bg](../../../bg/docs/routing/QUOTA_SHARE.md) · 🇧🇩 [bn](../../../bn/docs/routing/QUOTA_SHARE.md) · 🇨🇿 [cs](../../../cs/docs/routing/QUOTA_SHARE.md) · 🇩🇰 [da](../../../da/docs/routing/QUOTA_SHARE.md) · 🇩🇪 [de](../../../de/docs/routing/QUOTA_SHARE.md) · 🇬🇷 [el](../../../el/docs/routing/QUOTA_SHARE.md) · 🇪🇸 [es](../../../es/docs/routing/QUOTA_SHARE.md) · 🇪🇪 [et](../../../et/docs/routing/QUOTA_SHARE.md) · 🇮🇷 [fa](../../../fa/docs/routing/QUOTA_SHARE.md) · 🇫🇮 [fi](../../../fi/docs/routing/QUOTA_SHARE.md) · 🇫🇷 [fr](../../../fr/docs/routing/QUOTA_SHARE.md) · 🇮🇪 [ga](../../../ga/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [gu](../../../gu/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [ha](../../../ha/docs/routing/QUOTA_SHARE.md) · 🇮🇱 [he](../../../he/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [hi](../../../hi/docs/routing/QUOTA_SHARE.md) · 🇭🇷 [hr](../../../hr/docs/routing/QUOTA_SHARE.md) · 🇭🇺 [hu](../../../hu/docs/routing/QUOTA_SHARE.md) · 🇦🇲 [hy](../../../hy/docs/routing/QUOTA_SHARE.md) · 🇮🇩 [id](../../../id/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [ig](../../../ig/docs/routing/QUOTA_SHARE.md) · 🇮🇹 [it](../../../it/docs/routing/QUOTA_SHARE.md) · 🇯🇵 [ja](../../../ja/docs/routing/QUOTA_SHARE.md) · 🇬🇪 [ka](../../../ka/docs/routing/QUOTA_SHARE.md) · 🇰🇭 [km](../../../km/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [kn](../../../kn/docs/routing/QUOTA_SHARE.md) · 🇰🇷 [ko](../../../ko/docs/routing/QUOTA_SHARE.md) · 🇱🇹 [lt](../../../lt/docs/routing/QUOTA_SHARE.md) · 🇱🇻 [lv](../../../lv/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [ml](../../../ml/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [mr](../../../mr/docs/routing/QUOTA_SHARE.md) · 🇲🇾 [ms](../../../ms/docs/routing/QUOTA_SHARE.md) · 🇲🇹 [mt](../../../mt/docs/routing/QUOTA_SHARE.md) · 🇲🇲 [my](../../../my/docs/routing/QUOTA_SHARE.md) · 🇳🇵 [ne](../../../ne/docs/routing/QUOTA_SHARE.md) · 🇳🇱 [nl](../../../nl/docs/routing/QUOTA_SHARE.md) · 🇳🇴 [no](../../../no/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [or](../../../or/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [pa](../../../pa/docs/routing/QUOTA_SHARE.md) · 🇵🇭 [phi](../../../phi/docs/routing/QUOTA_SHARE.md) · 🇵🇱 [pl](../../../pl/docs/routing/QUOTA_SHARE.md) · 🇵🇹 [pt](../../../pt/docs/routing/QUOTA_SHARE.md) · 🇧🇷 [pt-BR](../../../pt-BR/docs/routing/QUOTA_SHARE.md) · 🇷🇴 [ro](../../../ro/docs/routing/QUOTA_SHARE.md) · 🇷🇺 [ru](../../../ru/docs/routing/QUOTA_SHARE.md) · 🇱🇰 [si](../../../si/docs/routing/QUOTA_SHARE.md) · 🇸🇰 [sk](../../../sk/docs/routing/QUOTA_SHARE.md) · 🇸🇮 [sl](../../../sl/docs/routing/QUOTA_SHARE.md) · 🇷🇸 [sr](../../../sr/docs/routing/QUOTA_SHARE.md) · 🇸🇪 [sv](../../../sv/docs/routing/QUOTA_SHARE.md) · 🇰🇪 [sw](../../../sw/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [ta](../../../ta/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [te](../../../te/docs/routing/QUOTA_SHARE.md) · 🇹🇭 [th](../../../th/docs/routing/QUOTA_SHARE.md) · 🇹🇷 [tr](../../../tr/docs/routing/QUOTA_SHARE.md) · 🇺🇦 [uk-UA](../../../uk-UA/docs/routing/QUOTA_SHARE.md) · 🇵🇰 [ur](../../../ur/docs/routing/QUOTA_SHARE.md) · 🇺🇿 [uz](../../../uz/docs/routing/QUOTA_SHARE.md) · 🇻🇳 [vi](../../../vi/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [yo](../../../yo/docs/routing/QUOTA_SHARE.md) · 🇨🇳 [zh-CN](../../../zh-CN/docs/routing/QUOTA_SHARE.md) · 🇹🇼 [zh-TW](../../../zh-TW/docs/routing/QUOTA_SHARE.md)

---

# Mehanizam za dijeljenje kvota

> **Referenca dokumenta**: `docs/routing/QUOTA_SHARE.md`
> Dio Grupe B (planovi 16 + 22).

---

## Pregled

Mehanizam za dijeljenje kvota (Quota Sharing Engine) distribuira vremenski ograničenu kvotu provajdera (npr. Codex 5-satni prozor, Kimi 1500 zahtjeva/h) ravnomjerno između više API ključeva koji dijele istu konekciju.

**Problem koji rješava:** OmniRoute proksira mnoge API ključeve prema istom upstream nalogu provajdera. Bez logike dijeljenja, nagli porast (burst) sa ključa A može iscrpiti kvotu provajdera za taj sat, ostavljajući ključeve B i C blokiranim dok se prozor ne resetuje. Mehanizam ovo sprječava tako što:

1. Prati tekuću potrošnju svakog ključa po dimenziji (%, zahtjevi, tokeni, $).
2. Primjenjuje algoritam pravedne raspodjele koji čuva rad: ključ može posuditi iz neiskorištenih udjela dok globalni skup nije zasićen.
3. Sprovođenjem rezultata u "hot path" (`chatCore.ts`) prije nego što zahtjev stigne do upstream izvršioca.

---

## Algoritam: pošteno podijeliti rad-očuvati

Implementirano u `src/lib/quota/fairShare.ts`.

### Načini rada

| Stanje                                     | Mode            | Ponašanje                                                     |
| ------------------------------------------ | --------------- | ------------------------------------------------------------- |
| `globalUsedPercent < saturationThreshold`  | **Velikodušno** | Ključ može posuditi do globalnog limita minus potrošen-ukupno |
| `globalUsedPercent >= saturationThreshold` | **Strogo**      | Strogo sprovoditi individualno pošteno učešće                 |

Zadani `saturationThreshold = 0.5` (env `QUOTA_SATURATION_THRESHOLD`).

Ova dva načina opisuju skup u zadanom načinu zaduživanja, `saturation`. Grupa u `consent` modu uvijek primjenjuje stroga pravila, bez obzira na zasićenost. Pogledajte [Posuđivanje sa suglasnošću (opt-in po bazenu)](#consented-lending-per-pool-opt-in).

### Odluka po dimenziji

Za svaku aktivnu dimenziju u bazenu, motor izračunava:

```
fairShareAllowed = poolLimit × (allocationWeight / 100)
consumed        = current rolling value for this key (from QuotaStore.peek)
remaining       = fairShareAllowed - consumed
```

Za dimenzije `percent`, `consumed` umjesto toga dolazi iz knjige atribucije (pogledajte [Procentualne dimenzije: atribucija po ključu](#percent-dimensions-per-key-attribution) ).

onda:

- **`policy = hard`** : ako je `consumed > fairShareAllowed` i mod je strog →** blok** .
- **`policy = soft`** : ako je `consumed > fairShareAllowed` i mod je strog →** kazniti** (odbacivanje prioriteta u kombinaciji; nikada hard-blok).
- **`policy = burst`** : dozvoli dok postoji globalni prostor bez obzira na pošteno učešće.

### Cap absoluto

`capValue` + `capUnit` na alokaciji je strogi plafon neovisno o načinu ili politici. Bilo koja dimenzija gdje je uvijek `consumed >= capValue`** blokova** zahtjev. Za `percent` cap, `consumed` je samo dio pripisan ključu.

### Višedimenzionalna provjera

Zahtjev je blokiran ako** bilo koji** dimenzija u bazenu bi ga blokirala. Dimenzije su nezavisne — 5h% iscrpljenosti ne utječe na sedmičnu % dimenziju.

### Pozajmljivanje

U velikodušnom modu, ključ čija je alokacija nedovoljno potrošena može koristiti višak neraspoređenih dionica drugih ključeva. Formula je:

```
maxAllowed = globalLimit - consumedByOtherKeys
```

gdje `consumedByOtherKeys = consumedTotal - consumedByThisKey`. Teto global (pool `limit` za tu dimenziju) je uvijek tvrdi plafon.

### Pozajmljivanje sa suglasnošću (opt-in po bazenu)

Svaki bazen ima način posudbe. `saturation` je zadana vrijednost i zadržava gore navedena pravila. U `consent` modu `hard` ključ prenosi svoj udio samo u okviru kapaciteta koji su drugi ključevi pristali da pozajme. Administrator postavlja način rada svakog bazena. Svaki nosilac ključa daje sopstvenu saglasnost putem [saglasnosti za kreditiranje](#lending-consent).

Pristanak je postotak od 0 do 100 i izborni rok u epohi milisekundama. Ključ posuđuje taj procenat svog neaktivnog udjela dok je rok u budućnosti.

Za jednu dimenziju, `L` je efektivno ograničenje: ograničenje plana pomnoženo s računima u skupu. Vrata računa, za ključ koji traži:

```
share_k         = w_k / 100 × L
idle_k          = max(0, share_k − consumed_k)
lent            = Σ over the other keys of lend_k / 100 × idle_k
taken           = Σ over the other keys of max(0, consumed_k − share_k)
borrowAvailable = max(0, lent − taken)
```

`w_k` je težina ključa, ili `100 / n` za svaki ključ kada nijedna težina nije veća od 0. `lend_k` je aktivni postotak ključa, a 0 nakon isteka roka. Vlastiti pristanak ključa koji je tražio nikada se ne računa. `hard` ključ se odbija kada njegova potrošnja dostigne svoj udio plus `borrowAvailable`.

Kapacitet koji nijedna alokacija ne zahteva (100 minus zbir pondera) nije pozajmljiva. Nijedan ključ nije pristao da ga posudi.

**Primjer.** `L` je 1000.

| Ključ | Težina | Dijeli | Potrošeno | Pozajmljuje |
| ----- | ------ | ------ | --------- | ----------- |
| A     | 50     | 500    | 530       | 0%          |
| B     | 30     | 300    | 100       | 50%         |
| C     | 0      | 0      | 60        | 0%          |

- B pozajmljuje 50% svojih 200 u mirovanju, što je 100. C je već uzeo 60 iznad svog udjela. A može da pozajmi 40.
- A se servira na 530 i odbija se kada njegova potrošnja dostigne 540.
- Prije nego što je C koristio bilo šta, s A na ili ispod svog udjela, C je mogao posuditi 100.
- Prije nego što je C koristio bilo šta, sa A na 530, C je mogao posuditi 70.

**Nulta težina.** Ključ težine 0 ima udio 0. Služi se samo dok je njegova potrošnja ispod onoga što drugi pozajmljuju. Kada niko ne pozajmljuje, odbija se od prvog zahteva.

**Rokovi.** Nijedan zadatak u pozadini ne ističe pristanak. Svaki zahtjev upoređuje rok sa svojim vremenom, a rok jednak tom vremenu je prošao. Pohranjeni rok koji nije konačan broj ili je prošao najveći datum koji `Date` može zadržati, računa se kao prošao.

**`soft` i `burst`.** Kreditiranje ih ne ograničava. `soft` ključu se gubi prioritet kada pređe svoj dio. `burst` ključ prolazi dok bazen ima mjesta. Plafon bazena i dalje odbija svaki ključ kada ukupan iznos bazena dostigne svoju granicu.

**Cijena na putu zahtjeva.** `saturation` bazen ne čita ništa više nego prije. U `consent` skupu, brojiva dimenzija čita druge ključeve samo za `hard` ključ na ili iznad njegovog udjela, dok drugi ključ posuđuje. Zatim vrši jedno čitanje po drugom ključu, paralelno. Neuspješno čitanje se računa kao potrošnja 0 za taj ključ. `percent` dimenzija ne dodaje čitanje, jer knjiga atribucije sadrži svaki ključ.

**Uređivanje bazena.** Uređivanje zadržava saglasnost ključeva koji ostaju. Ovo vrijedi za izmjene alokacije, zamjene u cijeloj grupi i `ensure` pozive. Uklonjeni ključ gubi saglasnost, a ključ koji je ponovo dodan počinje od 0. Administratorske rute vraćaju pristanak svakog ključa i nikada ga ne pišu. Prebacivanje skupa natrag na `saturation` zadržava svaki pohranjeni pristanak, što nema efekta u tom načinu rada. Ponovno prebacivanje bazena na `consent` ponovo aktivira pohranjene pristanke čiji rok nije prošao. Nosilac ključa može izbrisati pohranjeni pristanak u bilo kojem načinu rada.

**Nadogradnja.** Ako kolone `lending_percent` i `lending_until` već postoje, migracija dodaje samo `borrow_mode`, a pohranjeni postoci ostaju onakvi kakvi jesu. Svaki bazen počinje u `saturation` modu. Uključite `consent` po bazenu u čarobnjaku bazena. Ništa se ne zaključuje iz pohranjenih vrijednosti.

**Ograničenja.**

- Zajmodavac može pronaći bazen na svom plafonu prije nego što iskoristi svoj udio. Kapacitet koji su drugi pozajmili uračunava se u ukupni bazen.
- Provjera se pokreće prije zahtjeva i ne rezerviše ništa. Istovremeni zahtjevi očitavaju potrošnju prije nego što se bilo koji evidentira, tako da se pozajmljeni kapacitet može potrošiti više puta, ograničeno zahtjevima u letu. Provjera dijeljenja `saturation` načina ima isto svojstvo.

---

## Brojač kliznog prozora

Implementirano u `src/lib/quota/sqliteQuotaStore.ts` i `redisQuotaStore.ts`.

Dva bucketa po `(apiKeyId, dimensionKey)`:

- `curr`: trenutni bucket (`floor(nowMs / windowMs)`)
- `prev`: prethodni bucket (`curr - 1`)

Efektivna tekuća vrijednost:

```
effectiveBucketIndex = floor(nowMs / windowMs)
bucketStartMs        = effectiveBucketIndex × windowMs
elapsed              = nowMs - bucketStartMs
weight               = 1 - elapsed / windowMs

effective = prev × weight + curr
```

**Preciznost**: ~99% tačno. Greška je najviše 1% veličine prozora na granici između bucketa (inherentno aproksimaciji sa 2 bucketa).

### Konkurentnost

SQLite drajver: in-memory mutex po `(apiKeyId | dimensionKey)` ključu sprječava "read-modify-write" trku. Obrazac preslikava `src/sse/services/auth.ts` anti-thundering-herd (zaštita od preopterećenja).

Redis drajver: Lua EVAL skripta za atomsko povećanje — izvršava se kao jedna Redis komanda.

## Drajveri

### SQLite (podrazumevano, 0-instalacija)

- Tabela: `quota_consumption` (pogledajte migraciju `073_quota_pools.sql` / `074_quota_consumption.sql`).
- Najbolje za implementacije sa jednom instancom.
- Sva perzistencija se nalazi u postojećoj OmniRoute SQLite bazi podataka (`DATA_DIR/storage.sqlite`).

### Redis (opciono, više-instancno)

- Zahtijeva `ioredis` npm paket.
- Brojači su pohranjeni u Redis-u; metapodaci (pool-ovi/alokacije) su i dalje u SQLite-u.
- Najbolje za implementacije sa više replika gdje se brojači moraju dijeliti.

### Promjena drajvera

Putem korisničkog interfejsa za podešavanja (`/dashboard/settings` → Quota Store), ili putem env varijabli:

```bash
QUOTA_STORE_DRIVER=redis
QUOTA_STORE_REDIS_URL=redis://localhost:6379
```

Podešavanje baze podataka ima prednost nad env varijablama. Ako je `driver=redis`, ali URL nedostaje ili `ioredis` nije instaliran, factory se vraća na SQLite i bilježi upozorenje.

Redoslijed odabira drajvera:

1. DB podešavanje `quotaStore.driver`
2. Env `QUOTA_STORE_DRIVER`
3. Podrazumevano: `sqlite`

---

## Multi-Dimension

Bazen može imati više dimenzija. Svaka dimenzija je nezavisna:

```ts
QuotaDimension {
  unit: "percent" | "requests" | "tokens" | "usd",
  window: "5h" | "hourly" | "daily" | "weekly" | "monthly",
  limit: number,  // global pool ceiling for this dimension
}
```

**Primjer: Codex plan** (5h% + sedmično%):

```json
[
  { "unit": "percent", "window": "5h", "limit": 100 },
  { "unit": "percent", "window": "weekly", "limit": 100 }
]
```

Zahtjev mora zadovoljiti sve dimenzije da bi bio dozvoljen.

### Procentualne dimenzije: atribucija po ključu

Plan postotaka prijavljuje jednu cifru korištenja po računu i prozoru plana. Provajder ne daje brojač po API ključu.

Da bi se taj broj podijelio između ključeva, svaki skup vodi knjigu atribucije po računu i prozoru plana. `src/lib/quota/percentLedger.ts` drži pravila knjige. `src/lib/quota/percentAttribution.ts` pretvara knjigu u brojeve koje provođenje koristi. Rezultat je procjena izgrađena od tokena za svaku ključnu rutu.

#### Čitanja koja pokreću knjigu

Knjiga se kreće samo prema vlastitoj figuri dobavljača za traženi prozor plana. Ove veze prijavljuju jedno:

| Provajder                | Planirajte prozore |
| ------------------------ | ------------------ |
| Claude, preko OAuth veze | `5h`, `weekly`     |
| Codex                    | `5h`, `weekly`     |

Ovo se ne računa kao očitavanje:

- odgovor koji klijent provajdera označava kao zastareo
- Claude prozor čiji procenat provajder nije prijavio
- figura drugog prozora, ili u najgorem slučaju preko prozora
- rezervno zaglavlje ograničenja brzine
- neuspješno čitanje

Drugi provajderi, uključujući Claude sa API ključem, nemaju knjigu. Svaki ključ se naplaćuje 0 na svoje procentualne dimenzije, kao i prije ove promjene.

Očitavanje dijeli 30-sekundni keš signala zasićenja. Očitavanje Claude je datirano kada je cifra uočena u zaglavljima odgovora ili pročitana iz krajnje tačke upotrebe, kada je to vrijeme poznato. Ostala očitavanja su datirana po vremenu kada je taj unos u keš memoriji napravljen.

#### Šta knjiga čuva

Svaki snimljeni zahtjev dodaje svoje tokene, jednom, na brojač po grupi, računu i ključu. Brojač samo raste. Knjiga sadrži tri stvari:

- osnovna linija: brojka kada se knjiga otvorila ili prozor zadnji put okrenut
- posljednja primijenjena figura
- po ključu, njegov brojač tokena u tom istom trenutku, nazvan njegov znak

Knjiga se ažurira kada provedba ili ruta korištenja izračuna atribuciju. Upisi se upoređuju i postavljaju na broj revizije. Pisac koji izgubi ponovo pokušava jednom prilikom novog čitanja.

#### Kako se računa dio ključa

Svaki dio ključa se računa kada se knjiga čita. Rast figure od osnovne linije se dijeli između ključeva proporcionalno tokenima koji se usmjeravaju od svoje oznake.

Together, ti tokeni objašnjavaju najviše jednu tačku figure po `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` tokenima (podrazumevano 1.000). Rast koji oni ne objašnjavaju je spoljašnji. Osnovna linija je također eksterna.

Na primjer, knjiga se otvara na 0. Ključ A zatim usmjerava 900.000 tokena, a ključ B usmjerava 100.000. Kod broja 60, dio A je 54 boda, a dio B je 6.

Brojač ispod oznake ključa se ponovo pokrenuo i broji se u potpunosti. Ključ bez oznake, kao što je ključ koji se pridružuje grupi u sredini prozora, broji sve svoje tokene. Brojka koja zaostaje za tokenima uzrokuje grešku koja nestaje pri sljedećem čitanju. Ne akumulira se.

`QUOTA_PERCENT_MIN_TOKENS_PER_POINT` se čita na svakoj atribuciji. Vrijednost koja nije konačan broj od najmanje 1 pada nazad na 1.000.

#### Kako čitanje mijenja knjigu

Primjenjuje se prvo pravilo podudaranja:

1. **Još nema knjige:** čitanje otvara knjigu. Njegova figura je osnovna linija i svaki brojač je označen.
2. **Starije čitanje:** čitanje datirano prije posljednjeg primijenjenog se zanemaruje. Tako je i očitavanje čije je vrijeme resetovanja više od 30 minuta ranije od pohranjenog.
3. **Novi prozor provajdera:** vrijeme resetovanja više od 30 minuta kasnije od pohranjenog okreće knjigu. Brojka postaje osnovna linija i svaki brojač se ponovo označava. Ključevi bez šaltera napuštaju knjigu.
4. **Završen prozor:** pohranjeno vrijeme resetovanja koje nije nakon vremena očitavanja podataka znači da je prozor završen. Čitanje okreće knjigu, bez obzira na njenu figuru.
5. **Viša cifra:** samo posljednja figura se pomjera. Osnovna linija i oznake ostaju.
6. **Ista cifra:** figura, osnovna linija i oznake ostaju. Napisano je samo vrijeme resetiranja koje nedostaje knjizi.
7. **Donja cifra:** niži broj se nikada ne primjenjuje kao takav. Preokreće knjigu samo kada tri stvari stoje. To je najmanje dvije minute novije od posljednjeg primijenjenog očitanja. Ništa ne kaže da je prozor isti otvoren. To je više od jednog poena niže.

Prozor se računa kao isti otvoreni kada tri stvari drže. Oba vremena resetovanja su poznata. Udaljeni su 30 minuta jedan od drugog. Pohranjeni je još uvijek ispred očitavanja. Niža figura unutar tog prozora ništa ne mijenja.

Vrijeme resetiranja se pohranjuje samo dok je ispred vremena podataka očitavanja koje ga nosi. Viša cifra pohranjuje vrijeme resetovanja svog očitanja kada je ono upotrebljivo, a u suprotnom zadržava pohranjeno. Jednaka cifra bilježi vrijeme resetovanja svog čitanja samo kada ga knjiga nema. Ništa drugo ne mijenja. Niža brojka koja ne okreće knjigu ne bilježi vrijeme resetiranja.

#### Kada se knjiga koristi

Nakon čitanja, knjiga se koristi osim ako njeno pohranjeno vrijeme resetovanja nije nakon trenutnog vremena. Taj slučaj nastaje kada se očitavanje snimljeno neposredno prije resetiranja, kao što je ono koje se servira iz keša, promatra neposredno nakon toga.

Bez upotrebljivog čitanja, pohranjena knjiga se koristi samo dok još uvijek može biti knjiga trenutnog prozora. To važi u dva slučaja:

- njegovo vrijeme resetovanja je poznato i još je pred nama
- nema vrijeme resetiranja, a posljednje očitanje koje ga je promijenilo je staro najviše 15 minuta

Inače se ništa ne pripisuje, kao kad nema knjige. Knjiga čije je pohranjeno vrijeme resetiranja prošlo nikada se ne naplaćuje.

#### Izvršenje

Potrošnja ključa na dimenziji procenta je njegov pripisani dio plus udio vanjskog dijela. Eksterni dio prvo koristi kapacitet bez zahtjeva za dodjelu (100 minus zbir pondera). Samo se višak dijeli među ključevima po težini.

Ta se potrošnja uspoređuje sa poštenim udjelom ključa kao i za bilo koju drugu dimenziju. Strogi način rada i dalje počinje kada signal zasićenja dostigne `QUOTA_SATURATION_THRESHOLD` (podrazumevano 0,5). Svaki broj je skaliran efektivnim ograničenjem: ograničenje po računu puta broj računa u grupi.

Apsolutno ograničenje sa `capUnit: "percent"` broji samo dio pripisan ključu, skalirano na isti način. Uzmite ograničenje po računu od 100 i k računa. Granica od N se tada postiže kada dio ključa u cifri računa za posluživanje dostigne N/k poena. Svaki račun se provjerava prema svojoj knjizi. Na primjer, sa dva računa, ograničenje od 10 se postiže na 5 bodova brojke jednog računa.

Kada se prodavnica ne može očitati, ništa se ne pripisuje i svaki ključ se naplaćuje 0 na toj dimenziji. Kada pisanje knjige ne uspije, ta atribucija koristi knjigu onako kako je pročitana. Neuspješno upisivanje tokena ostavlja tokene tog zahtjeva izvan knjige. Nijedan od ovih kvarova ne blokira zahtjev.

U `consent` fondu, formula za pozajmljivanje koristi potrošnju svakog ključa na dimenziji postotaka kao što je gore opisano. Kada se pozajmi drugi ključ, knjiga se čita jednom i pripisuje svakom ključu. Bez upotrebljive knjige svaki ključ se naplaćuje 0. Ključ s težinom tada prolazi, a ključ s težinom 0 prolazi samo kada drugi ključ posudi.

#### Ruta upotrebe

`GET /api/quota/pools/{id}/usage` prijavljuje iste brojeve kroz istu funkciju. Dimenzija postotka ima jedan unos po vezi bazena u `accounts`. Njegovi `consumedTotal` i `perKey` na najvišem nivou odražavaju prvi unos.

Ruta također primjenjuje trenutno čitanje, tako da može unaprijediti knjigu kao što to čini zahtjev. `internal + external` se može razlikovati od `consumedTotal` kada nema upotrebljivog očitanja ili kada se ne primjenjuje niži broj.

#### Čuvanje i zadržavanje

Obje prodavnice kvota vode knjigu. Na SQLite, automatsko čišćenje baze podataka, kada je omogućeno, uklanja redove koji nisu ažurirani 60 dana. Na Redis, knjige i brojači veze bazena dijele jedan ključ. Istječe 60 dana nakon posljednjeg upisa tokena ili promjene knjige. Knjiga koja se ne mijenja se ne prepisuje, tako da se granica postavlja iznad najdužeg prozora plana. Ručno resetovanje istorije korišćenja takođe briše knjige o SQLite (pogledajte Ograničenja).

#### Ograničenja

- Sav rast broja računa od osnovne linije se dijeli na tokene, svaki ključ koji se od tada usmjerava. Kada je došlo do tog rasta nije bitno.
- Dakle, upotreba izvan OmniRoute se naplaćuje ključevima do onog što njihovi tokeni dozvoljavaju. To uključuje upotrebu napravljenu prije prvog zahtjeva ključa za prozor, kada je knjiga već bila otvorena.
- Na primjer, vanjska upotreba podiže račun za 60 bodova dok nema ključnih ruta. Ključ tada usmjerava 30.000 žetona i broj dostiže 60,6.
- Ako je knjiga bila otvorena prije te upotrebe, dio ključa je 30 bodova. Takođe nosi 7,65 eksterne upotrebe, sa četiri ključa težine 25.
- Ako se knjiga otvori nakon te upotrebe, 60 bodova je osnovna linija. Deo ključa je 0,6 poena, a nosi 15 eksterne upotrebe.
- Zahtjev ili posjeta ruti upotrebe otvara knjigu. Dakle, da li se takva upotreba računa kao osnovna, zavisi od toga kada je knjiga otvorena.
- Sa zadanim pragom, ključ koji usmjerava 60.000 tokena dok vanjska upotreba podiže račun za 60 bodova dobiva svih 60 kao vlastiti dio.
- Sa podom od 50.000, vlastiti dio je 1,2 boda. Ostalih 58,8 su vanjski i naplaćuju se po težini, kao i svaka vanjska upotreba.
- Postavite `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` blizu onoga što košta jedan bod na vašem planu. Vanjska upotreba uključuje promet na istom računu s ključeva izvan bazena.
- Ograničenje postotaka primjenjuje se u svakom načinu rada. Ograničeni ključ se može odbiti dok je račun daleko ispod praga zasićenja.
- Uzmite kapu od 10 i 12 tačaka vanjske upotrebe ranije u prozoru. Ključ koji usmjerava 20.000 tokena se tada odbija uz cifru računa od 12,4%.
- Podjela je procjena po obimu tokena. Zahtjev se računa kao njegovi prompt tokeni plus njegovi tokeni završetka. Popusti u predmemoriji i cijene modela ne mijenjaju taj broj.
- Zahtjev koji se ne završava statusom 200 ne bilježi tokene. Primjeri su tok koji klijent prekida i greška u uzvodnom toku nakon što je upotreba potrošena.
- Upotreba takvog zahtjeva naplaćuje se ključevima koji su snimili tokene, do onog što njihovi tokeni dozvoljavaju. Ostalo je eksterno. Ne pomera se nazad. Odgovor koji prijavljuje da nema upotrebe tokena ne bilježi ni tokene.
- Upotreba zahtjeva u toku može se prikazati u drugom dijelu aktivnog ključa za cijeli zahtjev. Vraća se nazad tek kada zahtjev završi sa statusom 200.
- Upotreba koja je već na računu kada se knjiga otvori računa se kao eksterna. Ovo pokriva nadogradnju, novi skup i novi račun. Upotreba u novom prozoru prije prvog čitanja također se računa kao eksterna.
- Svaki ključ počinje sa svojim težinskim udjelom te upotrebe, nakon kapaciteta nema zahtjeva za dodjelu. Sa jednim računom na 85% i pet ključeva težine 20, svaki počinje sa 17 od 20 korištenih ključeva.
- U grupi sa nekoliko naloga, cifra računa za posluživanje se primenjuje na zbirni budžet. Ovo je nepromijenjeno u knjizi.
- Niža brojka unutar prozora za koji provajder prijavljuje da je otvorena nije primijenjena. Vreme resetovanja koje se pomera unazad za više od 30 minuta se tretira kao staro očitavanje.
- U oba slučaja knjiga zadržava svoje stanje dok ne prođe pohranjeno vrijeme resetiranja. Nakon toga, knjiga se ne naplaćuje dok je čitanje ne pretvori.
- Lijek je ručno resetiranje istorije upotrebe (`POST /api/settings/purge-usage-history`). Briše knjige atribucije i njihove brojače tokena u SQLite bazi podataka.
- `all` period čisti svaku knjigu i šalter. Kraći period prvo briše knjige koje nisu napisane u njemu. Zatim briše brojače koji nisu upisani u njemu, već samo za vezu bazena koja nema preostalu knjigu. Čuvana knjiga i dalje označava svaki ključ na svom brojaču.
- Knjiga čija se figura nije pomjerila se ne prepisuje, tako da kraći period također može obrisati knjigu trenutnog prozora. Sljedeće čitanje tada otvara novu knjigu na trenutnoj slici.
- Resetovanje ne dotiče skladište Redis kvota. Tu se knjiga završava sa svojim prozorom ili ističe 60 dana nakon posljednjeg pisanja.
- Kada provajder ne šalje vreme resetovanja, prozor koji se resetuje i ponovo puni iznad stare brojke između dva očitavanja izgleda kao veći broj. Knjiga zadržava staru osnovu i oznake.
- Očitavanja su datirana po lokalnom satu. Kada radi ispred dobavljača, ili izvor prijavi vrijeme resetovanja malo ranije, knjiga se može rano pojaviti do te razlike.
- Rast u tom kratkom rasponu je podijeljen tokenima koji su u njemu usmjerani. Prvo čitanje u sljedećem prozoru to ispravlja. Kada okrenuta knjiga ne sadrži vrijeme resetiranja, toj korekciji je potrebna niža brojka koja je najmanje dva minuta novija od posljednjeg primijenjenog očitanja.
- Instance koje dijele očitanja datuma Redis pohranjuju sa svojim vlastitim satovima, tako da održavajte te satove u sinkronizaciji. Očitavanja instance čiji sat ide unatrag izgledaju starije i zanemaruju se.
- Kada nijedno upotrebljivo očitanje ne stigne nakon pohranjenog vremena resetiranja, procenti udjela po ključu i procentna ograničenja se ne primjenjuju dok se očitanje ne vrati. Bez vremena resetovanja, ovo počinje 15 minuta nakon posljednjeg čitanja koje je promijenilo knjigu.
- U prodavnici Redis, knjiga neaktivna 60 dana može isteći između čeka pisca i njenog pisanja. Zatim se ponovo kreira u reviziji iznad 1, što je važeće stanje.

---

## Plan Resolver

Implementirano u `src/lib/quota/planResolver.ts`.

Prioritet (od najvišeg do najnižeg):

1. **Ručno nadjačavanje baze podataka** — `provider_plans` tabela, po `connectionId`.
2. **Poznati katalog** — `src/lib/quota/planRegistry.ts` (samo podaci).
3. **Prazan plan** — nema dimenzija, potrebna je ručna konfiguracija.

### Poznati katalog

| Provider              | Dimenzije                                                     |
| --------------------- | ------------------------------------------------------------- |
| `codex`               | `percent/5h/100`, `percent/weekly/100`                        |
| `glm`                 | `tokens/5h` (limit=0, unknown), `tokens/weekly`               |
| `minimax`             | `tokens/5h`, `tokens/weekly`                                  |
| `bailian`             | `percent/5h/100`, `percent/weekly/100`, `percent/monthly/100` |
| `kimi`                | `requests/hourly/1500`                                        |
| `alibaba`             | `requests/monthly/90000`                                      |
| `openai`, `anthropic` | Nema podrazumijevanih — potrebna je ručna konfiguracija       |

---

## Integracija cjevovoda

### PRE kuka (`open-sse/handlers/chatCore.ts`)

Pokreće se prije upstream izvršitelja, nakon provjere autentifikacije i politike:

```
resolveComboTargets / handleSingleModel
  → enforceQuotaShare(apiKeyId, connectionId, provider, estimatedCost)
      → getQuotaStore().peek() per dimension
      → fairShare.decideFairShare()
      → if block → return 429 (buildErrorBody, Hard Rule #12)
      → if allow + deprioritize → set quotaSoftPenalty=true on candidate
  → executor.execute()
```

**Fail-open** : ako `enforceQuotaShare` izbaci, zahtjev je dozvoljen kroz `pino.warn` dnevnik. Ovo sprečava grešku u sistemu kvote da blokira sav saobraćaj.

**Kada se kapacitet vrati.** Odbijanje na udjelu ključa ili na plafonu bazena završava se jednom od dvije rečenice, u oba načina posudbe:

- `percent` prozor: `. The <window> window resets at <time>.` Vrijeme je resetiranje provajdera.
- Brojna jedinica: `. Enough <window> usage is expected to clear by <time>.` Vrijeme je gornja granica od kliznog prozora, ako ključ ne šalje ništa drugo.

`<time>` je ISO 8601 trenutak u UTC. Odbijanje tada nosi `Retry-After`: cijele sekunde do tog trenutka, plus jedan. Klijent koji čeka tako dugo pokušava ponoviti najviše jednu sekundu nakon trenutka. Kada trenutak nije poznat, odbijanje ne nosi ni rečenicu ni zaglavlje. Apsolutno odbijanje ograničenja ne nosi ni jedno ni drugo. Javni kod ostaje `quota_share_blocked`.

Odbijanje dijeljenja ne dotiče dijeljenu vezu. Ne postavlja hlađenje, nema zaključavanja modela i kvara provajdera, a ostali ključevi bazena se i dalje služe. Kada svaka meta kombinacije odbije ključ za svoj dio, kombinacija odgovara 429 bez čekanja. Njegov odgovor nosi nagoveštaj kao `Retry-After`. Putanja za ugrađivanje završava svoje odbijanje istom rečenicom i ne šalje `Retry-After`.

### POST kuka (rekordna potrošnja)

Nakon uspješnog odgovora:

```
executor returns success
  → spendRecorder.recordConsumption(apiKeyId, connectionId, provider, actualCost)
      → getQuotaStore().consume() per dimension
      → fail-open: errors logged as pino.warn, never propagated to client
```

**Drift note** : ako `consume` ne uspije nakon odgovora, brojač kotrljanja se smanjuje. Signal zasićenja od provajdera (npr. `anthropic-ratelimit-unified-5h-utilization`) ispravlja globalnu procjenu na sljedeći zahtjev.

### Kombinirana meka kazna (`open-sse/services/combo.ts`)

Kada `decision.deprioritize === true`:

```ts
if (candidate.quotaSoftPenalty) {
  score *= QUOTA_SOFT_DEPRIORITIZE_FACTOR; // default 0.7
}
```

Kazna se primjenjuje nakon svih ostalih faktora bodovanja. Smanjuje vjerovatnoću automatskog kombiniranja odabira zasićenog ključa bez njegovog čvrstog blokiranja.

---

## UI Walkthrough

### `/dashboard/costs/quota-share` — Glavna stranica o bazenima

Komponente (sve u `src/app/(dashboard)/dashboard/costs/quota-share/`):

| Komponenta             | Svrha                                                                                  |
| ---------------------- | -------------------------------------------------------------------------------------- |
| `QuotaConceptCard`     | Uvodna kartica koja objašnjava dijeljenje kvota novim korisnicima                      |
| `CreatePoolModal`      | Kreirajte novi skup kvota (veza + ime + početne alokacije)                             |
| `PoolCard`             | Sažetak po skupu: ime, veza, broj dodjela                                              |
| `DimensionBar`         | Naslagana traka po dimenzijama: udio svakog ključa + globalna upotreba                 |
| `AllocationTable`      | Tabela sa potrošenim, poštenim udjelom, deficit/surplus, zastavicom posudbe            |
| `BurnRateChart`        | EMA linijski grafikon brzine sagorevanja (lijeni ponovni bilježnici putem `dynamic()`) |
| `EditAllocationsModal` | Uredite težine dodjele, ograničenja i politike za skup                                 |
| `BorrowModeField`      | Birač načina posuđivanja (`saturation` ili `consent`) u čarobnjaku                     |
| `LendingBadge`         | Značka samo za čitanje na ključu koji posuđuje, samo u `consent` bazenima              |

Značka pozajmice pokazuje postotak i, kada je postavljen, rok u UTC sa imenovanom zonom. Procjenjuje rok u trenutku snimanja korištenja. Istekao ili nečitljiv rok prikazuje se kao `lending expired`.

Zakačivanje stranice:

- `usePools` — dohvaća `GET /api/quota/pools` svakih 30s.
- `usePoolUsage` — preuzima `GET /api/quota/pools/[id]/usage` na zahtjev.
- `useLocalStoragePoolMigration` — se pokreće jednom na mount radi migracije naslijeđenih LS podataka.

Korak ključeva čarobnjaka bazena ima `Show usage by member to key holders` kutiju. Postavlja `memberBreakdown` opciju bazena (pogledajte [Upotreba člana](#member-usage) ). Ispod njega, čarobnjak upozorava da neko ko zna koji je ključ koristio može uskladiti traku s tim ključem. Kada je polje označeno, tako piše kada korak navodi manje od tri ili više od 20 ključeva, jer trake tada ostaju skrivene. Broji ključeve u koraku i ne može reći koji od njih može podnijeti zahtjeve.

### `/dashboard/costs/quota-share/plans` — Konfiguracija plana provajdera

- `ProviderPlanConfigClient.tsx`: padajući meni za odabir provajdera, prikaz riješenog plana (automatsko iz kataloga ili ručna zamjena) i uređivanje dimenzija.
- Promjene pišu u `PUT /api/quota/plans/[connectionId]`.
- Brisanje se vraća na katalog ili prazan plan.

---

## Kvota za samoposluživanje API (opt-in)

`GET /api/v1/me/quota/{provider}` (također služi na `/v1/me/quota/{provider}`) omogućava API držaču ključa da čita, sa svojim vlastitim ključem, koliki je dio dijeljene pretplate njihova i šta ih blokira. Ruta je tanka ljuska preko `src/server/selfService/quotaHandler.ts`; pogled gradi `src/lib/quota/selfView.ts` i njegov ugovor odgovora je `src/shared/schemas/selfQuota.ts` (`SelfQuotaView` u `docs/openapi.yaml`).

### Omogućavanje i autentifikacija

- Oznaka značajke `QUOTA_SELF_PANEL`, zadani `false`. Dok je isključen, zahtjev koji stigne do rute dobija 404. Sa `REQUIRE_API_KEY=true`, API politika klijenta odbija nedostajući ili nevažeći ključ sa 401 prije pokretanja rute, bez obzira na zastavicu. Zahtjev bez ključa, ali sesije kontrolne ploče s prijavom, propušta tu politiku i dobiva vlastiti odgovor rute. Zastavica se rješava kao i svaka druga zastavica (kontrolna tabla ili REST nadjačavanje, zatim varijabla okruženja istog imena); vidi [`FEATURE_FLAGS.md`](../reference/FEATURE_FLAGS.md).
- Ime za prikaz svakog skupa i oznaka svakog rasporeda vraćaju se vlasnicima ključeva spremišta točno onako kako ih je administrator napisao. Prije nego što uključite zastavicu, provjerite jesu li prikladni za čitanje tih držača ključeva.
- Ključ se čita samo iz zaglavlja: `Authorization: Bearer <key>` ili `x-api-key: <key>`. Kada se oba pošalju, koristi se prvi koji potvrđuje. Ključ u nizu upita ili kolačić se zanemaruje. Serverov ključ okruženja je odbijen (401).
- Ključ treba `self:usage` opseg (403 bez njega).
- Segment provajdera se skraćuje, piše malim slovima i proverava u odnosu na `^[a-z0-9][a-z0-9._-]{0,63}$` (400 inače), a zatim se rešava kroz registar provajdera, tako da pseudonim kao što je `cc` čita `claude` skupove. `claude` i `anthropic` čitaju iste grupe.

### Šta svaka vidljivost pokazuje

| Vidljivost    | Zahteva                                                                          | Polja                                                                                                                                                                                                                                                      |
| ------------- | -------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Vlastiti udio | `self:usage`                                                                     | `pools[]` (ref, ime, dobavljač, politika, težina, ograničenje), `dimensions[].yourShare`, `accounts[]` sa `yourShare` (na `percent` prozoru bez `attributed` i `external`), `blocks`, `availableModels`, `expiresAt`, `apiBaseUrl`                         |
| Nivo računa   | `self:usage` + `self:account-quota`, a dobavljač u ključu `sharedQuotaProviders` | dodaje `dimensions[].total`, `accounts[].dimensions[].account` i `accounts[].modelWindows`, `attributed` i `external` na `yourShare` prozora `percent`, i `members` na skup s uključenim korištenjem članova (pogledajte [Upotreba člana](#member-usage) ) |

- `sharedQuotaProviders` je postavka po ključu (`PUT /api/keys/[id]/self-service`): `null`, zadana vrijednost, znači da svaki provajder do kojeg ključ dođe; `[]` znači ništa. `accountVisible` svakog bazena govori koja se vidljivost primjenjuje na njega.
- Trake računa i prozori modela prikazani su samo za račune čiju vezu ključ može koristiti. Kada ključ ima listu dozvoljenih veza, račun izvan njega zadržava svoj unos `Account N` bez `account` ili `modelWindows`. Prazna lista znači da nema ograničenja, kao za `/v1/me/status`. Ukupni iznos (`dimensions[].total`) ne ovisi o toj listi.
- Dvije figure prikazane samo sa `self:usage` dolaze iz upotrebe drugih ključeva. `exhausted` budžeta rasporeda odražava potrošnju svakog ključa prema tom rasporedu. U grupi čije su težine sve nula, `weight` ključa je `100 / number of members`. I jedno i drugo je ono što se primjena primjene na ključ.
- Skup je identificiran samo pomoću `ref`, neprozirne vrijednosti vezane za pozivni ključ. Njegovo ime za prikaz (`name`) je uključeno onako kako ga je administrator napisao. `ref` je izveden iz ključa i skupa sa tajnom API ključa servera (`API_KEY_SECRET`). Klijenti ne smiju ustrajati na tome: mijenja se ako se ta tajna rotira.
- Računi su navedeni kao `Account 1`, `Account 2`, … po redoslijedu skupa. Ne vraća se ID bazena, ID veze, e-pošta naloga ili ime naloga, a odgovor prolazi kroz šemu ugovora, koja ispušta bilo koje polje izvan njega.
- Prebrojive jedinice (`requests`, `tokens`, `usd`) se prijavljuju kao kantica bazena koju nameće kapija kvote: `limit` = plan limit × računa u grupi, `fairShare` = težina / 100 × `limit` (jednaka podjela kada je svaka težina 0), `consumed` vlastiti brojač = u zq'm ključu `remaining` = `fairShare` − `consumed` na 0.
- `blocks.schedules` navodi prozore rasporeda ključa (`open`/`closed`, `blackout` ili `outside-window`, `retryAfterSeconds`, rezervne spratove i da li je budžet prozora potrošen); `blocks.modelCaps` navodi svoje satnice po modelu sa potrošnjom.
- Ključ izvan svakog bazena provajdera dobija 200 sa `pools: []`; `availableModels` ( `qtSd/` ID-ovi koje ključ vidi u `/v1/models`), `expiresAt` i `apiBaseUrl` su i dalje popunjeni.
- `apiBaseUrl` je `OMNIROUTE_PUBLIC_API_BASE_URL`, zatim `OMNIROUTE_PUBLIC_BASE_URL`, inače `null`. To nikada nije porijeklo zahtjeva.

### `status` i `reason`

| `status`      | Značenje                                                                                                                                                                                                                                                                                                                                                                |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `ok`          | Trenutno očitavanje.                                                                                                                                                                                                                                                                                                                                                    |
| `stale`       | Očitavanje keširanog računa označeno je kao zastarjelo, ili ono čije je vrijeme resetiranja prošlo otkako je pročitan. Brojevi se čuvaju. Jedan prozor modela čije je vrijeme resetiranja prošlo označava cijelu `modelWindows` grupu `stale`. Za vlastiti udio ključa u `percent` prozoru: knjiga je pročitana bez čitanja naloga u kešu kapije da bi se to potvrdilo. |
| `unavailable` | Nema čitanja; brojevi su `null`, nikad `0`. `reason` kaže zašto.                                                                                                                                                                                                                                                                                                        |

| `reason`                          | Kada                                                                                                                           |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| `store_unavailable`               | Skladište kvota nije moglo biti pročitano ili ne može čitati knjige atribucije.                                                |
| `percent_attribution_unavailable` | Vlastiti udio ključa u prozoru `percent` : još ne postoji knjiga atribucije za taj račun i prozor, ili knjiga ne navodi ključ. |
| `percent_window_ended`            | Vlastiti udio ključa u prozoru `percent` : knjiga pripada prozoru plana koji je završio.                                       |
| `account_not_used_by_key`         | Vlastiti udio ključa u prozoru `percent` : veza računa je izvan dozvoljenih veza ključa. Njegova knjiga se ne čita.            |
| `window_not_reported`             | Keš ograničenja dobavljača nema očitavanje za taj prozor plana.                                                                |
| `connection_lookup_failed`        | Nije moguće pročitati vezu računa.                                                                                             |
| `not_supported`                   | OmniRoute ne može čitati ograničenja upotrebe za provajdera naloga.                                                            |
| `fetch_failed`                    | Nijedno keširano čitanje nije bilo upotrebljivo i osvježavanje ograničenja dobavljača nije uspjelo.                            |
| `not_available`                   | Očitavanje nema prozore upotrebe ili račun uopće nema očitavanje.                                                              |

Kada se skladište kvote ne može pročitati, polja `blocks` podržana u skladištu ( `exhausted` budžeta rasporeda, `consumed` i `reached` ograničenja modela) su također `null`.

### Saglasnost za pozajmicu

`PATCH /api/v1/me/quota/{provider}` bilježi vlastitu saglasnost pozivnog ključa za jedan skup. Koristi zastavu, zaglavlja i pravila provajdera `GET`. Opseg `self:usage` ovlašćuje ovo pisanje, iako se njegovo ime čita kao samo za čitanje.

```json
{
  "pool": "qpr_0123456789abcdef0123456789abcdef",
  "lendingPercent": 30,
  "lendingUntil": 1893456000000
}
```

- `pool` je `ref` koji `GET` vraća za taj skup.
- `lendingPercent` je cijeli broj od 0 do 100. Vrijednost 0 briše pristanak i njegov rok. Tijelo sa `lendingPercent` 0 je prihvaćeno u oba načina.
- `lendingUntil` je opciono: epoh milisekundi, ili `null` bez roka. Mora biti u budućnosti i najviše 8640000000000000. Vrijednost ispod 100000000000 čita se kao sekunde i odbija se.
- Bilo koje drugo polje je odbijeno. Telo duže od 4096 bajtova je odbijeno. Čitanje se zaustavlja na toj veličini, tako da se duže tijelo nikada ne drži cijelim.

Provjere se odvijaju po redoslijedu ove tabele. Svako odbijanje koristi standardno tijelo greške sa fiksnom porukom. Odbijanje jedne od ovih provjera ništa ne piše.

| Status | Poruka                                                                                             | Kada                                                            |
| ------ | -------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| 404    | `Not found`                                                                                        | `QUOTA_SELF_PANEL` zastava je isključena.                       |
| 401    | `Valid API key required`                                                                           | Ključ nedostaje ili je nevažeći ili je ključ okruženja servera. |
| 403    | `API key lacks the self:usage scope`                                                               | Ključu nedostaje `self:usage`.                                  |
| 400    | `Invalid provider`                                                                                 | Segment dobavljača je nevažeći.                                 |
| 429    | `Too many lending changes. Retry later.`                                                           | Ključ je prešao granicu. Odgovor nosi `Retry-After`.            |
| 400    | `Body must be { pool, lendingPercent, lendingUntil }. lendingPercent is an integer from 0 to 100.` | Tijelo nije JSON, predugačko je ili se ne podudara sa šemom.    |
| 400    | `lendingUntil must be a Unix time in milliseconds`                                                 | Rok se očitava u sekundama.                                     |
| 400    | `lendingUntil must be in the future`                                                               | Krajnji rok je u ili prije vremena zahtjeva.                    |
| 404    | `Pool not found`                                                                                   | `ref` ne imenuje skup ovog ključa za ovog provajdera.           |
| 403    | `Lending is not enabled for this pool`                                                             | Bazen je u `saturation` modu i `lendingPercent` je iznad 0.     |
| 500    | `Failed to build quota view`                                                                       | Svaki drugi neuspjeh. Njegov uzrok je evidentiran na serveru.   |

Ograničenje je 20 zahtjeva u 60 sekundi za svaki ključ. Svaki zahtjev koji prođe provjeru provajdera se računa, čak i onaj kasnije odbijen ili onaj koji ništa ne mijenja. Ima svoj brojač, osim ograničenja brzine zahtjeva ključa.

Zahtjev koji mijenja pohranjenu saglasnost upisuje jedan `quota.pool.lending.updated` zapis revizije. On imenuje ključ sa starim i novim vrijednostima. Isti organ je dvaput poslao, jednom piše i jednom revidira. Odgovor je 200 sa punim `GET` prikazom, napravljenim nakon pisanja.

`GET` view izvještava o pozajmljivanju na sljedeći način:

- Svaki bazen nosi `borrowMode` (`saturation` ili `consent`) i vlastiti `lendingPercent` i `lendingUntil` ključa.
- `lendingActive` je `true` samo u `consent` skupu, sa procentom iznad 0 i krajnjim rokom nije postignut.
- U `consent` bazenu, svaki prebrojiv `dimensions[].yourShare` nosi `borrowAvailable`. To je ono što ključ sada može koristiti iznad svog udjela, pozajmljenog od drugih ključeva.
- `borrowAvailable` koristi formulu kapije. Čita svaki drugi ključ, također dok je ključ ispod svog dijela. Za `hard` ključ koji je jedno dodatno čitanje po drugom ključu i prebrojiva dimenzija, paralelno.
- `borrowAvailable` je `null` za `soft` ili `burst` ključ, a `null` kada čitanje ne uspije.
- `borrowAvailable` je jedna figura za sve ostale ključeve zajedno. U grupi od dva ključa to je vlastita figura drugog ključa.
- `borrowAvailable` još nije prijavljen za `percent` windows ili `accounts[]`.
- U `saturation` spremištu pogled izvještava o pohranjenom pristanku sa `lendingActive: false` i bez `borrowAvailable`.

### Greške

Every response of this route, success or error, carries `Cache-Control: no-store`. A refusal that happens before the route runs does not carry it, for example the client API policy's 401 or the IP filter's 403. Errors of the route use the standard error body with a fixed message: 400 (invalid provider), 401 (missing or invalid key), 403 (missing `self:usage`), 404 (flag off) and 500 (`Failed to build quota view`). The 500 covers any failure once the request reaches the route, including the key lookup itself; its cause is logged on the server and never returned. The errors of the `PATCH` are listed in [Lending consent](#lending-consent).

### Ograničenja

- `remaining` je dio poštenog udjela ključa koji nije koristio. To nije garancija. Ključ se može poslužiti i izvan njega dok bazen ima mjesta. Jednom kada ukupan iznos bazena dostigne `limit`, svaki ključ bazena se odbija, bez obzira na njegov vlastiti `remaining`, a ključ bez `self:account-quota` ne može vidjeti taj zbroj.
- `remaining` ne uzima u obzir apsolutni `cap` alokacije. Izvršenje odbija ključ kada njegova vlastita potrošnja u prozoru jedinice kapa dostigne vrijednost limita.
- Traka na nivou naloga dolazi iz keša ograničenja provajdera i može kasniti sa odlukom o primeni za nekoliko minuta. Očitavanje čije je vrijeme resetiranja prošlo se prijavljuje kao `stale`.
- Prozori po modelu (`modelWindows`) su prijavljeni samo za dobavljače koji danas imaju mapiranje plan-prozora: Claude i Codex. Za druge provajdere `modelWindows` je i dalje prisutan kada se prikažu podaci o nalogu, sa praznom `windows` listom.
- Vlastiti udio ključa u `percent` prozoru je procjena. Dolazi iz knjige atribucije i nosi sva ograničenja navedena pod "Procentualne dimenzije: atribucija po ključu" iznad.
- `consumed` je broj izvršenja u poređenju sa pravičnim udjelom. To je `attributed` plus `external`, tačno. `attributed` je dio koji knjiga daje ključ za tokene koje je usmjerila. `external` je dio korištenja računa ključa koji ključevi skupa ne uzimaju u obzir.
- Oba dijela se šalju samo kada je `accountVisible` skupa istinit: ključ ima `self:account-quota`, a dobavljač je u svom `sharedQuotaProviders`. Ključ bez njega dobija sam `consumed`, sa istim `status` i `reason`.
- Uz oba dijela i vlastitu težinu, držač može razraditi korištenje izvan bazena koje se naplaćuje na ključeve bazena. Vlasnik s opsegom računa već vidi ukupan iznos računa.
- Ključ koji ništa nije rutirao u prozoru i dalje može čitati svoj vanjski naboj iz `consumed`, jer mu je tada pripisani dio 0.
- Na primjer, knjiga se otvara na 0, a ključevi A i B imaju težinu od 50 svaki. Ključ A usmjerava 900.000 tokena, a ključ B 100.000. Račun tada dostiže 60% ograničenja od 100. Tada je `attributed` 54 za ključ A i 6 za ključ B, a `external` je 0 za oba.
- Pogled čita knjigu i nikada ne piše njeno stanje. Ne otvara knjigu i nikada ne traži od dobavljača čitanje. Sa Redis skladištem, čitanje uklanja zamijenjena revizijska polja u pozadini, kao što to čine čitanja kapije.
- Udio je `ok` samo dok keš kapije drži očitavanje računa. Bez jednog to je `stale`, tako da se u grupi bez nedavnog zahtjeva prikazuje kao moguće zastarjelo.
- Dok zahtjev ne prođe kroz skup, dionica je nedostupna. Taj zahtjev otvara knjigu, a broj računa u tom trenutku se računa kao korištenje izvan bazena.
- U grupi s nekoliko računa, svaki unos računa koristi vlastitu knjigu tog računa i ograničenje jednog računa. Provedba mjeri obje strane prema broju računa, tako da je proporcija ista.
- Prozori po modelu nemaju udio za ključ. Knjiga ne sadrži podatke po modelu.
- Rezervni spratovi rasporeda se ne vrednuju pogledom: raspored se može prikazati kao `open` dok je zahtev odbijen sa razlogom `schedule-reserve`.
- Kada dva skupa istog ključa dijele vezu, primjena primjenjuje jedno od njih, a pogled navodi oba.
- Ne postoji ograničenje po adresi za neuspjele pokušaje ključa: iza obrnutog proksija pozivaoci mogu dijeliti jednu adresu (zavisi od toga da li su proslijeđene klijentske adrese pouzdane), tako da bi zaključavanje moglo uskratiti rutu svakom držaču ključa. Sa `REQUIRE_API_KEY=true`, API politika klijenta odbija nevažeći ključ prije pokretanja rute, s tijelom te politike 401 umjesto ove rute.

### Upotreba članova

Administrator može dozvoliti vlasnicima ključeva da vide kako se korištenje prozora dijeli između članova skupa. Opcija je `memberBreakdown` bazena, po defaultu isključena. Postavlja se u čarobnjaku bazena ili sa `PATCH /api/quota/pools/{id}`. `GET /api/quota/pools` i `GET /api/quota/pools/{id}` to prijavljuju.

Dimenzija pogleda nosi `members` samo kada sve ovo ima:

- opcija bazena je uključena
- bazen ima najviše 20 dodijeljenih ključeva, a najmanje tri od njih mogu postavljati zahtjeve: aktivni, nisu opozvani, nisu zabranjeni i nisu istekli
- `accountVisible` bazena je istinit: ključ ima `self:account-quota` i provajder je u svom `sharedQuotaProviders`
- u prozoru `percent`, veza naloga je jedna od ključeva koje može koristiti
- pročitan je vlastiti udio ključa u tom prozoru: njegov `status` nije `unavailable`

Inače `members` je odsutan. Nikada nije prazna lista.

- Svaka kriška je `{ slot, consumed, isYou }`. Shema odgovora odbija bilo koje drugo svojstvo na isječku i listu od više od 20 isječaka. Slice su navedene po redoslijedu utora.
- Postoji jedan odsječak po dodijeljenom ključu, uključujući ključ koji više ne može postavljati zahtjeve. Član bez upotrebe pokazuje pravu nulu.
- Slot 1 je uvijek ključ za traženje, sa `isYou` true. Ostali brojevi slotova su rangovi heša s ključem. Ključ je `API_KEY_SECRET` i pokriva bazen, ključ za traženje i član.
- Dakle, brojevi se ne slažu između nositelja. Za jednog nosioca ostaju isti između posjeta. Mogu se promijeniti kada se ključ pridruži ili napusti bazen, ili kada se ta tajna rotira.
- U prozoru koji se može brojati, isečak je brojač člana u skladištu kvota, isti brojač kao i njegov sopstveni `consumed`.
- Na prozoru `percent` slice je `attributed` dio člana, iz iste knjige koji se čita kao vlastiti dio ključa. Upotreba izvan bazena nikada se ne dijeli na kriške. Taj naboj je podijeljen po težini, tako da bi kriške koje su ga nosile pokazale težine.
- Svaki pogled čita jednu vrijednost po drugom članu i prebrojivom prozoru, paralelno. Na prozoru `percent` kriške ne koštaju čitanje osim pročitane knjige koju je dionica pročitala. Kada se jedna vrijednost ne može pročitati, taj prozor nema `members`, a vlastiti udio ključa ostaje.
- Opcija i broj upotrebljivih ključeva se čitaju jednom po spremištu, i to samo za ključ koji može vidjeti podatke računa. Neuspješno čitanje opcije ili broja upotrebljivih ključeva isključuje trake za taj skup. Server bilježi upozorenje, a ostatak pogleda je izgrađen.

Barovi nemaju imena ili ID. Oni i dalje govore ključnom nosiocu stvari o drugim članovima:

- Nosioci i dalje mogu upariti kriške po njihovim vrijednostima.
- Stabilno numerisanje omogućava nosiocu da prati jednog člana tokom vremena.
- Broj rezova pokazuje koliko je ključeva dodijeljeno u bazen.
- U grupi od tri ključa, neko ko zna šta je koristio jedan ključ može reći šta je poslednji ključ koristio.
- Kada bazen padne ispod tri upotrebljiva ključa, šipke nestaju. Pregledi snimljeni ranije i dalje pokazuju šta je svaki član koristio.
- U prozoru koji se može brojati, ukupni skup minus rezovi mogu pokazati upotrebu ključeva koji više nisu dodijeljeni.
- Član koji pokazuje nulu na jednom računu, a koristi na drugom može pokazati koji član koristi koji račun.
- U prebrojivom skupu sa politikom `hard`, dio koji prestaje rasti na poštenom udjelu člana ukazuje na težinu tog člana.

### Serija upotrebe (`GET /api/v1/me/usage`)

`GET /api/v1/me/usage?range=<range>` (također služi na `/v1/me/usage`) vraća upotrebu i cijenu vlastitih zahtjeva pozivnog ključa: ukupne vrijednosti, jedan unos po UTC danu, po danu i modelu, po modelu i po provajderu. Dijeli zastavu, pravila provjere autentičnosti, `self:usage` opseg, `Cache-Control: no-store` i ponašanje greške gornje rute kvote. Ključ se provjerava prije `range`. Greške su 400 (`Invalid range`), 401, 403, 404 i 500 (`Failed to build usage`).

- `range` je jedan od `1d`, `7d`, `30d` (podrazumevano) ili `90d`. Bilo koja druga vrijednost, prazna vrijednost ili ponovljeni parametar je 400. Skup se zaustavlja na `90d` da bi se ograničila cijena poziva. Pogled čita samo neobrađenu istoriju korišćenja, nikada dnevne sažetke, koji nemaju ključ.
- Redovi se biraju prema ID-u pozivnog tastera. Kolona imena ključa se nikada ne podudara, a redovi snimljeni bez ID-a ključa se nikada ne broje.
- Izgradnja serije pokreće pet grupisanih upita nad redovima ključa u prozoru. Izgrađena serija se ponovo koristi 60 sekundi po ključu i opsegu, a ponovno korišteni poziv ne pokreće nijedan. Njegova `generatedAt` daje starost.
- Prozor se završava kada je serija izgrađena. Red utisnut kasnije, na primjer nagibom sata, se ne računa.
- `coverage.retentionDays` je operatorova neobrađena postavka zadržavanja istorije upotrebe (`retention.usageHistory` u postavkama baze podataka). `coverage.truncatedByRetention` je istinit kada je traženi raspon duži od te postavke. On uspoređuje dva broja i ne provjerava da li zaista nedostaju redovi.
- Provajder se vraća kao snimljen za sopstvene zahtjeve ključa. Model je snimljeno ime nakon posljednjeg `/`, a redovi su grupirani po njemu. Kombinirani zahtjev čiji je svaki cilj odbijen se bilježi s oznakom rutiranja kao provajderom (ime kombinacije, `auto` ili `combo`) i nizom modela koji je klijent poslao. Ostali odbijeni zahtjevi, na primjer zbog otvorenog prekidača, hlađenja modela ili preskakanja kvote, zadržavaju ciljnog dobavljača i model.
- Osim brojanja i troškova, odgovor nosi prosječno kašnjenje, stope uspješnosti i vremena prvog i posljednjeg zahtjeva.
- `byModel` navodi 50 parova dobavljač i model s najviše zahtjeva. Sa više parova, njegovi unosi ne zbrajaju `summary`, a `summary.uniqueModels` broji svaki snimljeni model pravopisa. `byModelTruncated` je tada istinit, a model čiji parovi padaju na obje strane reza pokazuje djelomične ukupne vrijednosti.
- Prijavljena su dva troška. `costUsd` je fakturisani trošak, kako to pokazuje analitika korišćenja. Provajderi fiksne pretplate, kao što je plan Claude Code, računaju 0 dolara tamo. `listPriceUsd` je ista upotreba po cijeni po maloprodajnoj cijeni, uključujući pretplate. Zahtjev čiji model nema red cijene računa njegov pohranjeni trošak: trošak koji je provajder prijavio ili onaj koji je izračunat kada je zahtjev zabilježen. Samo zahtjev sa nijednim broji 0, bez markera, tako da zbir može biti djelomičan.
- Ugovor odgovora je `src/shared/schemas/selfUsage.ts` (`SelfUsageSeries` u `docs/openapi.yaml`).

### Samouslužna stranica

Kada je `QUOTA_SELF_PANEL` uključen, `/quota/{provider}` je javna stranica. Držač ključeva tamo upisuje API ključ i vidi skupove tog ključa za provajdera. Svaki bazen prikazuje jednu karticu po prozoru bazena, s korištenjem bazena za svakoga i vlastitim udjelom ključa. Svaki račun pula ima svoje kartice, sa korištenjem računa i udjelom ključa. Upotreba računa se pojavljuje samo kada ključ može vidjeti podatke o računu. Stranica također navodi ograničenja po modelu za svaki račun i vlastitu upotrebu ključa. Pojavljuje se obavijest kada raspored blokira ključ upravo sada. Kartica navodi svaku kapicu ključa po modelu s njegovom upotrebom i označava one koje su dosegnute. `{provider}` je id dobavljača ili njegov pseudonim (`/quota/claude`, `/quota/cc`). Nepoznati provajder i svaka `/quota/*` putanja dok je zastavica isključena, odgovorite na 404. Skupovi na prilagođenom OpenAI- ili Anthropic-kompatibilnom čvoru nemaju stranicu. API i dalje odgovara umjesto njih.

Stranica nema sesiju. Ključ se šalje samo u `Authorization` zaglavlju `GET /api/v1/me/quota/{provider}`, `PATCH /api/v1/me/quota/{provider}` i `GET /api/v1/me/usage`, nikada u URL. Ključ koji server prihvata čuva se u `sessionStorage` kartici. Sa "Zapamti na ovom uređaju" umjesto toga se čuva u `localStorage`, a "Zaboravi ključ" ga uklanja iz oba. Ključ koji server odbija uklanja se iz skladišta.

Pul u `consent` modu prikazuje kreditnu karticu. Tu nosilac ključa postavlja cijeli postotak od 0 do 100 neaktivnog udjela ključa za pozajmljivanje. Vlasnik također bira koliko dugo će saglasnost trajati: dok se ne isključi, 1 sat, 8 sati, 24 sata, 7 dana ili 30 dana. Trajanje se računa od trenutka pohranjivanja. Dok je rok na snazi, nosilac ga može zadržati. Ako taj rok prođe prije Save, kartica ne šalje ništa i traži drugi izbor. Sa 0% se ne šalje rok. Kartica prikazuje pohranjeni rok sa naznačenom vremenskom zonom. Saglasnost čiji je rok istekao se prikazuje kao završena.

Za `hard` ključ, kartica također navodi, po prozoru bazena, koji drugi ključevi sada posuđuju ključu. Svaki red je jedna figura za sve ostale tipke zajedno. U grupi od dva ključa to je vlastita figura drugog ključa. Broj koji prikaz ne prijavljuje čita se kao nedostupan, a ne kao nula. Za ključ `soft` ili `burst` kartica kaže da se ne primjenjuje nikakva brojka.

Grupa u `saturation` modu čiji ključ pohranjuje postotak iznad 0 pokazuje samo povlačenje. Piše da pohranjeni postotak tu nema efekta. Njegovo dugme za povlačenje šalje 0 bez roka. Pul u `saturation` modu sa pohranjenim 0 ne prikazuje kreditnu karticu. Nakon spremanja, kartica koja vraćenom pregledu više nije potrebna ostaje sa svojom porukom sve dok se ponovo ne promijeni prikaz stranice.

Ništa se ne pohranjuje dok držalac ne pritisne Sačuvaj ili Povuci. Svaki pritisak šalje jedan `PATCH /api/v1/me/quota/{provider}` zahtjev, a drugi pritisak ne šalje ništa dok je prvi na čekanju. Tijelo nosi neprozirni `ref` bazena iz pogleda, procenta i roka. Odgovor je obnovljeni prikaz kvote, a stranica ga prikazuje bez drugog čitanja. Kada se dva snimanja preklapaju, stranica čita kvotu jednom nakon posljednjeg odgovora. Stranica ne čuva saglasnost u memoriji pretraživača.

Odbijena promjena je objašnjena na kartici tekstom odabranim iz statusa HTTP. Tijelo greške se ne čita. 401 kaže da ključ nije prihvaćen i ponovo učitava kvotu. 403 kaže da fond ne prima promjene zajmova, a 404 kaže da je fond nestao. Oba nude dugme koje ponovo učitava kvotu. 400 ili drugi 4xx odgovor traži od vlasnika da provjeri postotak i rok. A 429 traži od nosioca da sačeka, sa sekundama `Retry-After` kada ih dobije odgovor. Odgovor 5xx, 408 ili greška mreže govori da promjena možda nije sačuvana i zadržava upisane vrijednosti. Odgovor izvan ugovora ponovo učitava kvotu. Neuspješno spremanje ne uklanja ključ samo po sebi. Kada je ponovno učitavanje nakon što je odbijeno, stranica uklanja ključ kao kod svakog odbijenog čitanja.

Kada se ključ prihvati, stranica također prikazuje karticu "Podesite svoje alate" sa tri kartice. "Claude Code" daje `env` blok za `~/.claude/settings.json`. "Shell" daje iste varijable kao `export` linije. "Claude Desktop" daje vrijednosti za svoj prozor za zaključivanje treće strane. Modeli su modeli podjele kvote koje ključ može pozvati za tog provajdera. Kada takva lista ne dolazi s ključem, blok umjesto toga uključuje otkrivanje modela pristupnika. Adresa mrežnog prolaza je javno API porijeklo o kojem server prijavljuje (`OMNIROUTE_PUBLIC_API_BASE_URL`, zatim `OMNIROUTE_PUBLIC_BASE_URL`). Kada nije postavljeno nijedno, kartica prikazuje čuvar mjesta i govori vlasniku da pita administratora. Ključ se prikazuje kao čuvar mjesta. "Uključi moj ključ" stavlja cijeli ključ u tekst na ekranu iu ono što kopira dugme. To traje sve dok se kutija ne obriše, ključ se ne zaboravi ili zamijeni ili se stranica ne ostavi. Kartica ne šalje zahtjeve i ne nudi preuzimanje datoteka.

Čitanje API oznaka `stale` je prikazano kao moguće zastarjelo. Očitavanje koje označava `unavailable` prikazano je sa svojim razlogom, nikada kao nula.

Na procentualnim planovima stranica izvlači vlastiti udio ključa kada ga API prijavi. Kaže da je broj procjena i imenuje njegova dva dijela. Ograničenja po modelu prikazuju samo račun.

Kada prozor nosi `members`, njegova kartica također prikazuje traku sa jednim segmentom po članu, po redoslijedu utora. Segment ključa upita koristi boju akcenta. Ostali segmenti kruže kroz boje dijagrama teme. Legenda teksta navodi svaki segment sa njegovom vrijednošću, tako da ništa ne ovisi o boji. Segmenti su označeni `You` ili `Member N`, gdje je N slot.

### Namjenski port za stranicu

`QUOTA_PANEL_PORT` otvara drugi slušalac koji opslužuje samo samoposlužnu stranicu. Isključeno je osim ako nije postavljena varijabla. `QUOTA_PANEL_HOST` je adresa povezivanja i podrazumevano je `127.0.0.1`.

Slušatelj prenosi ove staze na glavni port i odgovara 404 za svaku drugu putanju:

| Put                                                                      | Služi                              |
| ------------------------------------------------------------------------ | ---------------------------------- |
| `/quota/{provider}`                                                      | Stranica                           |
| `/api/v1/me/quota/{provider}`, `/v1/me/quota/{provider}`                 | Prikaz kvote na stranici           |
| `/api/v1/me/usage`, `/v1/me/usage`                                       | Serija upotrebe koju stranica čita |
| `/_next/static/`                                                         | Skripte, stilovi i fontovi izrade  |
| `/favicon.ico`, `/favicon.svg`, `/icon-512.png`, `/apple-touch-icon.png` | Ikone                              |

`GET` i `HEAD` se prenose bez tijela. Prenosi se i jedan zahtjev sa tijelom: `PATCH` putanje prikaza kvote, koju stranica šalje da sačuva izbor pozajmljivanja. Bilo koja druga metoda odgovara na 404, osim na CONNECT zahtjev, čija je veza zatvorena bez odgovora. Svaki drugi zahtjev koji deklarira tijelo odgovara na 404 i njegova veza je zatvorena. Zahtjevi za nadogradnju se odbijaju i njihova veza je zatvorena. Odbijen je put sa segmentom tačke ili markerom fragmenta, kao na API portu. Tako je i cilj zahtjeva sa karakterom izvan ASCII za ispis. Na sirovi kontrolni znak u cilju HTTP parser odgovara 400, prije vlastite provjere ovog porta. Zaglavlja zahtjeva koja okvir rezerviše za vlastitu upotrebu se ne prenose: imena koja počinju sa `x-middleware-`, `x-invoke-`, `x-nextjs-`, `x-now-` ili `x-next-`, i imena `x-matched-path` i `next-resume`. Zahtjev se prenosi bez njih. Kontrolna tabla, stranica za prijavu, API za upravljanje i rute zaključivanja ne mogu se pristupiti preko ovog porta.

`PATCH` mora nositi `Content-Type: application/json`, bez parametra ili samo sa `charset=utf-8`. Mora nositi jedan `Content-Length` od 1 do 4096, napisan kao obične cifre, a ne `Transfer-Encoding`. `PATCH` koji krši jedno od ovih pravila odgovara 404. Na neke krivo oblikovane dužine, kao što je potpisana ili ponovljena, HTTP parser odgovara 400 prije vlastite provjere ovog porta. Port čita deklarirane bajtove prije nego što kontaktira glavni port i čeka na njih najviše 5 sekundi. Tijelo koje do tada nije kompletno odgovara na 404 i njegova veza je zatvorena. Ništa ne stiže do glavnog porta u tom slučaju, ili kada klijent napusti prvi. Port prenosi tačno deklarisane bajtove, sa istim `Content-Length`. Bajtovi nakon njih se čitaju kao sljedeći zahtjev na vezi. TLS obrnuti proxy ispred mora proslijediti `Content-Length` i ne smije ponovo razdvojiti tijelo zahtjeva. Glavni port provjerava API ključ u `Authorization` zaglavlju, kao i za `GET`.

Tijelo 404 je `{"error":"not_found","message":"Not found."}`. Neuspjeli relej odgovara na 502 (`api_bridge_unavailable`) ili 504 (`api_bridge_timeout`) bez polja `detail`.

Slušalac ne čita `QUOTA_SELF_PANEL` i ne uključuje stranicu. Dok je zastavica isključena, stranica i njen API odgovaraju na 404 na glavnom portu, a slušalac prenosi taj odgovor.

Pod razvojnim serverom (`next dev`), stranica ne postaje interaktivna preko ovog porta. Razvojni hot-reload socket je zahtjev za nadogradnju, a port ga odbija. Koristite glavni port dok razvijate.

Port služi običan HTTP, a stranica šalje API ključeve. Zadržite zadanu adresu povezivanja i stavite obrnuti proxy sa TLS ispred njega. Adresa povezivanja koja nije loopback bilježi ovo obavještenje:

```text
[Quota Panel] Bound to <host>. This port serves plain HTTP and the page sends API keys. Put a TLS reverse proxy in front of it.
```

Peer koji ne šalje zaglavlje za prosljeđivanje računa se kao lokalni na glavnom portu. Dakle, proxy na istom hostu mora poslati `X-Forwarded-For`. Proxy na privatnoj adresi je pouzdan za to zaglavlje samo sa `OMNIROUTE_TRUST_PROXY=private` (ili `lan`). Bilo koji drugi peer se prijavljuje putem adrese njegove veze, a zaglavlja prosljeđivanja koje je poslao se izbacuju.

Slušalac istovremeno ima najviše 256 veza. Klijent ima 10 sekundi da pošalje zaglavlja zahtjeva i 30 sekundi da pošalje cijeli zahtjev. Veza koja se održava u stanju mirovanja se zatvara nakon otprilike 5 sekundi. Veza bez aktivnosti 60 sekundi je zatvorena. Ove vrijednosti su fiksne. Postavite ograničenja veze i brzine na obrnutom proxyju također ispred. Obrnuti proxy ispred trebao bi zadržati svoje neaktivne uzvodne veze manje od 5 sekundi ili ih ne koristiti ponovo. Relej glavnog porta koristi uzvodno vremensko ograničenje API porta (`API_BRIDGE_*`).

Slušatelj se također pokreće kada `API_PORT` nije postavljena. `QUOTA_PANEL_PORT` mora biti port od 1 do 65535, napisan samo ciframa. Mora se razlikovati od porta na kontrolnoj tabli i API porta. Dok je živi WebSocket server uključen, on se također mora razlikovati od `LIVE_WS_PORT` (podrazumevano 20132). Bilo koja druga vrijednost ne otvara ništa i bilježi upozorenje. Upozorenje o odbijenoj vrijednosti imenuje varijablu i ne ponavlja vrijednost. Port koji je već u upotrebi ne otvara ništa i bilježi ovo upozorenje:

```text
[Quota Panel] Port <port> is already in use. The quota panel port stays off.
```

Sa `OMNIROUTE_BASE_PATH` skupom, slušalac očekuje svaku putanju iznad pod tim prefiksom. Koristite isti `OMNIROUTE_BASE_PATH` u vrijeme izgradnje iu vrijeme izvođenja. Napišite ga s početnom kosom crtom i bez kose crte na kraju, na primjer `/omniroute`. Drugi oblik, uključujući `/` i `/omniroute/`, ostavlja port isključen upozorenjem, iako build prihvata te forme. Kao i osnovna staza čiji prvi segment imenuje rutu aplikacije: `api`, `v1`, `v1beta`, `_next`, `quota`, `dashboard`, `docs`, `login`, `codex`, `responses`, `anthropic`, `openai`, `v0` ili `connect`, u svakom slučaju.

Ograničenja:

- `/quota/{provider}/` sa kosom crtom na kraju odgovara 404 na ovom portu.
- Servisni radnik i manifest web aplikacije se ne poslužuju na ovom portu.
- Prilagođeni favicon postavljen na kontrolnoj tabli nije prikazan na ovom portu.
- Ikone se ne prikazuju kada aplikacija radi pod osnovnom putanjom.
- Luka govori jednostavno HTTP/1.1.
- Vezanje koje ne uspije se ne pokušava ponovo sve dok se proces ponovo ne pokrene.
- Slušatelj nema vezu ili ograničenje brzine po adresi klijenta.
- Podešavanje kontejnera nije obuhvaćeno ovim odeljkom.

---

## Varijable okruženja

| Varijabilna                          | Default           | Opis                                                                   |
| ------------------------------------ | ----------------- | ---------------------------------------------------------------------- |
| `QUOTA_STORE_DRIVER`                 | `sqlite`          | Driver za korištenje: `sqlite` ili `redis`                             |
| `QUOTA_STORE_REDIS_URL`              | _(prazno)_        | Redis URL, npr `redis://localhost:6379`                                |
| `QUOTA_SATURATION_THRESHOLD`         | `0.5`             | 0..1; `>= threshold` aktivira strogi način rada                        |
| `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` | `1000`            | Tokeni koji objašnjavaju najviše jednu tačku prozora plana procenta    |
| `QUOTA_SOFT_DEPRIORITIZE_FACTOR`     | `0.7`             | 0..1; množitelj za soft-policy combo rezultat                          |
| `QUOTA_CONSUMPTION_RETENTION_DAYS`   | `14`              | Danima prije nego što GC ukloni stare `quota_consumption` kante        |
| `QUOTA_PANEL_PORT`                   | _(nepostavljeno)_ | Namjenski port za samoposlužnu stranicu. Unset znači da nema slušaoca. |
| `QUOTA_PANEL_HOST`                   | `127.0.0.1`       | Vezati adresu za taj port                                              |

DB postavke (`quotaStore.*`) nadjačavaju env vars.

---

## Rješavanje problema

### Redis je konfigurisan, ali se ne povezuje

Provjerite da li je `ioredis` instaliran (`npm ls ioredis`) i da li je `QUOTA_STORE_REDIS_URL` dostupan. U slučaju neuspjeha povezivanja, fabrika se vraća na SQLite (zabilježeno pod `warn`).

### `peek` vraća zastarjele podatke / fail-open

Ako `peek` baci izuzetak, `enforceQuotaShare` tretira rezultat kao "dozvoli" (`fail-open`). Provjerite `pino` logove za unose `quota:enforce` i `quota:factory` kako biste identifikovali osnovni uzrok.

### Odstupanje brojača potrošnje

Ako se stvarna upotreba provajdera razlikuje od brojača, to je očekivano — klizni prozor sa 2 bucket-a ima ~1% greške na granicama prozora, a `consume` je "fire-and-forget" nakon odgovora. Signal zasićenja (`saturationSignals.ts`) čita stvarnu iskorištenost provajdera sa TTL-om od 30s i prilagođava `globalUsedPercent` u skladu s tim.

### Grupa prikazuje "nema podataka" za stopu sagorijevanja

`computeBurnRate` zahtijeva najmanje 2 historijska uzorka. Nove grupe bez prethodnih `consume` poziva prikazat će `tokensPerSecond: 0` i `timeToExhaustionMs: null`.

## Migracija iz localStorage

Kada se `/dashboard/costs/quota-share` prvi put učita, hook `useLocalStoragePoolMigration` provjerava:

1. `localStorage.getItem("omniroute:quota-share:pools")` nije prazan.
2. `GET /api/quota/pools` vraća `[]` (DB je prazna).

Ako su oba uslova ispunjena, šalje svaki naslijeđeni pool na `POST /api/quota/pools` u batch-u, a zatim uklanja localStorage ključ. Migracija je idempotentna: uslov 2 sprječava ponovnu migraciju.

---

## Klasifikacija interne strategije

`quota-share` je **isključivo interna** strategija rutiranja (`INTERNAL_ROUTING_STRATEGY_VALUES` u `src/shared/constants/routingStrategies.ts`). Koristi se isključivo za `qtSd/` pool kombinacije koje kreira sistem i namjerno je isključena iz `ROUTING_STRATEGY_VALUES` tako da se nikada ne pojavljuje kao opcija koju korisnik može odabrati u UI-u ili API-ju.

---

## Test Coverage

Dva sloja automatiziranog pokrivanja broda s motorom za podjelu kvota:

| Suite                 | Command                                                                | Šta pokriva                                                                                                                                                                                                             |
| :-------------------- | :--------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Jedinica (29 testova) | `node --import tsx/esm --test tests/unit/quota-share-strategy.test.ts` | DRR planer, gating zasićenja, ograničenja konkurentnosti, fairShare matematika, zaostali red čekanja                                                                                                                    |
| Integraciona matrica  | `npm run test:combo:matrix`                                            | Odluka o rutiranju od kraja do kraja kroz pravi kombinovani cevovod; DRR pravičnost + određivanje prioriteta zasićenja putem šavova uživo (`registerQuotaFetcher`, `setLKGP`, `__setHeadroomSaturationFetcherForTests`) |

Matrica integracije radi u CI zajedno sa sve 22 javne strategije. Jedinica se može pokretati samostalno.

---

## DB sažetak sheme

Tri tabele dodane migracijama `078`, `079` i `085`:

- `quota_pools` + `quota_allocations` — definicije spremišta i dodjele po ključu.
- `quota_consumption` — kotrljajući brojači sa 2 kašike po `(apiKeyId, dimensionKey)`.
- `provider_plans` — ručni plan dobavljača poništava (dimenzije JSON po connectionId).

Sve tabele dodane putem idempotentnih `CREATE TABLE IF NOT EXISTS` migracija.

Privoljeno pozajmljivanje dodaje tri kolone: `quota_allocations.lending_percent` (cijeli broj, zadano 0), `quota_allocations.lending_until` (milisekunde epohe ili `NULL` bez roka) i `quota_pools.borrow_mode` (zadano `saturation`). Njegova migracija samo dodaje ove stupce i ne upisuje nijedan postojeći red.

Knjiga procenta atribucije dodaje `quota_percent_ledger` (jedan red po grupi, računu i prozoru plana) i `quota_percent_ledger_tokens` (jedan brojač tokena po grupi, računu i API ključu). `src/lib/db/quotaPercentLedger.ts` ih čita i piše.
