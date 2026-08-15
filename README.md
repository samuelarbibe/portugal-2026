# Portugal — 4–13 October 2026

Planning context for a 9-night trip, 2 adults. This README is written to be dropped into
an AI agent as context; `index.html` is the live deliverable.

- **Land** OPO, Sun 4 Oct, 09:00
- **Depart** LIS, Tue 13 Oct, 22:15
- **9 nights, five bases** — Porto 2 · Pinhão 1 · Coimbra 1 · Batalha 1 · Lisbon 4

**Live site:** https://samuelarbibe.github.io/portugal-2026/

## The file

`index.html` is a **self-contained single-file site** — embedded CSS and JS, no build step,
opens from `file://` as happily as over HTTP, prints cleanly via `@media print`.

The booking checklist persists ticks in `localStorage` under keys `pt26.<data-k>`. Storage
is scoped to origin, so **the hosted copy and the local copy keep separate checklists**.
The working copy lives at **`~/Downloads/portugal-trip-2026.html`** and **must keep that exact
path** — the checklist ticks are keyed to it. This repo (**`~/Documents/Workspace/portugal-2026`**)
holds a snapshot published to Pages: copy the working file over `index.html`, re-insert the robots
meta tag before `<meta name="viewport">`, commit, push.

The overview strip is a 20-column CSS grid: 10 day cells spanning 2 columns each, plus
9 night chips offset one column (`grid-column:2i / span 2`) so each night visually
straddles the two days it joins.

The page carries `<meta name="robots" content="noindex, nofollow, noarchive">`. The site is
public to anyone with the URL — that tag only keeps it out of search results.

## Standing constraints — do not re-litigate

- **No wine-focused activities.** The Douro is for scenery, not tastings. Ask for
  non-alcoholic pairings at restaurants.
- **Minimal private drivers — inside cities only.** Self-drive between cities.
- **One rental car only:** collected in Porto 6 Oct 09:30, dropped at LIS airport Fri 9
  (booked to 20:30). **Lisbon is entirely car-free.**
- Mid-range boutique hotels / Airbnbs. Avoid Six Senses — too wine-led.
- Cities + nature + food in roughly equal measure; moderate hiking wanted.
- Check into the hotel on arrival day before going out.
- **The traveller books everything themselves** and reports back. Recommend and compare;
  do not book.

## Bookings

| Nights | Where | Property |
|---|---|---|
| 1–2 · 4–6 Oct | Porto | **NOLIA Boutique Hotel** |
| 3 · 6 Oct | Pinhão, Douro | **The Vintage House** — dinner at the Rabelo, Tue 6 20:00, booked |
| 4 · 7 Oct | Coimbra | **Airbnb "Studio King Deluxe"**, host Nuno Miguel, R. Lourenço de Almeida Azevedo 5. In after 15:00, **out by 11:00 — early and firm** |
| 5 · 8 Oct | Batalha | **Hotel Lis Batalha**, Double Room Mansarda, Largo do Mestre Afonso Domingues (the monastery square). +351 244 765 260 |
| 6–9 · 9–13 Oct | Lisbon | **"HUL · Chiado"** Airbnb, room `4902781`, Rua Nova da Trindade block. Lockbox self check-in |

Tue 13 is a Lisbon day with no night — Uber to LIS 18:45.

## ⚠ Live item — 7 Oct is booked three times, deliberately

Three rooms are held for Wed 7. **Decision deferred (15 Aug): the traveller is holding all
three until the start of October, while cancellation is free.** Do not push them to cancel
now — that is their call and it is a reasonable one.

1. **Airbnb "Studio King Deluxe"**, Coimbra — **the main line.** The whole written plan
   assumes it. Most generous cancellation window, so safe to hold longest.
2. **Palace Hotel do Bussaco**, Luso — the only night left that could absorb the ~€700–1,000
   of unspent splurge, which is the real argument for keeping it held. **Also the risk:**
   direct palace bookings commonly use a **14- or 21-day** window = **23 or 16 September**
   for a 7 Oct arrival, i.e. possibly already past by "start of October".
3. **Vila Julieta Guesthouse** — Booking.com, 20 Alameda Conchada. **Auto-charges** when its
   window closes, and holds no option the Airbnb doesn't hold better. Let this one go first.

**What the decision drives:** not just the bed. The **Biblioteca Joanina 09:00 slot**,
**Tomar** and the **Mira de Aire** timing all assume waking in Coimbra, so nothing on
Thursday can be locked until this lands. Pick Bussaco and Thursday is rebuilt from scratch.

**Bussaco was briefly written as the main line and reversed the same day. Don't re-argue
it unasked.** Coimbra buys **Tomar** (unreachable from Luso), the Coimbra evening, and the
09:00 Joanina slot from ten minutes below the university gate. It costs the Buçaco forest
walk — reduced to an optional 30-minute roadside stop on Wednesday — and Mealhada's leitão.

A durable reminder is set for **20 Sept 2026** to force the decision before any plausible
14-day deadline.

## Route

```
  Sun 4   Mon 5   Tue 6   Wed 7   Thu 8   Fri 9   Sat 10  Sun 11  Mon 12  Tue 13
 ┌───────────────┬───────┬───────┬───────┬───────────────────────────────────────┐
 │     PORTO     │ ▸Douro│▸Coimbra│▸Batalha│             LISBON                  │
 └───────┬───────┴───┬───┴───┬───┴───┬───┴───────────────────────────────────────┘
    N1 N2 ·  NOLIA    N3 ·    N4 ·    N5 ·      N6  N7  N8  N9 · HUL Chiado
             Porto   Pinhão  Coimbra Batalha         (car-free)
                       │       │       │
                    Vintage  Studio   Hotel    car returned at LIS on Fri 9
                     House    King     Lis
```

Key legs: Porto Boavista→Arouca 1h05 (Passadiços do Paiva)→Pinhão · N222 driven both directions ·
Folgosa→Galafura→Viseu 1h20 · Viseu→Coimbra 1h15 · Coimbra→Tomar 1h10 ·
Tomar→Mira de Aire→Batalha 1h10 · Batalha→Alcobaça→Nazaré 0h45 ·
Nazaré→Óbidos→LIS 1h40.

## Day shape through the middle

- **Wed 7** — Casal de Loivos climb 07:45 · rabelo cruise 11:00 · station azulejos ·
  N222 west · **DOC at Folgosa as lunch, 13:15** (en route south; lunch service is the
  reliable one in shoulder season) · Galafura 15:20 · **Viseu 16:45** (Sé, Rua Direita;
  Grão Vasco closes 18:00) · **17:45 the fork** — IP3 straight down puts you in Coimbra at
  19:00, or the A25/A1 via the Mealhada exit puts you at **Buçaco 18:35** for a 30-min
  Fonte Fria walk and Coimbra at 19:50 · dinner in the old town 20:45 · **fado at
  À Capella 21:30, only if Buçaco was skipped** — they're the same slot, and the fado is
  the recommendation.
- **Thu 8** — 08:15 bags in the car (11:00 checkout is firm) · **Biblioteca Joanina 09:00,
  first slot — book this before anything else on the trip** · university, Sé Velha, Arco
  de Almedina · 11:15 drive to **Tomar** · light lunch · **Convento de Cristo 13:15, allow
  2h15** (the Charola, the Manueline window; last admission ~17:00) · **Grutas de Mira de
  Aire 16:15** (no reservations, up to 30 min queue) · **Hotel Lis Batalha 17:45** ·
  floodlit west front 18:30 · dinner in Batalha, booked through the hotel.
- **Fri 9** — the fullest day: ~2h25 driving, four stops. **Mosteiro da Batalha 09:00**
  across the square · **Alcobaça 11:00** (the Pedro and Inês tombs) · **Nazaré 12:30**
  seafront lunch, funicular to Sítio, Praia do Norte and the lighthouse fort ·
  **Óbidos 16:15**, walls at golden hour · **LIS car return 18:45** · Chiado 19:20 ·
  dinner 20:45.

Two structural facts that drive the above: **Conímbriga is dropped — Tomar replaces it**,
and **the Batalha monastery interior cannot be done Thursday** (you arrive 17:45, past the
~17:30 last admission), so it opens Friday. Tomar → caves → Batalha is the tightest chain
in the trip; if the convent overruns, **drop the caves, not the convent**. On Friday,
**Óbidos is the cut** if the day slips — 55 min from Lisbon, and Sat 10 is deliberately
empty. **Alcobaça is not the cut**: it sits between Batalha and Nazaré, so the detour costs
about five minutes.

**Sintra is locked to Mon 12** — all its palaces open daily, whereas DGPC/state museums
close Mondays. It runs rail+bus one way: Rossio→Sintra train, bus 434 to Pena, walk/435 to
Regaleira, Scotturb **1624** over Cabo da Roca to Cascais, train home. Monserrate is cut to
make the bus connection (it has scaffolding anyway).

Other closure facts baked in: **Mon 5 Oct is Implantação da República**, a national
holiday. CAM Gulbenkian and MAAT close Tuesdays. Feira da Ladra runs Tuesdays and Saturdays.

## Car rental — BOOKED (15 Aug 2026)

- **Pick up:** Porto **Boavista**, Avenida da Boavista 1203, 4100-130 — **Tue 6 Oct, 09:30**
- **Return:** **Lisbon Airport**, Alameda das Comunidades Portuguesas, 1700-111 (the return
  area beside Terminal 1) — **Fri 9 Oct, 20:30**
- 3 days 11 hours → **billed as 4 rental days**. One car for the whole trip; Lisbon is
  car-free from Friday evening.

Two knock-ons already applied to `index.html`:

1. **Tue 6 shifts an hour later.** The day was built on an 08:30 city-centre collection.
   Boavista is ~3 km west of the centre and **not walkable with bags** — metro to Casa da
   Música then ~12 min on foot, or a 10-min Uber (~€7). New shape: 08:30 check out, 09:00
   travel out, 09:30 collect, 11:00 Paiva (**book the 11:00 slot, not 10:00**), 14:00
   Ponte 516, 14:45 lunch, 15:50 drive, 17:45 Pinhão, 20:00 Rabelo. The cost is the pool
   afternoon, now about an hour. **The lever if they want it back is skipping Ponte 516.**
2. **Fri 9 gains 1h45 of slack.** The day was written against an 18:45 hand-back with no
   margin; the booking runs to 20:30, so **Óbidos is no longer the automatic cut**. Advice
   given: still return around 18:45 and spend the slack on the day rather than on Óbidos,
   because the day ends at a lockbox in an unfamiliar building. Leaving Óbidos at 19:15
   still works and pushes dinner to ~21:30.

Still to confirm on the booking: **automatic transmission**, the **Via Verde transponder**
(Portugal's motorways are cash-free; the route uses the A32, A24 and A1), **full-to-full
fuel**, and whether the LIS return is in the Terminal 1 car park or an off-site shuttle lot.
The one-way fee should already be inside a Porto→Lisbon booking — check the total.

## Open items

- **Decide the night of 7 Oct** (see live item) — deferred to ~20 Sept / start of October.
- **Read the exact free-cancellation date off all three 7 Oct bookings** — now, not in October.
- **Book the Biblioteca Joanina 09:00 first slot** for Thu 8 — everything else on Thursday
  hangs off it.
- Verify the **Mosteiro da Batalha's October opening hours** (Friday starts there at 09:00)
  and the **Grutas de Mira de Aire October closing time**.
- Ask Hotel Lis to book Thursday dinner — small town, quiet midweek in October; Leiria is
  15 min north as fallback.
- Message the Coimbra host about arriving after dark (19:15, or 19:50 with the Buçaco stop).
- Message the **HUL host** about floor/lift and street-vs-courtyard bedroom — before 4 Oct,
  while cancellation is free. Save the lockbox code offline.
- Book a **bag locker near Cais do Sodré** for Tue 13 — lockbox check-in means no host to
  hold bags.
- Email **NOLIA** about the 09:00 landing: early check-in vs adding the night of 3 Oct.
- Verify the **Scotturb 1624 October timetable** — it decides Monday's Cabo da Roca leg.
- Verify the **Tile Museum** renovation closure (it was the rainy-day plan).
- Choose the Fri 9 late Lisbon dinner.

## Budget

Roughly **€3,700–4,300** all in. About **€700–1,000 of accommodation budget went unspent**
and is now **banked for good** — Bussaco was the last night that could have absorbed a
splurge. The remaining levers are meals or a room upgrade at NOLIA or the Vintage House.
The site displays prices in ILS (₪) at roughly ₪4 to the euro.

## Notes for agents picking this up

- Two researched source documents live outside this repo in `~/Downloads`:
  `portugal-trip-final-draft.md` and `portugal-trip-final-whatsapp.txt`. They contain real
  2026 ticket URLs and closure notices — **trust them over recalled facts**.
- Peneda-Gerês and the PR24 Sistelo hike were dropped; Passadiços do Paiva and Ponte 516
  on Tue 6 replaced them. The remaining hiking is Paiva and the Casal de Loivos climb.
- Live web lookup is unavailable in the authoring environment (WebSearch blocked by org
  policy; WebFetch/curl denied; Playwright MCP navigation blocked by a pre-tool callback).
  Anything needing verification is flagged rather than checked.
- Diagrams in this repo are ASCII, never mermaid.
