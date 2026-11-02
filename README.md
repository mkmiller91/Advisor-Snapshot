# Client Snapshot: Advisor Planning Tool

An interactive, browser-based tool for financial advisors. Enter a client's fact-finder numbers and get net worth, life insurance needs, retirement readiness, a debt payoff comparison and a college funding estimate on one printable page.

**Live tool:** https://mkmiller91.github.io/Advisor-Snapshot/

## What it does

| Tab | What you get |
|---|---|
| **Overview** | A retirement readiness gauge, key numbers (net worth, monthly surplus, insurance gap, extra saving needed) and plain-language observations such as emergency fund months and coverage gaps. |
| **Balance sheet** | Assets and liabilities as stacked bars, net worth, and liabilities as a share of assets. |
| **Protection** | Life insurance need using the DIME method (Debt, Income, Mortgage, Education) compared with coverage already in force. |
| **Retirement** | A projection chart in today's dollars with hover values, plus what-if sliders for retirement age, extra savings and desired income. Save two scenarios and compare them side by side. |
| **Debt payoff** | Current payment vs. current payment plus an extra amount: time to payoff, total interest, interest saved. |
| **College** | Future cost at enrollment, amount needed, projected savings, percent funded and the extra monthly saving required. |

Other features: sliders next to key inputs, optional firm name, advisor name and logo for the report header, and a print / save-as-PDF view that produces a clean client summary.

## How to use it

1. Open the live link (or open `index.html` in any browser).
2. Click **Load sample** to see an example client, or **Clear** and enter your own numbers in the left panel.
3. Move between tabs to explore each area. Drag the sliders on the Retirement tab to test scenarios.
4. Click **Print / save PDF** to produce a report.

## Privacy

Everything runs in the browser. No client data is sent to a server, stored, or tracked. Refreshing the page clears all entries. An uploaded logo stays in the browser as well.

## How the numbers work

- **Net worth:** total assets minus total liabilities.
- **DIME need:** non-mortgage debt + (annual income x years of income to replace) + mortgage balance + education funding. The gap is the need minus existing coverage.
- **Retirement:** projections use real (inflation-adjusted) returns, so all values are in today's dollars. Taxable and retirement balances are combined, contributions are made at year end, and withdrawals happen at the start of each year. The yearly withdrawal is desired income minus Social Security. "Needed at retirement" is the present value of those withdrawals through the plan-through age. "Extra saving needed" is the shortfall spread over the remaining contribution years.
- **Debt payoff:** fixed rate, monthly compounding, no new borrowing. If the payment does not cover monthly interest, the tool reports that the debt is never paid off.
- **College:** costs start at age 18 and rise with college cost inflation. Savings keep earning while the student is enrolled. Contributions are made at month end.

## Limitations

This is a planning illustration, not a full financial plan. It does not model taxes, fees, market volatility, financial aid, Social Security claiming strategy or changing income. Results depend entirely on the assumptions entered.

## Disclaimer

For education and illustration only. This tool does not provide investment, insurance, tax or legal advice.

## Built with

Plain HTML, CSS and JavaScript in a single file, with no frameworks or build step. Charts are drawn with inline SVG. The only external resource is Google Fonts, and the page still works if it fails to load. Hosted with GitHub Pages.

## Roadmap

- Monte Carlo simulation of market returns
- Tax-aware retirement withdrawals
- Social Security claiming-age comparison
- Saving and loading client scenarios

## Author

Created by **Michael Miller**, Economics (Financial Services) student at Widener University, with AI assistance from Claude (Anthropic). Calculations were reviewed and checked by hand.

Contact: mkmiller@widener.edu | [LinkedIn](https://www.linkedin.com/in/michael-miller06)
