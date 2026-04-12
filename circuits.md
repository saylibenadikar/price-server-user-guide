# Circuits and Substations

The price server publishes prices per distribution circuit (PG&E) or substation (SCE). This page lists all available circuits and what physical infrastructure they represent.

## PG&E circuits

Each PG&E program is named `<RATE>-<9-digit-circuit-id>` (e.g. `EELEC-013532223`). The 9-digit circuit ID encodes a specific distribution **feeder** — a power line segment that carries electricity from a substation to customers in a local area.

The circuit ID hierarchy:

- **Region** — PG&E's five distribution planning regions (Bay Area, Central Valley, etc.)
- **Division** — operational division within a region (East Bay, Fresno, etc.)
- **Substation** — the distribution substation the feeder originates from
- **Feeder** — the specific feeder number (last 4 digits of the circuit ID)

For example, circuit `013532223`:
- Region: Bay Area
- Division: Diablo
- Substation: LAKEWOOD
- Feeder: 2223

Sources: [PG&E 2022 Grid Needs Assessment](https://docs.cpuc.ca.gov/PublishedDocs/Efile/G000/M496/K629/496629893.PDF) (CPUC filing, Appendix D) and the [Priicer community cross-reference](https://forum.priicer.com/t/pg-e-dynamic-pilot-california/33).

### Available PG&E circuits (59)

These are the 59 circuits currently available in the GridX Pricing API. Each circuit has a program for every PG&E rate schedule (EELEC, BEV1, BEV2P, BEV2S, B6, B19P) — 354 PG&E programs total.

#### Bay Area

| Circuit ID | Division | Substation | Feeder |
|------------|----------|------------|--------|
| `012041131` | East Bay | OAKLAND D | 1131 |
| `012640401` | East Bay | BECK STREET | 0401 |
| `013532223` | Diablo | LAKEWOOD | 2223 |
| `013921103` | East Bay | FRANKLIN | 1103 |
| `014052103` | Mission | NORTH DUBLIN | 2103 |
| `014321101` | Diablo | SAN RAMON (BALFOUR) | 1101 |
| `014592108` | Diablo | BRENTWOOD | 2108 |
| `022011162` | Peninsula | MISSION X BANK 10 | 1162 |
| `024011104` | Peninsula | BAY MEADOWS | 1104 |
| `024040403` | Peninsula | BERESFORD | 0403 |
| `024091102` | Peninsula | GLENWOOD | 1102 |
| `024101103` | Peninsula | HALF MOON BAY | 1103 |
| `024131103` | Peninsula | MENLO | 1103 |

#### North Coast

| Circuit ID | Division | Substation | Feeder |
|------------|----------|------------|--------|
| `042211101` | North Bay | NOVATO | 1101 |
| `042571101` | Sonoma | MOLINO | 1101 |
| `042891102` | Sonoma | GEYSERVILLE | 1102 |

#### North Valley and Sierra

| Circuit ID | Division | Substation | Feeder |
|------------|----------|------------|--------|
| `042450414` | North Bay | VALLEJO B | 0414 |
| `102841106` | North Valley | ANITA | 1106 |
| `103081106` | North Valley | BUTTE | 1106 |
| `103351101` | North Valley | DESCHUTES | 1101 |
| `152442109` | Sierra | PLEASANT GROVE | 2109 |
| `152561107` | Sierra | PENRYN | 1107 |
| `152701109` | Sierra | BELL | 1109 |

#### South Bay and Central Coast

| Circuit ID | Division | Substation | Feeder |
|------------|----------|------------|--------|
| `082031112` | De Anza | MOUNTAIN VIEW | 1112 |
| `082831109` | San Jose | MILPITAS | 1109 |
| `082952113` | San Jose | EDENVALE | 2113 |
| `083182102` | San Jose | LLAGAS | 2102 |
| `083371113` | De Anza | SARATOGA | 1113 |
| `083611114` | De Anza | BRITTON | 1114 |
| `083771102` | De Anza | VASONA | 1102 |
| `083892102` | San Jose | MONTAGUE | 2102 |
| `182191101` | Central Coast | SAN ARDO | 1101 |
| `182381104` | Central Coast | DOLAN ROAD | 1104 |
| `182492104` | Central Coast | HOLLISTER | 2104 |
| `183052109` | Los Padres | TEMPLETON | 2109 |

#### Central Valley

| Circuit ID | Division | Substation | Feeder |
|------------|----------|------------|--------|
| `162611702` | Stockton | MANTECA | 1702 |
| `162611703` | Stockton | MANTECA | 1703 |
| `162611704` | Stockton | MANTECA | 1704 |
| `162991101` | Stockton | CORRAL | 1101 |
| `163121106` | Stockton | COUNTRY CLUB | 1106 |
| `163191711` | Yosemite | RIVERBANK | 1711 |
| `163191714` | Yosemite | RIVERBANK | 1714 |
| `163251101` | Yosemite | CROWS LANDING | 1101 |
| `163722110` | Stockton | MOSHER | 2110 |
| `163912104` | Stockton | EIGHT MILE | 2104 |
| `252051104` | Fresno | ASHLAN AVENUE | 1104 |
| `252051114` | Fresno | ASHLAN AVENUE | 1114 |
| `252062112` | Fresno | SHEPHERD | 2112 |
| `252281111` | Fresno | CALIFORNIA AVE | 1111 |
| `252711104` | Fresno | KERMAN | 1104 |
| `252802101` | Yosemite | MERCED | 2101 |
| `253611106` | Yosemite | ATWATER | 1106 |
| `253882109` | Yosemite | EL CAPITAN | 2109 |
| `253911102` | Kern | LAMONT | 1102 |
| `254081104` | Fresno | CLOVIS | 1104 |
| `254091104` | Fresno | DINUBA | 1104 |
| `254411105` | Fresno | MC MULLIN SUB | 1105 |
| `254452101` | Yosemite | MARIPOSA | 2101 |
| `254572101` | Kern | RENFRO | 2101 |

## SCE substations

Each SCE program is named `<RATE>-<substation>` (e.g. `TOU-PRIME-Eagle Rock`). The substation name identifies an SCE distribution substation. Each substation has a program for every SCE rate schedule (TOU-PRIME, TOU-D-49, TOU-D-58) — 138 SCE programs total.

### Available SCE substations (46)

| Substation | | Substation | | Substation |
|---|---|---|---|---|
| Alamitos | | Gould | | San Bernardino |
| Antelope | | Hinson | | Santa Clara |
| Bailey | | Johanna | | Santiago |
| Barre | | Kramer | | Saugus |
| Center | | La Cienega | | Springville |
| Chino | | La Fresa | | System |
| Del Amo | | Laguna Bell | | Valley AB |
| Devers | | Lighthipe | | Valley EFG |
| Eagle Rock | | Mesa | | Vestal |
| El Casco | | Mira Loma | | Victor |
| El Nido | | Mirage | | Viejo |
| Ellis | | Moorpark | | Villa Park |
| Etiwanda | | Olinda | | Vista 115 |
| Goleta | | Padua | | Vista 66 |
| | | Rector | | Walnut |
| | | Rio Hondo | | Windhub |

> **Note:** "System" represents the SCE system-wide average. The remaining 45 substations represent specific distribution substations within the SCE service territory in Southern California.
