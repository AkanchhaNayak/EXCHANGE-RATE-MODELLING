Exchange Rate Modelling: Currency Futures, Evolution and Market Analysis

An empirical study of currency futures with a focus on the USD/INR futures market. The project traces the evolution of currency futures, reviews the global and Indian literature, links pricing theory to data, and models volatility with GARCH(1,1). It closes with an India vs Japan comparison and the policy implications for RBI and SEBI.

Author: Akanchha, MA Financial Economics, University of Hyderabad

Table of Contents
Project Overview
Research Questions
Report Structure
Data
Methodology
Key Findings
India vs Japan Case Study
Policy Implications
Limitations
Repository Structure
Tools and Libraries
References
Project Overview

After the collapse of Bretton Woods, floating exchange rates created a need for standardised, exchange-traded hedging tools. Currency futures, first launched at the CME in 1972 and introduced in India in 2008, were the response. This project asks how well these instruments work in practice, using USD/INR as the main case.

The study combines three strands of work:

Theory: Interest Rate Parity, Cost of Carry, the Expectations Hypothesis, the Efficient Market Hypothesis, and arbitrage and hedging theory.
Market analysis: turnover, liquidity and trends in the USD/INR futures market from 2015 to 2025, plus global context.
Econometrics: static hedging analysis (optimal hedge ratio, hedging effectiveness) and dynamic volatility modelling (GARCH(1,1)).
Research Questions
How have currency futures evolved from the post-Bretton Woods era to today?
Does the USD/INR futures market behave the way pricing theory predicts?
How persistent is volatility in USD/INR futures, and how does it relate to liquidity?
How effective are USD/INR futures as a hedging instrument?
How does India's market compare structurally and quantitatively with Japan's?
What do the results imply for regulation and policy?
Report Structure
Section	Content
I. Introduction	Background, motivation, and a summary of the research trajectory
II. Evolution of Currency Futures	From fixed rates to floating, the birth of futures, and how markets differ today
III. Review of Literature	Global perspective (Hodrick and Srivastava, Dale, Harvey and Huang, Lien and Yang, Rothig, Rosenberg and Traub) and Indian perspective (Upadhyay, Bhanumurthy, Sahu, Kaur and Singh, Mirchandani, Kharbanda and Singh)
IV. Theoretical Underpinning	IRP, Cost of Carry, Expectations Hypothesis, EMH, arbitrage and hedging theory, supporting theories (PPP, CIA, UIP)
V. Market Analysis	Market size and volume, liquidity analysis (2015 to 2025), trade and turnover across exchanges, volatility analysis
VI. Case Study	Structural and quantitative comparison of the Japanese and Indian futures markets
VII. Challenges	Ten challenges, from market risk and basis risk to regulation and hedging efficiency
VIII. Policy and Regulatory Implications	Implications for RBI, SEBI and exchanges
IX. Conclusion	Summary of findings and the policy paradox
X. References	Academic sources
Data
Item	Detail
Instrument	USD/INR futures (settlement prices) and USD/INR spot
Source	Investing.com historical data (futures and spot series)
Sample	2,407 daily observations, converted to daily log returns
Turnover and volume	Exchange and SEBI annexure tables (NSE, BSE, MSEI); 2015 to 2025
Global context	BIS Triennial Survey (OTC FX turnover), CME Group statistics
Case study data	CME Group contract specifications and market data for JPY and INR futures
Methodology

1. Static analysis (hedging)

Annualised standard deviations of futures and spot returns
Pearson correlation between spot and futures returns
Optimal Hedge Ratio: OHR = ρ × (σS / σF)
Hedging Effectiveness: HE = ρ²

2. Descriptive diagnostics

Kurtosis and the Jarque-Bera test to check normality of returns
Evidence of fat tails and volatility clustering, which motivates GARCH

3. Dynamic analysis (GARCH(1,1))

Constant-mean GARCH(1,1) with a normal distribution, estimated by maximum likelihood with robust covariance
Conditional volatility series extracted and compared with annual trading volume

4. Market and liquidity analysis

Annual and quarterly turnover (USD and INR) with implied average exchange rates
Phase-wise liquidity interpretation: expansion, peak and contraction
Key Findings
Hedging
Metric	Value
Annualised futures volatility	4.96%
Annualised spot volatility	5.10%
Spot-futures correlation (ρ)	0.7688
Optimal Hedge Ratio	0.7901
Hedging Effectiveness (ρ²)	59.10%

A futures position of about 0.79 per unit of spot exposure minimises variance, and futures can cut portfolio variance by more than half.

GARCH(1,1)
Parameter	Estimate
α₁ (shock reaction)	0.0431
β₁ (persistence)	0.9568
α₁ + β₁	≈ 0.9999
Returns are non-normal, with fat tails (Jarque-Bera p ≈ 0.000).
Volatility is extremely persistent: shocks decay slowly, and the largest spikes appear around early 2020 (COVID-19) and 2021.
Conditional volatility fell to near its sample low in late 2024 and early 2025.
Volatility and liquidity
Trading activity rises with volatility. Peak liquidity (2021 to 2022) coincides with high-volatility periods, and the contraction after 2023 coincides with calmer markets.
Average daily turnover fell about 35% in early 2025 compared with 2024.
The implied average USD/INR rate rose from about ₹83.5 (2024) to about ₹86.8 (2025 YTD), roughly a 3.9% depreciation of the rupee.
Theory vs evidence
The strong spot-futures link supports Cost of Carry and arbitrage pricing.
Fat tails and near-unit persistence challenge a smooth EMH and the simple Expectations Hypothesis, and suggest a risk premium for bearing persistent risk.
India vs Japan Case Study
Feature	Japan (JPY futures, CME)	India (INR futures, CME)
Contract size	¥12,500,000	₹5,000,000
Settlement	Physical delivery	Cash settled
Listings	Up to 8 consecutive quarters	12 monthly plus 4 quarterly
Volume (sample contract)	197,891	441
Open interest	304,985	1,248
Market character	Deep, liquid, global hub	Smaller, emerging, more short-term price variability
Regulators	FSA and Bank of Japan	SEBI and RBI
Policy Implications
Volatility persistence: consider temporary margin adjustments, circuit breakers and enhanced surveillance during stress periods.
Participation restrictions: exchange-traded currency derivatives turnover fell from ₹3,61,59,682 crore (FY2023-24) to ₹15,94,263 crore (FY2024-25) after the RBI restricted exchange trading to those with underlying exposure. Much activity moved to OTC forwards. Regulators must balance speculation control against liquidity and transparency.
Exchange vs OTC: exchange-traded FX derivatives are a small fraction of global FX turnover (BIS: US$9.6 trillion per day in April 2025). Better OTC reporting or migrating suitable products to exchanges could improve monitoring of systemic risk.
Risk models: margin frameworks should move from static historical volatility to dynamic models such as GARCH.
Risk premium: policymakers should study how risk premia are priced in the futures market.
Limitations
GARCH(1,1) is symmetric and assumes normal innovations. Extensions (GJR-GARCH, EGARCH, Student-t errors) could capture asymmetry and fatter tails.
The static hedge ratio is a single full-sample estimate, not time-varying. A dynamic hedge (for example, DCC-GARCH) would be a natural extension.
Conclusions about the 2024 to 2025 period rest on a partial year (2025 data run to early March).
Volume and turnover figures come from different sources, units (USD, INR, contracts) and periods, so cross-market comparisons should be read with care.
Exchange-traded FX turnover estimates use a rule-of-thumb share (about 2%) of OTC turnover.
The case study compares single contract snapshots, not long time series.
Repository Structure

(Adjust to match your actual files.)

.
├── README.md
├── report/
│   └── EXCHANGE_RATE_MODELLING.pdf
├── data/
│   ├── usd_inr_futures.csv
│   ├── usd_inr_spot.csv
│   └── turnover_sebi_nse_bse_msei.csv
├── notebooks/
│   ├── 01_descriptive_stats.ipynb
│   ├── 02_hedge_ratio.ipynb
│   └── 03_garch_volatility.ipynb
└── figures/
Tools and Libraries

Python with pandas, numpy, scipy, statsmodels and arch for modelling, and matplotlib for charts. Excel was used for turnover and volume charts.

References

Key sources include Hodrick and Srivastava (1985), Dale (1981), Harvey and Huang (1991), Chakraborty and Barkoulas (2001), Lien and Yang (2006), Rothig (2004), Rosenberg and Traub (2006, 2008), Upadhyay (2009), Bhanumurthy (2004), Sahu (2012), Kaur and Singh (2024), Kharbanda and Singh (2018), plus Hull, Options, Futures, and Other Derivatives, and Madura, International Financial Management. The full list is in Section X of the report.
