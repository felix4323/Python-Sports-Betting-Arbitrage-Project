# Python Sports Betting Arbitrage Project

Python project analysing sports betting arbitrage opportunities across 3,100 professional men's tennis matches using historical best available closing odds.

This project investigates how arbitrage opportunities vary across tournament level, surface, and round, and includes a backtest of an arbitrage betting strategy.

## What is a Sports Betting Arbitrage?

A sports betting arbitrage occurs when differences in bookmaker odds create an opportunity to generate a theoretically guaranteed profit by placing bets on all possible outcomes.

The notebook explains the arbitrage calculation and stake allocation methodology in detail.

## Objectives

The main objective of this project was to investigate potential drivers of sports betting arbitrage opportunities by comparing arbitrage opportunities across different tournament levels, surfaces, and rounds.

A betting strategy was also backtested using historical odds to estimate theoretical profitability. 

## Data

The dataset analysed contains the best available closing odds for both players across 3,100 professional men’s tennis matches. The best available closing odds represent the highest available odds for each player shortly before the match begins. 

The historical odds were manually collected from a website providing historical best available closing odds. The underlying dataset is not included in this repository due to restrictions on publicly redistributing the source data.

## Methodology 

The analysis is split into four main stages:
- Arbitrage detection: identifying matches where the closing odds created an arbitrage opportunity.
- Stake allocation: for each identified arbitrage opportunity, the optimal stake allocation was calculated for both outcomes.
- Market analysis: comparing the frequency and magnitude of opportunities by tournament level, surface, and round.
- Backtesting: historical odds were used to estimate the strategy's theoretical returns.

## Key Findings

- Identified 216 arbitrage opportunities across 3,100 matches, representing approximately 7% of the matches analysed.
- Lower tournament levels showed greater arbitrage potential, but opportunities may be harder to capitalise on due to fewer available bookmakers and lower betting limits.
- Found that grass-court matches had the highest average arbitrage return per match across the surfaces analysed.
- The backtest produced a best-case theoretical profit of £1,089 based on £100 stakes per arbitrage opportunity. 

## Backtest Assumptions & Limitations

The £1,089 result represents a best-case theoretical profit, assuming that £100 could be staked on every opportunity and that the best closing odds could be successfully executed.

In practice, odds may change before bets can be placed, bookmakers have limits, and rules can differ between bookmakers. In particular, player retirements may result in one bet being voided and another not. This could reduce the theoretical profit. 

A rough estimate suggests that accounting for this could reduce the profit to around £750, although this estimate does not account for other bookmaker limits, restrictions, or execution difficulties.

## Tools & Libraries
- Python
- Matplotlib
- Jupyter Notebook
