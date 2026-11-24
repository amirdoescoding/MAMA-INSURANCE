# Competitive analysis and evidence bank (input for the tool brainstorm)

2026-11-24. Built with the competitive-analyst, research-analyst and data-researcher agents, using the
competitive-analysis-process, competitive-research-snapshot, market-landscape-scan, organic-growth-advisor and
problem-statement skills. **No tool is chosen here.** This feeds the ≥8-idea scoring table.

Legend: **[D1/D2/D3]** synthetic case data. **[web]** real public source (URL in section 6). **(unverified)**
came from a search summary or a single secondary source: check before using it in the memo.

## 0. Reframe

The brief is about **acquiring people who never searched for home insurance**, not about retaining existing
clients. Free perks for policyholders (wearables, sensors, apps) are the retention route competitors already
took, and they don't reach our target.

## 1. What competitors give away

| Player | Free offer | Acquisition or retention | Bridge to paid | Evidence | Fit for Mama (€120k) |
|---|---|---|---|---|---|
| Lemonade | Giveback (unused premium to charity), $12M+ cumulative | Brand | Policy needed | No conversion data | Brand idea only |
| Hippo (US) | Hippo Home app: maintenance checklist + reminders; smart kit | Both | 10 to 13% discount with kit | Self-reported claim reduction | Checklist yes, hardware no |
| Kin (US) | Content, checklists | Acquisition (SEO) | Quote | None | Undifferentiated |
| Getsafe (DE) | App, chat, €15 to €30 referral credit | Retention, referral | Policy needed | 500k+ customers (self-reported) | Referral later |
| Luko (FR) | Water leak sensor (free status unclear) | Retention | Policy needed | Receivership, book sold to Allianz Direct for €4.3M (Jan 2024) | Cautionary tale |
| Hiscox UK | LeakBot (£149) + yearly engineer visit | Retention | Policy needed | None published | No |
| Ditto (IN) | Free 30-min advice, no obligation | Acquisition through trust | Adviser is also the agent | 30k+ Google reviews (self-reported) | Advice-first, via Mia |
| Generali Jeniot | Gas, smoke and water sensors as a policy option | Retention | Bundled | 2M connected target (2018), no outcome | No |
| UnipolSai | Unibox C@sa device with the policy | Retention | Bundled | None | No |
| Intesa XME Protezione | 15% off year 1, account holders only | Bank cross-sell | Current account | None | Bank = partner target |
| Allianz Direct, Prima, Poste, Genertel, Verti, Zurich Connect | **No free consumer tool found** (light search) | n/a | Quote form | n/a | **White space** |
| UniSalute (health) | App with open section for non-clients (vision, hearing, sleep tests) | Both | Login for clients | 4.1★ (2,666 ratings); source from 2013 | **Pattern to copy** |
| Facile.it / Segugio | Free comparison, insurer pays | Acquisition | They are Mama's paid channel (~50% of policies) | ~5M monthly users, €248M revenue 2025 | Rival for the same user |
| Immobiliare.it / Idealista | Free valuation (OMI), mortgage tools | Lead gen | Mortgage brokers | None | Traffic partner |
| ProntoPro | Free quotes from tradespeople | Marketplace | Pro fees | 50M+ requests, 6.7M IT customers | Referral partner |

### Recurring patterns
1. Free hardware or services only come with a policy: retention, useless for never-buyers.
2. Hardware economics fail at ~€91/yr margin per policy (Luko, Hiscox: no results).
3. Free content and checklists: cheap, undifferentiated unless personalised.
4. Advice first (Ditto): builds trust, but a human team costs too much. Automate it.
5. A free open section for non-clients (UniSalute): the closest match to the brief.
6. Utility → recurring use → offer (Credit Karma, 106M members): the model behind free tools that convert.
7. Free-content funnels that rely on organic search are fragile (NerdWallet monthly users −20% YoY, 2024): own the return channel.

### Three plays we can borrow
- **UniSalute:** a no-login core for non-clients; the insurance part is separate.
- **Hippo Home without hardware:** a personal checklist + reminders (reminders need explicit consent).
- **Ditto through Mia:** an honest "what you have, what's missing" result first, quote offered afterwards, Mama's interest disclosed.

## 2. Evidence from D1 to D3 (synthetic)

Source: `docs/Mama Tools - Data analysis report.pdf` p3 to p12 and `graphify-out/converted/`.

- **People think they're covered when they aren't.** 43% say insured, only 14% have real multirisk;
  58 have mortgage fire-only, 51 don't know what they have. [D1, report p3]
- **#1 barrier is "someone else covers me": 33%** (landlord, bank, building, parents); 53% of uninsured tenants.
  Then price 19%, no risk 15%, never thought 14%, complicated 12%, distrust 8%. [D1, report p4]
- **The moment beats the profile.** Open (4 to 5/5) among uninsured: no event 5%, moved 18%, new lease 29%,
  renovation 41%, bought 45%, new baby 60% (n=5). Core target with an event: 36% vs 6%. [D1, report p5]
- **Top pain: repairs, leaks, damp, mould** = 21% of answers, 7.0 h/month, strongest insurance link.
  Moving 11% (7.6 h, 21% open). Taxes and cleaning: big but weak fit. [D1, report p6]
- **Search.** Home problems 9.23M searches/yr at €0.81 vs insurance 0.72M at €4.29 (13x volume, 1/5 CPC).
  "come togliere la muffa" 265k/yr at €0.41, peak Jan (3x Aug); "caldaia in blocco" peak Dec;
  "trasloco" peak Jun and Sep. "Mama insurance": 210/month. [D2]
- **Funnel (model B, free core + extras for policyholders):** activation 36%, consent 18%, quote 6%,
  quote→policy 11%. 90k activated × 6% × 11% ≈ **594 policies** from ~250k users. [D3]
- **Cost check.** €120k / 600 = €200 per policy at M6. Under €110 over 12 months means ~1,100 to 1,450
  policies, so **~670 more in M7 to M12 from near-free channels**. Best channels (policies per 1,000 users):
  partners 4.48, word of mouth 3.56, SEO 3.01; paid social 1.82. [D3]

| Moment | Key data | Insurance bridge | Season |
|---|---|---|---|
| Water, leaks, mould | 21% of tasks; mould 265k searches/yr at €0.41 | Water damage, RC | Nov to Jan |
| Moving, utilities | 11%; trasloco 328k/yr | Contents, RC | Jun to Sep |
| New tenant | 53% think the landlord covers them; 29% open | Tenant policy from €4.99/month | Jun to Sep |
| New owner, renovation | 45% / 41% open (small n) | Multirisk, water | Flat |
| Mortgage fire-only gap | 58 fire-only respondents | Contents, RC, theft | Flat |
| Boiler, deadlines | 10%; boiler searches peak in winter | Breakdown, assistance | Nov to Feb |
| Theft | porta blindata 18k/mo, allarme casa 15k/mo | Theft | Flat |

## 3. Public evidence (real)

- **Tenure.** 70.8% of households own, 20.5% rent (ISTAT, 2021 census). [web]
- **Coverage gap.** Fire cover 49% of homes in 2025 (ANIA via Facile.it); **MEMORY.md says ~52%, same
  source: reconcile.** ~7% have nat-cat cover; 78% of homes in medium or high quake/flood hazard (ANIA). [web]
- **Hazard.** 94.5% of comuni at landslide, flood or erosion risk; 6.8M people in medium flood hazard
  (ISPRA, July 2025). [web]
- **Nat-cat law.** Mandatory for businesses (staggered to 1 Jan 2026), **not for households**. ANIA (July 2026)
  asked to extend it to homes; Federproprietà open to a gradual obligation. Tailwind, never a deadline.
  IVASS cat-policy comparator expected end 2026 (partner or rival). [web]
- **730.** 19% deduction on nat-cat premiums for homes (code 43), traceable payment, cap above €75k income. [web]
- **Mortgage.** Only fire and explosion is legally required; no contents; any insurer allowed. [web]
- **Burglary.** 155,590 home burglaries in 2024 (+5.4%; Censis-Verisure, commercial source). [web]
- **Trust.** IVASS trust score 59.5/100, literacy 54/100 (2021). Garante fined Verisure €400k and
  Energia Pulita €300k for bundled consent: keep consent separate and log it (wording, time, place). [web]
- **Free tools at scale.** HubSpot Website Grader: 4M sites graded, no conversion published. Credit Karma
  106M members. Quiz vendors claim 35 to 55% of completers leave contact details (vendor data, warm audience).
  No public free-tool → policy rate exists for insurance: use D3. [web]

### Open data a tool could use (no scraping)
- ISPRA IdroGEO: open, has APIs. Licence differs by layer (CC BY 4.0 or CC BY-SA 4.0): check share-alike.
- INGV MPS04 seismic hazard: WFS, DOI citation; licence field empty in the record seen.
- OMI property values (Agenzia delle Entrate): free download, commercial reuse unclear: ask in writing.
- ANIA reports: cite, don't reproduce.

## 4. White spaces and idea seeds (not scored)

Gaps nobody in Italy covers well: "do I even need it?", a personal "what am I really covered for?" check,
plain language for older owners, neutral advice.

| # | Seed | Why (evidence) | Bridge | Biggest risk |
|---|---|---|---|---|
| 1 | "Am I really covered?" check (landlord, bank, condo policy) | #1 barrier 33%; 14% real multirisk | Honest gap → quote | Needs input from the user's documents |
| 2 | Water, mould and leak fixer (diagnose, what to do, who pays) | Top pain 21%; €0.41 CPC; winter = month 1 | Water damage cover | Searchers may be tenants who don't own the problem |
| 3 | Home risk by address (ISPRA + INGV) | 7% cat cover vs 78% exposed; nat-cat debate = PR | Nat-cat cover, 730 deduction | Data licences; don't imply a deadline |
| 4 | Move-in kit for tenants and buyers (deposit, utilities, checks; no lease generator) | Life event 36% vs 6% open | Tenant / multirisk policy | Seasonal (Jun to Sep) |
| 5 | Home passport: boiler, deadlines, expiries with reminders | Hippo pattern; regional boiler fines €100 to €3,000 | Renewal moments | Indirect fit, needs return visits |
| 6 | 730 deduction checker | Annual fiscal moment; code 43 | Nat-cat cover | Small audience, fiscal disclaimer |
| 7 | Second or inherited home checklist | ~1 home in 3 unoccupied (unverified) | Theft, water | Weakest evidence |

## 5. To verify before the memo
- Italian direct insurers really have no free tool (light search only).
- Fire cover 49% vs 52% (MEMORY.md).
- Nat-cat business uptake 683k policies / 16% (search summary).
- ISPRA layer licences, OMI commercial reuse.
- Water-damage share of home claims: not found in public data (ask Mama or IVASS bulletin).

## 6. Sources

Competitors
- Lemonade Giveback 2025: https://www.lemonade.com/investor/news/2025-giveback
- Lemonade Q2 2021 letter: https://www.marketscreener.com/quote/stock/LEMONADE-INC-109161819/news/Lemonade-Q2-2021-Earnings-Conference-Call-Letter-to-Shareholders-36541973
- Lemonade FY2025: https://www.insurancejournal.com/news/national/2026/02/19/858721.htm
- Hippo Home: https://home.hippo.com/hippo-home , https://www.myhippo.com/smart-home , https://hippo.com/blog/sheltr
- Kin: https://insurify.com/homeowners-insurance/companies/kin/
- Getsafe: https://apps.apple.com/gb/app/getsafe/id1296674334
- Luko / Allianz Direct: https://www.optionfinance.fr/info-financiere-en-continu/d/2024-01-24-allianz-direct-acquiert-les-activites-dassurance-habitation-de-luko.html , https://www.moneyvox.fr/assurance/actualites/98920/allianz-finalise-le-transfert-des-clients-de-luko
- Hiscox LeakBot: https://www.hiscox.co.uk/node/8976
- Ditto: https://joinditto.in/health-insurance/ad/
- Generali Jeniot: https://www.aziendabanca.it/notizie/generali-jeniot-iot , https://www.aziendabanca.it/notizie/assicurazioni/casa-semplice-alleanza
- Intesa XME Protezione: https://www.intesasanpaolo.com/it/common/landing/promo-polizza-protezione-salute-e-casa.html
- Allianz Direct home terms: https://www.allianzdirect.it/dam/documents/set-informativi/prodotti/casaefamiglia/Set-informativo-casa.pdf
- UniSalute: https://www.quotidianosanita.it/?p=17175 , https://apps.apple.com/it/app/unisalute-up/id638165919
- Facile.it / Segugio: https://www.facile.it/assicurazioni-casa.html , https://assicurazioni.segugio.it/assicurazione-casa.html , https://www.milanofinanza.it/news/facile-it-scommette-sul-risparmio-202507110658104654
- Immobiliare.it: https://www.immobiliare.it/en/valutazione-immobiliare/
- ProntoPro: https://avvenire.it/economia/oltre-50-milioni-le-richieste-alla-piattaforma-prontopro_114367
- Yolo: https://www.aziendabanca.it/notizie/fintech-insurtech/yolo-casa-yolo-auto-genertel

Free-tool evidence
- HubSpot Website Grader: https://www.hubspot.com/blog/bid/4834/Website-Grader-Evaluates-Over-1-Million-URLs
- Credit Karma (Intuit SEC filing 2020): https://www.sec.gov/Archives/edgar/data/896878/000119312520048757/d872929d425.htm
- NerdWallet Q4 2024: https://investors.nerdwallet.com/news-releases/news-release-details/nerdwallet-reports-fourth-quarter-and-full-year-2024-results
- Quiz benchmarks (vendor): https://tryinteract.com/blog/quiz-conversion-rate-report/

Italy
- ISTAT tenure: https://www.istat.it/comunicato-stampa/abitazioni-occupate/
- ANIA coverage: https://www.facile.it/assicurazioni/news/polizze-casa-sanita-2025-dati-ania.html , https://www.quotidiano.net/economia/catastrofi-assicurato-solo-il-7-3b28a9b3
- ISPRA hazard 2025: https://www.isprambiente.gov.it/it/archivio/notizie-e-novita-normative/notizie-ispra/2025/07/dissesto-idrogeologico
- Nat-cat businesses: https://ance.it/2025/03/polizze-catastrofali-proroga-differenziata-per-lobbligo-assicurativo-delle-imprese/
- Nat-cat households (ANIA, July 2026): https://www.avvenire.it/economia/lavoro/liverani-ania-estendere-obbligo-polizza-catastrofi-a-case_110472
- Federproprietà: https://tg24.sky.it/cronaca/2026/07/23/polizze-catastrofali-federproprieta-apre-obbligo-graduale
- IVASS comparator: https://www.milanofinanza.it/news/per-le-polizze-catastrofali-arriva-la-bussola-dell-ivass-2699531
- 730 deduction: https://www.altroconsumo.it/soldi/730/consigli/assicurazioni
- Mortgage fire policy: https://www.intesasanpaolo.com/content/internetbanking/it/faq/common/faqHome/polizza-incendio-mutui.privati.html
- Burglary: https://www.censis.it/wp-content/uploads/2025/11/Rapporto-Verisure-Censis.-Sintesi-dei-principali-risultati.pdf
- IVASS trust survey: https://www.dirittobancario.it/wp-content/uploads/sites/default/files/allegati/indagine_ivass_sulle_conoscenze_e_comportamenti_assicurativi_degli_italiani.pdf
- Garante consent fines: https://ntplusdiritto.ilsole24ore.com/art/lead-generation-e-telemarketing-nuova-frontiera-compliance-provvedimento-garante-AIPUJzEB
- ISPRA IdroGEO data: https://www.isprambiente.gov.it/it/news/la-piattaforma-idrogeo-di-ispra-e-nel-catalogo-pubblico-del-dipartimento-per-la-trasformazione-digitale-della-presidenza-del-consiglio-dei-ministri
- INGV data: https://data.ingv.it/metadata/web_service_eng
- OMI reuse note: https://github.com/ondata/quotazioni-immobiliari-agenzia-entrate
