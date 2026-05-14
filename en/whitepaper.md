---
title: "Finland's Path to a Sovereign Bitcoin Reserve"
subtitle: "Operating Model, Custody, Political Sequencing"
author: "Jukka Blomberg · NorthPoint, Helsinki"
date: "13 May 2026"
version: "0.2"
license: "CC-BY 4.0"
abstract: |
  The international sovereign Bitcoin landscape converged between October 2024 and
  May 2026. The United States established a Strategic Bitcoin Reserve by Executive
  Order. Sweden's opposition filed a parliamentary motion for a national reserve,
  naming Finland and Norway as the comparator states it risks falling behind. The
  Czech National Bank Governor publicly considered an allocation. El Salvador and
  Bhutan operate active sovereign positions. The European Central Bank is silent —
  the composition of member-state reserves is a national competence, not an ECB
  question. Finland has not yet defined its position. This whitepaper proposes one:
  a three-track operating model, a three-tier custody architecture, a cross-party
  political sequencing plan, and replies to the five most common counter-arguments.
---

# Executive Summary

The case for a Finnish sovereign Bitcoin reserve framework rests on four converging facts.

**First, the international policy direction has settled.** The United States, Sweden, Czechia, El Salvador, and Bhutan have all moved. Switzerland's grassroots referendum failed — a useful confirmation that this is a top-down policy question, not a bottom-up citizen initiative.

**Second, Sweden's parliamentary filing of October 2024 explicitly names Finland (and Norway) as the comparator states it fears falling behind.**[^sweden] The position of Nordic leadership on this question is, at this moment, on offer rather than contested. Sweden has done Finland the unusual favour of nominating Finland's leadership in writing — and refusing to act is the only way to validate Sweden's anxiety.

**Third, Finland's structural advantages are rare in combination and unmatched among small European economies.** Cheap nuclear electricity (Olkiluoto 3 online since 2023), cold climate (free cooling for high-density compute infrastructure eight months a year), engineering pedigree (Linux, MySQL, Nokia, IQM, Wolt, Supercell — and Martti Malmi, who worked directly with Satoshi Nakamoto on early Bitcoin), governance trust (#1 globally on the Transparency International index for most of the past decade), and a mature MiCA implementation through the Finnish Financial Supervisory Authority.

**Fourth, the European Central Bank is silent — and the silence is structural, not accidental.** The composition of member-state foreign exchange reserves is a national competence under the Treaty on the Functioning of the European Union. The ECB approves monetary policy; it does not approve member states' reserve composition. Germany holds gold. Italy holds gold. Finland already holds gold. This is the legal frame in which a Finnish Bitcoin reserve sits.

Within this frame, this whitepaper proposes three sequential tracks.

**Track A — Establish a published governance framework for state-held digital assets.** Finland already custodies digital assets that arrive through law-enforcement seizure. The operational reality is fragmented across at least three agencies (Tulli, Verohallinto, the relevant prosecutorial offices); liquidation decisions are made on a recurring basis without published policy; and no report is filed on a defined cadence with Eduskunta. Track A does not propose growing this footprint — it proposes governing it. A single named authority, a published framework, a quarterly transparency report, and a deferral of further liquidation pending parliamentary review. No new monetary policy is required. No purchases are required. No parliamentary authorization beyond an interagency Memorandum of Understanding is needed. Track A is worth doing on its own merits, even if Tracks B and C are never adopted.

**Track B — Establish the legal mechanism for permanent sovereign accumulation.** A one-time amendment to the Confiscation Act (Pakkokeinolaki) allows Bitcoin obtained through law-enforcement seizure, after all due-process and forfeiture procedures are exhausted, to enter a permanent sovereign reserve rather than being liquidated to euros. This is budget-neutral. It mirrors the U.S. Strategic Bitcoin Reserve framework (March 2025) and parallels the Swedish opposition's October 2024 proposal. The point is the *mechanism* and the *legal precedent* it establishes — not the immediate flow rate.

**Track C — Strategic allocation.** An optional 0.5% allocation of Finland's foreign exchange reserves to Bitcoin, phased over five years. Conditional on Tracks A and B succeeding and on a Suomen Pankki working-paper consensus on custody and risk methodology. Debated openly in Eduskunta. Sized so that even an extreme 90% drawdown represents less than 0.05% of total reserves. This is the substantive policy track; Tracks A and B are the governance preconditions that make it possible to debate Track C seriously.

The remainder of this document covers each track in detail; a three-tier custody architecture (cold storage at Suomen Pankki, institutional partner custody for operational liquidity, an independent proof-of-reserves audit layer); a political sequencing plan that frames the proposal for each major Finnish parliamentary party; replies to the five most common counter-arguments (volatility, ECB optics, illicit-use, legitimacy signalling, the Dalio transparency objection); and three concrete first moves Finland can take in 2026 that require no new legislation, at a combined cost under €500,000.

This document is published under CC-BY 4.0 so that policymakers, journalists, and other jurisdictions — Sweden, Norway, Estonia, Denmark, Germany — can freely cite, adapt, and fork it. The author is the founder of NorthPoint and previously served as Chief Marketing Officer at two international cryptocurrency exchanges between 2017 and 2024.

[^sweden]: Dioukarev, D. & Perez, D. (2024). *Motion 2024/25:1232 — Strategic Bitcoin Reserve.* Sveriges Riksdag. Filed 1 October 2024. See also [Sweden's opposition party calls for strategic Bitcoin reserve, BeInCrypto](https://beincrypto.com/swedens-opposition-party-calls-for-strategic-bitcoin-reserve/).

---

# 1. Why now

The international sovereign Bitcoin landscape changed materially between October 2024 and May 2026. The pattern across jurisdictions is converging, and the window in which Finland can act *deliberately* rather than reactively is approximately eighteen months.

**United States (March 2025 — present).** An Executive Order established the Strategic Bitcoin Reserve from forfeited assets. As of May 2026, the White House has publicly signalled a Treasury-led purchase mechanism is "weeks away."[^whitehouse] The U.S. position has moved from "Bitcoin is a speculative asset" to "Bitcoin is a strategic reserve component" within twelve months.

**Sweden (October 2024 — present).** Members of Parliament Dennis Dioukarev and David Perez filed a formal motion asking the Government to study a national Bitcoin reserve, with structure, oversight, and custody options. The motion explicitly states that Sweden "risks falling behind Finland and Norway if it stays too cautious."[^sweden_quote] The motion was reviewed by the Finance Committee in October 2024 and has been a recurring talking point in Swedish economic-policy discussions since.

The naming of Finland in the motion is the key political detail. It is not the case that Sweden is racing past Finland on this question. It is the case that Sweden has nominated Finland — in writing, on a parliamentary record — as the country whose movement Sweden is afraid of. That is a positioning gift, and it has an expiry date. Once Sweden adopts its own framework, the gift is rescinded.

**Czech Republic (January 2025).** Czech National Bank Governor Aleš Michl publicly stated that Bitcoin should be considered as a potential reserve diversification component, becoming the first sitting central-bank governor of an EU member state to do so. The proposal was politically contained, but the institutional precedent — that a serving EU central-bank governor can speak publicly on the topic without consequence — is established.

**El Salvador (June 2021 — present).** Continuous sovereign Bitcoin acquisitions through the General Directorate of Digital Assets. As of early 2026, El Salvador's reported holdings exceed 6,000 BTC.

**Bhutan (2024 — present).** An active sovereign Bitcoin treasury operated through Druk Holding and Investments, reportedly valued at approximately $252M after a 100 BTC transfer in May 2026.[^bhutan] Bhutan's relevance to Finland is the demonstration that a small nation can operate a sovereign Bitcoin position with credibility — and that such a position can be operational, not merely declarative.

**Switzerland (May 2026).** The grassroots referendum to amend Article 99 of the Swiss Constitution to require the Swiss National Bank to hold Bitcoin failed to gather the required 100,000 signatures.[^swiss] This is informative for Finland: bottom-up citizen-initiative paths do not work for sovereign-reserve policy. Top-down parliamentary and central-bank paths do.

**The European Central Bank — silent.** The ECB has not issued public guidance on member-state sovereign Bitcoin reserves. This is not a coincidence. The composition of member-state foreign-exchange reserves is a national competence under the Treaty on the Functioning of the European Union; the ECB's mandate is monetary policy. The silence is the legal frame: member states have the latitude to define their own approaches, and the absence of ECB pushback is itself the operative signal.

**The pattern.** Among major economies, top-down paths (U.S., Sweden, Czechia) are succeeding where bottom-up paths (Switzerland) are not. Finland's path must therefore be top-down: through Eduskunta and Suomen Pankki, with operator and academic groundwork to provide intellectual scaffolding. Without a deliberate position, Finland's default is whatever the next government's default is — and the cost of continued silence is that the discourse is shaped, in the meantime, by Sweden, Czechia, the United States, and others.

The eighteen-month window opens with Sweden's filing (October 2024) and closes with the autumn 2026 Eduskunta budget cycle, by which point a Finnish position should be either on the record or formally deferred. Acting in 2026 means leading. Acting in 2027 means following.

[^whitehouse]: Multiple media reports, May 2026. See [White House Adviser: U.S. Bitcoin Reserve Announcement Coming Soon, HokaNews](https://www.hokanews.com/2026/05/white-house-adviser-says-bitcoin.html).

[^sweden_quote]: Translated from the Swedish original. The motion's reasoning section names Finland and Norway specifically as comparator states. See [Sweden Eyes First-Ever National Bitcoin Reserve Amid Geopolitical Tensions, TradingView](https://www.tradingview.com/news/cryptonews:fab316eaa094b:0-sweden-eyes-first-ever-national-bitcoin-reserve-amid-geopolitical-tensions/).

[^bhutan]: [Bhutan Transfers 100 BTC Worth $8.1M as Sovereign Reserve Drops to $252M, BanklessTimes, 12 May 2026](https://www.banklesstimes.com/articles/2026/05/12/bhutan-transfers-100-btc-worth-8-1m-as-sovereign-reserve-drops-to-252m/).

[^swiss]: [Swiss Bitcoin Reserve Campaign Fails to Gather Enough Signatures, HokaNews, May 2026](https://www.hokanews.com/2026/05/swiss-bitcoin-reserve-campaign-fails-to.html).

---

# 2. The Three-Track Operating Model

The recommendations are sequenced. Track A can begin immediately with no new legislation. Track B requires a single legislative amendment. Track C requires a parliamentary debate and a Suomen Pankki working paper. Each track can succeed independently of the others, but the credibility and operational competence required for Track C accumulates through Tracks A and B.

## Track A — Establish a published governance framework for state-held digital assets

The starting condition is operational, not strategic. Finland already custodies digital assets that arrive through law-enforcement seizure — primarily Bitcoin from criminal-investigation forfeitures stretching back to a major Tulli (Finnish Customs) case in 2016. These holdings are managed across at least three agencies: Tulli, Verohallinto, and the prosecutorial offices that handle individual seizure cases. Liquidation decisions are made on a recurring basis. No published framework governs how those decisions are made. No defined cadence reports the resulting flows to Eduskunta. No coherent strategic logic links the operational reality to any stated policy.

This is not, in any meaningful sense, a "Bitcoin reserve." It is a custody footprint that exists by accident, governed by default. Track A formalizes the framework that the operational reality already implies.

**The mandate.** A single named supervisory authority — recommended to be Suomen Pankki, in coordination with Tulli, Verohallinto, and the Ministry of Finance — consolidates accountability for state-held digital assets. Further liquidation is deferred pending a formal parliamentary review. Quarterly transparency reports list total holdings, custodial arrangement, agency-level provenance, and net change since the prior period.

**What this changes.**
- The fragmented custodial reality becomes legible to Eduskunta, journalists, and the public.
- Liquidation becomes a deliberate policy act rather than a default operational choice. The lesson of past liquidations between 2017 and 2019, conducted at then-prevailing prices in the absence of any sovereign-reserve framework, is not that those decisions were wrong by the standards of the time — it is that "liquidate at market" is not a neutral default. It is an active policy taken without published guidance.
- The intellectual and operational scaffolding for Track B is established: Finland develops the published framework, the custodial competence, and the reporting cadence before being asked to commit to a permanent reserve.

**What this does not require.**
- New monetary policy.
- Bitcoin purchases.
- A change to the Currency Act, the Bank of Finland Act, or the Treaty implementing the Euro.
- European Central Bank approval. (This is administrative custody, not monetary policy.)

**What is required.**
- An interagency Memorandum of Understanding between Tulli, Verohallinto, the prosecutorial offices, Suomen Pankki, and the Ministry of Finance.
- A nominated Officer for Digital Reserves — a single named individual within Suomen Pankki — accountable for the framework.
- A quarterly reporting cadence aligned with Suomen Pankki's existing reserves reporting.
- An audit relationship with the State Audit Office (Valtiontalouden tarkastusvirasto, VTV) for independent verification.

**Timeline.** Six to nine months. Most of which is interagency negotiation, not technical work.

## Track B — Establish the legal mechanism for permanent sovereign accumulation

**The mandate.** A one-time amendment to the Confiscation Act (Pakkokeinolaki) provides that Bitcoin and other digital assets obtained through law-enforcement seizure, after all due-process and forfeiture procedures are exhausted, enter a permanent sovereign reserve held under the Track A framework — rather than being liquidated to euros as a matter of course. A discretionary mechanism permits liquidation in cases where the original victim's restitution is best served by euro recovery.

**What this changes.**
- Finland establishes the *legal mechanism* for budget-neutral sovereign Bitcoin accumulation. The mechanism is the relevant policy artifact; the immediate flow rate is incidental.
- Finland aligns structurally with the U.S. Strategic Bitcoin Reserve framework (March 2025), which uses the same mechanism, and positions ahead of the Swedish opposition proposal (October 2024), which contemplates the same mechanism but has not yet been adopted.
- Finland creates a stable answer to the question "what happens to the next major seizure?" — a question that will recur, and that absent Track B will continue to be answered by default.

**What is required.**
- A single legislative amendment to the Confiscation Act allowing non-liquidation of seized digital assets, with the discretionary euro-recovery mechanism noted above.
- The custodial capacity established in Track A.
- An audit and accountability extension covering the new permanent-reserve flow.

**Risk considerations.**
- *Volatility.* Track B does not require Finland to hold Bitcoin against operational liabilities. The reserve is a long-duration strategic asset, comparable to gold. Mark-to-market volatility is accounting noise, not policy risk.
- *Operational security.* Custody risk is the dominant operational concern. The three-tier architecture in Section 3 is designed to mitigate it.
- *Political reversal.* A future government may choose to liquidate. This is acceptable — the legislative framework should make any future liquidation a deliberate parliamentary act rather than a default operational choice.

**Timeline.** Twelve to eighteen months from first reading to Presidential assent.

## Track C — Strategic allocation

**The mandate.** A modest allocation — proposed at 0.5% of Finland's foreign exchange reserves, phased over five years — is acquired through periodic purchases at Suomen Pankki's discretion. The allocation is reviewed annually and may be increased to a ceiling of 2% or decreased to zero based on performance, geopolitical context, and Suomen Pankki's judgment.

**What this changes.**
- Finland's reserves include a small but deliberate exposure to a non-sovereign, non-fiat asset class.
- Finland joins a small set of nations (likely the U.S., possibly Sweden and Czechia) that have made active Bitcoin reserve allocation decisions through formal parliamentary process.
- Finland establishes operational competence in purchasing and custody at meaningful scale — competence that becomes valuable independent of Bitcoin's specific trajectory, as digital-asset infrastructure increasingly intersects with sovereign-asset management.

**What is required.**
- A Suomen Pankki working paper on the case for and against allocation, modelled on existing diversification analyses for gold and non-euro currencies.
- An Eduskunta debate and a formal motion authorizing the allocation, with explicit ceilings and a review cadence.
- The operational capacity built in Tracks A and B.

**Risk considerations.**
- *Volatility.* Bitcoin's one-year volatility historically exceeds 60%. At 0.5% allocation, a 90% drawdown represents 0.045% of total reserves — below the noise of normal reserve fluctuations.
- *ECB optics.* The ECB does not approve member-state reserve composition. Some Governing Council members will privately criticize. The political cost of mild criticism is acceptable in exchange for the strategic value of the position.
- *Counterparty risk.* Acquisition mechanism matters. Direct OTC purchase through regulated counterparties is preferable to exchange-based acquisition. Custody is handled per the Track A framework and the architecture in Section 3.

**Timeline.** Eighteen to thirty-six months from Suomen Pankki working paper to first allocation tranche.

---

# 3. Custody Architecture

Custody is the operational hinge. A sovereign Bitcoin reserve that is custodied poorly is a strategic liability; one that is custodied well is a long-duration asset on par with gold.

The proposed architecture is three-tier.

**Tier 1 — Suomen Pankki cold storage.** The majority of holdings (recommended: 80%+) are held in deep cold storage under Bank of Finland direct custody. This means air-gapped key generation, multi-signature controls (recommended: 3-of-5 with geographic key distribution), hardware-security-module-backed key storage, and no internet-connected systems holding any part of the spending capability. The keys never leave the Bank's secure facilities. The operational analogue is the Bank's existing gold vault: physical security with cryptographic equivalents.

**Tier 2 — Institutional partner custody.** A smaller portion (recommended: up to 20%) is held with one or more regulated institutional custodians (such as BitGo, Coinbase Custody, Anchorage, Fireblocks, or a Nordic alternative). This tier exists for operational liquidity — if Finland ever needs to move Bitcoin quickly (for example, to a settlement counterparty or to meet an unexpected obligation), Tier 2 is the operational layer that does not require unwinding Tier 1's cold storage. Vendor selection should be open, competitive, and reviewed every two years.

**Tier 3 — Independent audit and proof-of-reserves.** A third party (recommended: the State Audit Office VTV, with technical support from an independent cryptographic auditor) verifies on a quarterly basis that the addresses claimed in the transparency report are controlled by the Bank — by signing a randomly-selected challenge transaction or providing equivalent cryptographic proof. This layer is what gives the reserve political legitimacy. Without proof-of-reserves, a sovereign Bitcoin reserve is a claim. With it, the reserve is a verifiable fact.

The cost of this three-tier architecture, including initial setup, is estimated at €1.5–3.0 million in years one and two, declining to €300–500k annually thereafter. For reference, this is a fraction of one percent of Suomen Pankki's annual operating expenses.

**A note on what custody is not.** Custody is not the same as exposure. A sovereign reserve can have Bitcoin exposure without holding Bitcoin directly — through spot-Bitcoin ETF positions or via any future IMF mechanism. The author's view is that direct custody is strictly preferable, because it preserves Finland's optionality and operational competence in a future in which non-direct exposure may become politically constrained (for example, if the issuer of a Bitcoin ETF becomes subject to sanctions, regulatory capture, or a hostile government's leverage). Direct custody is sovereign. Synthetic exposure is not.

---

# 4. Political Sequencing

The technical content of this whitepaper is the easy part. The political sequencing is the hard part. The proposal must be framed differently for each major Finnish party, while remaining substantively identical.

**Kokoomus (National Coalition Party).** The frame is **national sovereignty over money**. Bitcoin is the digital evolution of gold; central banks have held gold for centuries to preserve sovereign optionality outside the dominant fiat system; a Bitcoin reserve continues that tradition into the digital era. This frame aligns with Kokoomus's existing positions on Finland's independence within EU monetary arrangements and on prudent reserve management.

**Perussuomalaiset (Finns Party).** The frame is **independence from ECB monetary policy**. The ECB's balance sheet has grown by over 400% since 2009; eurozone monetary debasement is a structural risk; a Bitcoin reserve is a hedge against debasement and a signal that Finland's monetary thinking is not entirely subordinated to Frankfurt. This frame aligns with the party's existing positions on Finland's monetary independence.

**Keskusta (Centre Party).** The frame is **digital infrastructure for the next economic era**. Finland led the previous digital era (Nokia, Linux, MySQL, IQM, Wolt, Supercell). Bitcoin is foundational digital infrastructure for the next era of value transfer. Finland should lead, not follow. This frame aligns with Keskusta's existing positions on regional digital infrastructure and Finland's role as a small, innovative economy.

**SDP (Social Democratic Party).** The frame is **operational competence and energy infrastructure**. The Bitcoin mining industry is one of the few economic sectors that can recover and monetize stranded or seasonal energy — particularly relevant in Finland, where electricity production exceeds consumption in shoulder seasons. A sovereign reserve creates the political conditions for a Finnish Bitcoin mining strategy that recovers waste heat, supports rural electrification economics, and creates skilled jobs.

**Vihreät (Green League).** The frame is **transparency and audit**. A properly-constructed Bitcoin reserve is the most transparent reserve asset in history — every transaction is publicly verifiable. This frame aligns with Vihreät's positions on public-finance transparency and government accountability. The custodial energy footprint can be addressed by mandating renewable or stranded-energy mining for any Finnish state-related operations.

**Vasemmistoliitto (Left Alliance).** The frame is **systemic diversification**. The 2008 and 2023 banking crises demonstrated the fragility of fiat reserve systems; a small diversification into a non-correlated asset class is a prudent hedge for working-class Finns, whose pension funds and state services depend on Finland's monetary stability.

**RKP (Swedish People's Party).** The frame is **Nordic cooperation and competitiveness**. Sweden has filed. Norway is studying. Estonia is interested. If Finland does not move, Finland's competitiveness in the Nordic digital-finance corridor declines.

**Sequencing in calendar terms.**

| Phase | Activity | Timing |
|---|---|---|
| 0 | Whitepaper publication, press, stakeholder briefings | Months 1–2 |
| 1 | Informal cross-party MP meetings, working group formation | Months 3–6 |
| 2 | Formal Eduskunta motion (Track B amendment) | Months 6–12 |
| 3 | Suomen Pankki working paper (Track C analysis) | Months 12–18 |
| 4 | Implementation of Tracks A and B | Months 18–24 |
| 5 | Track C debate and decision | Months 24–36 |

This is a three-year horizon. It is achievable.

---

# 5. The Finnish edge

Finland is structurally well-positioned to lead this question among small European economies. Five reasons.

**Cheap nuclear electricity.** Finland brought Olkiluoto 3 online in 2023, adding 1.6 GW of baseload nuclear capacity. Finnish wholesale electricity prices are among the lowest in the Nordics during winter months. This is the relevant comparator for any Bitcoin-related infrastructure — mining, custody operations, data-centre security — and a competitive advantage that does not exist for, say, Germany.

**Cold climate.** Free cooling for data centres and high-density compute infrastructure for approximately eight months per year. This is the same comparative advantage that has attracted hyperscale data-centre investments from Google (Hamina), Microsoft (Espoo), and others. It applies equally to any cryptographic-custody infrastructure.

**Engineering credibility.** Finland has produced disproportionate contributions to the digital infrastructure of the modern era. Linus Torvalds (Linux). Martti Malmi, who worked directly with Satoshi Nakamoto on early Bitcoin development. The Nokia engineering culture that seeded a generation of Finnish startups. MySQL's roots. IQM's quantum-computing work. Wolt. Supercell. Finland is not a country attempting to credibly enter digital infrastructure for the first time. It is a country resuming a role it has held before.

**High-trust governance.** Finland ranks consistently among the top three countries globally on the Transparency International Corruption Perceptions Index. The institutional credibility of Finnish governance — Suomen Pankki, the Ministry of Finance, the State Audit Office — is internationally recognized. A Finnish sovereign Bitcoin reserve will be credibly managed in a way that analogous reserves in many other jurisdictions would not be. This is itself a soft-power asset.

**Mature regulatory framework.** The Finnish Financial Supervisory Authority (FIN-FSA, Finanssivalvonta) has supervised crypto-asset service providers since 2019, predating MiCA. Finland's MiCA implementation has been among the cleanest and earliest in the EU. The legal scaffolding for sovereign engagement with digital assets is already present.

The combination is rare. There are perhaps five countries in the world that combine all five characteristics. Among small European economies, Finland is uniquely positioned.

---

# 6. Counter-arguments and replies

Five objections recur in conversations with policymakers, central-bank staff, and journalists. Each is addressed below. Serious additional objections will be added to this section in future revisions of this document; the GitHub issue tracker is the venue for proposing additions.

**Objection 1: "Bitcoin's volatility makes it unsuitable for sovereign reserves."**

Reply: One-year volatility is high. Five-year and ten-year volatility, in returns terms, is positive and substantially exceeds traditional reserve assets. The relevant question is not "is Bitcoin volatile?" — it is — but "what allocation size makes the volatility immaterial to total reserves?" The proposal here (Track C at 0.5%) is calibrated so that even an extreme 90% drawdown represents less than 0.05% of total reserves. This is below the noise of normal reserve fluctuations.

**Objection 2: "The European Central Bank will not approve."**

Reply: The ECB approves member-state monetary policy. It does not approve the composition of member-state foreign exchange reserves. Germany holds gold. Italy holds gold. Finland already holds gold. The legal framework for member-state reserve composition is unambiguous: it is a national competence under the Treaty on the Functioning of the European Union. The ECB has been notably silent on sovereign Bitcoin reserves precisely because the question lies outside its mandate.

A related concern is reputational: will an ECB Governing Council member privately criticize Finland's move? Almost certainly some will. The political cost of mild criticism is acceptable in exchange for the strategic value of the position. Finland has weathered ECB skepticism on multiple prior issues (notably during the 2010–2015 sovereign debt crises) and survived it.

**Objection 3: "Bitcoin is used for illicit activity."**

Reply: This argument has been deployed against every novel financial technology since at least the Medici banks: gold, paper currency, Swiss bank accounts, cash, the internet itself. In every instance, the argument was technically true and politically useful — and in every instance, the technology became part of legitimate financial infrastructure.

The empirical fact is that Bitcoin transactions are publicly visible on the blockchain. Modern law-enforcement and intelligence agencies have well-developed capabilities for tracing on-chain flows. The U.S. Treasury's Office of Foreign Assets Control sanctioned the Tornado Cash mixer in 2022 precisely because such tracing works. Cash, by contrast, is genuinely untraceable. The illicit-activity argument applies more strongly to cash than to Bitcoin.

**Objection 4: "This signals that Finland accepts cryptocurrency as legitimate."**

Reply: Yes, and that is the point. MiCA already accepts cryptocurrency as legitimate. Finland is bound by MiCA. The question is whether Finland leads the implementation, follows it, or resists it. This proposal recommends leading.

Refusing to engage with the question does not make the question disappear. It simply means that Finland's eventual position will be defined by other actors — the U.S., Sweden, Czechia, and the ECB — rather than by Finland itself.

**Objection 5: "Ray Dalio has stated that Bitcoin's transparency makes it unlikely to become a central-bank reserve asset."[^dalio]**

Reply: Dalio's argument is specifically about central banks needing to act covertly to manage their currencies — for example, by selling reserve assets quietly to defend a peg. This concern applies primarily to central banks of countries with managed-float or pegged currencies, where the timing of intervention matters enormously.

It does not apply to Finland. The eurozone does not maintain a managed-float; the euro floats freely against major counterparts; Finland's reserve operations are not central to active currency defense. A transparent reserve asset is, for a country in Finland's position, a credibility *advantage*, not a liability. Every transaction is auditable. Every holding is verifiable. This is the opposite of a problem for a country whose institutional brand is built on transparency.

The Dalio argument is correct for its intended target (managed-float central banks). It is not correct for Finland.

[^dalio]: [World's Largest Hedge Fund Founder Says Bitcoin Transparency Makes it Unlikely to Become a Central Bank Reserve Asset, BitcoinKE, May 2026](https://bitcoinke.io/2026/05/bitcoin-transparency-limits-its-reserve-asset-status/).

---

# 7. Three concrete first moves in 2026

If the recommendations above sound large, the following three actions can be taken in 2026 with no new legislation, no Eduskunta motion, and no Suomen Pankki working paper. They are first steps that build optionality without committing Finland to any particular path.

**Move 1: Appoint a Suomen Pankki Officer for Digital Reserves.**

A single named individual within Suomen Pankki — at minimum a Director-level appointment — is given responsibility for monitoring the international sovereign Bitcoin landscape, briefing the Board on developments, and serving as the public point of contact for digital-reserve questions. This role does not require purchasing Bitcoin or changing policy. It requires reading, attending international meetings, and reporting. The annual cost is well under €200,000.

**Move 2: Publish a quarterly transparency report on Finland's operational digital-asset footprint.**

The data exists; it is simply not published on a defined cadence. The first transparency report can be issued in Q3 2026, listing: which agencies currently custody digital assets, under what statutory basis, at what aggregate level, with what change since the prior period, and with any liquidation events explained. This requires no new policy — only that existing operational facts be made legible to Eduskunta and the public. The political effect is significant: it forces every subsequent administration to either continue the disclosure or explain why it has been discontinued.

**Move 3: Convene a cross-party Eduskunta working group.**

Four MPs from four different parties, one year of work, output a non-binding white paper. This mirrors the Swedish parliamentary path. Estimated direct cost: under €100,000. The output is a Finnish-government-authored framework that becomes the reference document for any subsequent legislative work. If the working group recommends no action, Finland has lost very little. If the working group recommends Track A or B, the political legitimacy of the proposal is established.

The combined cost of these three moves is under €500,000. The political and strategic optionality created is substantial.

---

# 8. Conclusion

Three observations close this document.

**First, the policy environment is permissive, not hostile.** The United States is moving. Sweden is moving. Czechia is moving. The ECB is silent. The Finnish institutional infrastructure (Suomen Pankki, FIN-FSA, VTV, the Confiscation Act) is sufficient to support the proposal with marginal amendments. The constraint on Finnish action is not external; it is internal will.

**Second, the cost of inaction is rising.** Every quarter that Finland does not take a position is a quarter in which Sweden, Norway, the United States, and Czechia define the European and Nordic discourse on Finland's behalf. The leadership position Finland can take in May 2026 — as the country Sweden itself named — is not the same position Finland can take in May 2027, when there will already be three or four European jurisdictions with formal reserve frameworks and Sweden's anxiety about Finland will have proved unfounded. The first-mover advantage is real and decaying.

**Third, the case is structural, not ideological.** This whitepaper does not require the reader to be enthusiastic about Bitcoin. It requires only that the reader believe (a) Finland should maintain optionality over its reserve composition, (b) sovereign assets should be governed transparently, (c) the international policy direction is sufficiently settled that Finland needs a position rather than an absence, and (d) Finland should not default to following others on a question where it could lead.

If those four propositions are accepted, the three-track operating model proposed here is the conservative path. The riskier path is doing nothing.

---

## About the author

Jukka Blomberg is the founder of [NorthPoint](https://northpoint.fi), a Helsinki-based marketing-and-compliance consultancy for crypto firms. He served as Chief Marketing Officer at two international cryptocurrency exchanges between 2017 and 2024, where he worked directly with regulators, listing committees, and treasury teams across Europe, Asia, and the Middle East. He writes at [northpoint.fi/resources/writing](https://northpoint.fi/resources/writing).

This whitepaper is published in personal capacity. The opinions are the author's own and do not necessarily reflect those of any current or former employer.

## Acknowledgements

To be added in subsequent revisions, with permission, as substantial contributors and reviewers are credited. If you wish to be acknowledged for review, citation, or feedback, please contact the author or open a pull request.

## How to cite

Suggested short form:

> Blomberg, J. (2026). *Finland's Path to a Sovereign Bitcoin Reserve: Operating Model, Custody, Political Sequencing.* Version 0.2. https://github.com/jukkablomberg/finnish-bitcoin-reserve

Full citation metadata is available in [CITATION.cff](../CITATION.cff).

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC-BY 4.0)](../LICENSE). You are free to share and adapt, including for commercial purposes, with appropriate credit.

---

*Version 0.2 — published 13 May 2026.*
*Source repository: https://github.com/jukkablomberg/finnish-bitcoin-reserve*
*Landing page: https://northpoint.fi/whitepapers/finnish-bitcoin-reserve*
