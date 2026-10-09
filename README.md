# Datacircle

Datacircle is a data co-op.

Step 1: Query your favorite B2B data APIs through us. Same request, same price, no markup.
Step 2: You're DONE. Every morning, you get the flat file of your data plus everyone else's.

[datacircle.dev](https://datacircle.dev) · [Docs](https://docs.datacircle.dev) · wayne@datacircle.dev

## Benchmarks

Our measures, each with how it was taken. Reuse them, citing datacircle.dev ([CC BY 4.0](LICENSE)).

| Benchmark | What it measures | Taken |
| --- | --- | --- |
| [The US dataset vs LinkedIn](benchmarks/us-dataset-vs-linkedin/) | 3,000 people drawn at random from our US dataset, each checked on LinkedIn: 88% have the same company and title (95% CI: 86% to 89%), 93% the same current company | 2026-10-08 |
| [LinkedIn profile API prices](benchmarks/linkedin-profile-api-prices/) | 12 LinkedIn profile APIs: the price of 1,000 profiles, from each vendor's own pricing page | 2026-10-09 |
| [B2B data API prices](benchmarks/b2b-data-api-prices/) | 17 B2B data APIs: the price of 1,000 people, a profile or a person with a work email | 2026-10-09 |
| [Free plans of B2B prospecting tools](benchmarks/free-b2b-data-plans/) | 7 tools: the most emails and phones their free plans give a month | 2026-10-09 |

Each folder holds its README and the numbers as CSV.

## The call

You send the provider's own request to api.datacircle.dev, with your Datacircle key. That's the only change.

Docs: https://docs.datacircle.dev/api-reference/up2data/enrich-one-linkedin-profile

## What else we have

Free: 10M+ U.S. B2B leads, as a flat file. Download it at datacircle.dev.

Use it from Claude, ChatGPT or Cursor: add api.datacircle.dev/mcp as an MCP server. Docs: https://docs.datacircle.dev/mcp-server

## Questions

**Which APIs?**
Right now we have 2 live LinkedIn profile APIs that we trust: Up2Data and HarvestAPI.

**Is each request live, or cached?**
Live. Each request goes to the provider and gets the profile as it is today.

**So I query my API first, then give you the results?**
No. You query your API through us. That's the only step. You're done.

**How do I get the flat file?**
Add $50 to your account: you get $50 of API PLUS the flat file. Or invite 3 people who sign up.

**What's free?**
Sign up at datacircle.dev with your work email: a $5 credit, that's 4,000 LinkedIn profiles at $1.25 per 1,000.

**What does it cost to refresh N profiles every week?**
N × $1.25 per 1,000, every week, each request live. 9.5K a week: about $12 a week, $48 a month.

**Should I send you my data?**
No. We only take data from live APIs we trust. Even very good data sent to us could be doctored, so we can't use it. Query your API through us, and it goes in the file.

**Why not let people send data, like 5x5?**
5x5 can take data people send because they work with vetted partners. We go through APIs instead.

**If there's no markup, how do you make money?**
The co-op data stays free, as flat files. But a lot of people want a database, so we'll host one for them. That's a separate offer from the API key.

## Contact

wayne@datacircle.dev
