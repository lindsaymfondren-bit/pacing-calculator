# Pacing Calculator

A lightweight ad pacing calculator that estimates impressions remaining, needed per day, and a daily budget estimate using planned CPM and yesterday’s effective CPM.

## What it does

This tool helps with quick pacing checks by calculating:

- Estimated Total Impressions
- Impressions Remaining
- Needed Per Day
- Yesterday’s Effective CPM
- Daily Budget Estimate Based on Yesterday’s Effective CPM

It is meant to be a simple pacing aid, not an automated budgeting tool.

## Inputs

The calculator uses:

- Budget
- CPM (Planned/Input)
- Impressions So Far
- Days Left
- Yesterday’s Impressions
- Current Daily Budget

## How it works

### 1. Estimated Total Impressions
`(Budget / CPM) * 1000`

### 2. Impressions Remaining
`Estimated Total Impressions - Impressions So Far`

### 3. Needed Per Day
`Impressions Remaining / Days Left`

### 4. Yesterday’s Effective CPM
`(Current Daily Budget / Yesterday’s Impressions) * 1000`

### 5. Daily Budget Estimate Based on Yesterday’s Effective CPM
`(Needed Per Day / 1000) * Yesterday’s Effective CPM`

## Why it uses two CPMs

This calculator includes both:

- **Planned/Input CPM** — the CPM from the budget sheet or planning assumptions
- **Yesterday’s Effective CPM** — a recent-delivery CPM based on actual impressions from the previous day

These may be very different. That does not necessarily mean something is wrong. It may reflect changing delivery conditions, mixed ad sets, or differences between planning assumptions and real-world performance.

## Important notes

- Best used for a **single campaign, ad set, or tactic** with a reasonably consistent CPM
- Blended client totals with multiple ad sets, tactics, or mixed CPMs may produce misleading results
- Yesterday’s Effective CPM can vary significantly day to day
- This tool is a pacing aid, not a final budget recommendation engine

## Disclaimer

Use judgment before making budget changes.

This calculator is designed to support pacing decisions, not replace platform behavior, account knowledge, or human decision-making.

## Use case

This tool is useful for quick pacing checks when you want to compare:

- what the campaign was expected to deliver based on planned CPM
- what recent delivery suggests based on yesterday’s actual performance

## Future improvements

Possible future additions:

- platform-specific notes or logic
- search-specific pacing mode
- budget remaining / spend-so-far version
- campaign-level saving/export
- more explicit pacing warnings

## Built with

- HTML
- CSS
- JavaScript# pacing-calculator
