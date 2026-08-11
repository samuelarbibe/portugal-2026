# Portugal — 4–13 October 2026

Planning context for a 9-night trip, 2 adults. This README is written to be dropped into
an AI agent as context; `portugal-trip-2026.html` is the live deliverable.

- **Land** OPO, Sun 4 Oct, 09:00
- **Depart** LIS, Tue 13 Oct, 22:15
- **9 nights, five bases** — Porto 2 · Pinhão 1 · Buçaco 1 · Batalha 1 · Lisbon 4

## The file

`portugal-trip-2026.html` is a **self-contained single-file site** — embedded CSS and JS,
no build step, opens straight from `file://`, prints cleanly via `@media print`. GitHub
will not render it in the browser; download it and open it locally.

The booking checklist persists ticks in `localStorage` under keys `pt26.<data-k>`. Storage
is scoped to the file's path, so **keep the same filename and location** when regenerating,
or saved ticks are lost. The working copy lives at `~/Downloads/portugal-trip-2026.html`;
this repo holds a snapshot.

The overview strip is a 20-column CSS grid: 10 day cells spanning 2 columns each, plus
9 night chips offset one column (`grid-column:2i / span 2`) so each night visually
straddles the two days it joins.

## Standing constraints — do not re-litigate

- **No wine-focused activities.** The Douro is for scenery, not tastings. Ask for
  non-alcoholic pairings at restaurants.
- **Minimal private drivers — inside cities only.** Self-drive between cities.
- **One rental car only:** picked up in Porto 6 Oct, dropped at LIS airport on arrival
  Fri 9. **Lisbon is entirely car-free.**
- Mid-range boutique hotels / Airbnbs. Avoid Six Senses — too wine-led.
- Cities + nature + food in roughly equal measure; moderate hiking wanted.
- Check into the hotel on arrival day before going out.
- **The traveller books everything themselves** and reports back. Recommend and compare;
  do not book.

## Bookings — all nine nights held

| Nights | Where | Property |
|---|---|---|
| 1–2 · 4–6 Oct | Porto | **NOLIA Boutique Hotel** |
| 3 · 6 Oct | Pinhão, Douro | **The Vintage House** — dinner at the Rabelo, Tue 6 20:00, booked |
| 4 · 7 Oct | Luso / Buçaco | **Palace Hotel do Bussaco** ⚠ see below |
| 5 · 8 Oct | Batalha | **Hotel Lis Batalha**, Double Room Mansarda, Largo do Mestre Afonso Domingues (the monastery square). +351 244 765 260 |
| 6–9 · 9–13 Oct | Lisbon | **"HUL · Chiado"** Airbnb, room `4902781`, Rua Nova da Trindade block. Lockbox self check-in |

Tue 13 is a Lisbon day with no night — Uber to LIS 18:45.

## ⚠ Live item — the night of 7 Oct is booked three times

Deliberate hedge; two must be cancelled.

1. **Palace Hotel do Bussaco**, Luso — *the recommended keeper*
2. **Airbnb "Studio King Deluxe"**, Coimbra, host Nuno Miguel, R. Lourenço de Almeida
   Azevedo 5 — the runner-up
3. **Vila Julieta Guesthouse**, Booking.com, 20 Alameda Conchada, Coimbra

**Cancel order: Vila Julieta first** — Booking.com auto-charges, and it loses to both
others. **Then the Airbnb**, if Bussaco stays.

**Why Bussaco wins.** It restores the two things the Batalha booking cost: the Buçaco
forest walk becomes a dawn walk out of the hotel door (Via Sacra → Cruz Alta → Fonte
Fria, ~2h, ~200 m, shaded) rather than an hour of backtracking from Coimbra; and leitão
à Bairrada at Mealhada is 10 minutes away. It is also the last place the unspent
accommodation budget can land. *Ask for a renovated room — the fabric is uneven.*

**What it costs.** The Coimbra evening and fado at À Capella. Thursday gets full enough
that the Mosteiro da Batalha slides to **Friday 09:00**, which cuts **Mira de Aire**.
Thursday's card in the HTML carries the full alternate Coimbra-Airbnb timings, so the
itinerary can be flipped back in one pass.

## Route

```
  Sun 4   Mon 5   Tue 6   Wed 7   Thu 8   Fri 9   Sat 10  Sun 11  Mon 12  Tue 13
 ┌───────────────┬───────┬───────┬───────┬───────────────────────────────────────┐
 │     PORTO     │ ▸Douro│ ▸Buçaco│▸Batalha│              LISBON                 │
 └───────┬───────┴───┬───┴───┬───┴───┬───┴───────────────────────────────────────┘
    N1 N2 ·  NOLIA    N3 ·    N4 ·    N5 ·      N6  N7  N8  N9 · HUL Chiado
             Porto   Pinhão  Buçaco  Batalha         (car-free)
                       │       │       │
                    Vintage  Bussaco  Lis      car returned at LIS on Fri 9
                     House
```

Key legs: Porto→Pinhão via Passadiços do Paiva · N222 both directions ·
Folgosa→Galafura→Luso ~1h50 · Buçaco→Coimbra 0h30 · Coimbra→Conímbriga→Batalha 1h05 ·
Batalha→Alcobaça→Nazaré 0h50 · Nazaré→LIS ~1h30.

## Day shape through the middle

- **Wed 7** — Casal de Loivos climb 07:45 · rabelo cruise 11:00 · station azulejos ·
  N222 west · **DOC at Folgosa as lunch, 13:15** (en route south; lunch service is the
  reliable one in shoulder season) · Galafura viewpoint 15:20 · Luso 18:20 · Fonte Fria
  walk 19:00 · dinner in the hotel dining room 20:00, or Mealhada leitão if lunch was light.
- **Thu 8** — Buçaco forest walk from the door 07:45 · check out 11:00 · Coimbra 11:45,
  **Biblioteca Joanina ~12:00** · old town, Sé Velha · **Conímbriga 15:15** (today's flex) ·
  Hotel Lis Batalha 17:30 · floodlit west front 18:30 · dinner in Batalha.
- **Fri 9** — **Mosteiro da Batalha 09:00** across the square (Capelas Imperfeitas) ·
  **Alcobaça 11:20** — the Pedro and Inês tombs face each other across the transept, and
  she was murdered in Coimbra · **Nazaré 13:05**: seafront lunch, funicular to Sítio,
  Praia do Norte and the lighthouse fort · LIS car drop 18:15 · Chiado 18:50.

**Sintra is locked to Mon 12** — all its palaces open daily, whereas DGPC/state museums
close Mondays. It runs rail+bus one way: Rossio→Sintra train, bus 434 to Pena,
walk/435 to Regaleira, Scotturb **1624** over Cabo da Roca to Cascais, train home.
Monserrate is cut to make the bus connection (it has scaffolding anyway).

Other closure facts baked into the plan: **Mon 5 Oct is Implantação da República**, a
national holiday. CAM Gulbenkian and MAAT close Tuesdays. Feira da Ladra runs Tuesdays
and Saturdays.

## Open items

- Decide the three-way 7 Oct cancellation (above).
- Verify the **Mosteiro da Batalha's October opening hours** — Friday now starts there at 09:00.
- Book the **Biblioteca Joanina** timed slot, ~12:00 Thu 8.
- Ask Hotel Lis to book **Thursday dinner** — small town, quiet midweek in October;
  Leiria 15 min north is the fallback.
- Message the **HUL host** about floor/lift and whether the bedroom faces the street —
  before 4 Oct, while cancellation is free. Save the lockbox code offline.
- Book a **bag locker near Cais do Sodré** for Tue 13 — lockbox check-in means no host
  to hold bags.
- Email **NOLIA** about the 09:00 landing: early check-in vs adding the night of 3 Oct.
- Verify the **Scotturb 1624 October timetable** — it decides Monday's Cabo da Roca leg.
- Verify the **Tile Museum** renovation closure (it was the rainy-day plan).
- Choose the Fri 9 late Lisbon dinner.

## Budget

Roughly **€3,700–4,300** all in, with about **€700–1,000 of accommodation budget
unspent** — Bussaco is the last place it can land. The site displays prices in ILS (₪) at
roughly ₪4 to the euro.

## Notes for agents picking this up

- Two researched source documents live outside this repo in `~/Downloads`:
  `portugal-trip-final-draft.md` and `portugal-trip-final-whatsapp.txt`. They contain real
  2026 ticket URLs and closure notices — **trust them over recalled facts**.
- Peneda-Gerês and the PR24 Sistelo hike were dropped; Passadiços do Paiva and Ponte 516
  on Tue 6 replaced them.
- Diagrams in this repo are ASCII, never mermaid.
