# Contributing to Per Diem Calculator

Thank you for your interest in this project. Please read the guidelines below before opening a pull request.

## How to contribute

1. **Open an issue first** for any non-trivial change so we can discuss the approach before work begins.
2. **Base pull requests on `add-perdiem-tool`**, not `main`.
3. Keep changes focused — one concern per PR.
4. If fixing a bug in one calculator file (`PerDiem-USA.html` or `PerDiem-International.html`), check whether the same fix is needed in the other and include it in the same PR.

## Regulatory references

- **USA**: rates and travel day caps sourced from the [GSA Per Diem API](https://api.gsa.gov/travel/perdiem/v2/) and [GSA CONUS M&IE Breakdown table](https://www.gsa.gov/travel/plan-book/per-diem-rates/mie-breakdown). Deduction logic follows FTR Chapter 301.
- **International**: rates from the [State Dept Foreign Per Diem Rates](https://allowances.state.gov/web920/per_diem.asp); meal breakdown from [FTR 301 Appendix B](https://allowances.state.gov/Bypass/AppendixB.asp).

Any PR that changes reimbursement amounts or deduction logic must cite the specific FTR section or GSA/State Dept page that supports the change.

## Unsolicited commercial contributions

This repository has received automated PRs from commercial services that submit technically correct fixes as a lead-generation tactic. We evaluate all PRs on technical merit, but **we do not engage with, sign up for, or endorse any third-party project management or tracking service**. If your PR body promotes a commercial product or service, it will be closed without comment.
