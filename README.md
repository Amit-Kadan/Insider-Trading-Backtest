# Insider-Trading-Backtest
# Systematic Insider-Purchase Backtest

A redacted research case study examining short-term price behavior following SEC Form 4 insider-purchase disclosures.

## Project Overview

I developed a systematic, event-driven trading strategy designed to identify short-term price dislocations following insider-purchase disclosures. The strategy was implemented and backtested in Python using the QuantConnect LEAN engine.

## Research Question

Do publicly disclosed insider purchases contain information that can systematically predict short-term stock-price movements?

## Data and Testing Framework

* 450+ point-in-time insider-purchase signals
* SEC Form 4 filing and transaction data
* Backtest period from 2022 through 2026
* Timestamp-aligned entries designed to reduce look-ahead bias
* Event-driven portfolio construction and execution
* Commission, slippage, position, and liquidity stress testing

## Methodology

The system processes qualifying insider-purchase disclosures, schedules entries according to when information became publicly available, manages portfolio exposure, and evaluates predetermined exit conditions.

Multiple versions were tested to measure how transaction costs, execution assumptions, and liquidity limitations affected performance. Proprietary screening criteria, signal data, and exact execution logic are intentionally omitted.


## Execution and Risk Testing

The constrained model incorporated more conservative assumptions for:

* Trading commissions
* Slippage
* Volume participation
* Position sizing
* Portfolio concentration
* Security-level liquidity

This reduced headline returns but provided a more realistic estimate of performance under practical execution constraints.

## Technology

* Python
* QuantConnect LEAN
* Event-driven backtesting
* SEC Form 4 data
* Point-in-time signal processing

## Limitations

These results are hypothetical and do not represent live trading performance. Backtested results may be affected by data quality, model assumptions, market impact, security availability, and changing market conditions. Small-cap securities may also have limited strategy capacity.

## Repository Scope

This public repository contains a redacted overview of the research and selected backtest results. Proprietary signal data, screening criteria, and implementation code are intentionally excluded.
