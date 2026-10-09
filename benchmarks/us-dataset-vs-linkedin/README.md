# The US dataset vs LinkedIn, October 2026

How many people in a B2B dataset still have the company and title the dataset says? We drew 3,000 people at random from Datacircle's US dataset (the snapshot of 2026-10-04: 43.6M people in the 50M+ file, the 10M+ file a subset of it, [docs](https://docs.datacircle.dev/files)) and looked each one up on LinkedIn on 2026-10-08.

**88% have the same company and the same title on LinkedIn** (95% CI: 86% to 89%, 2,628 of 3,000). 93% have the same current company.

The same benchmark on datacircle.dev: https://datacircle.dev/b2b-data-accuracy

## Results

| Measure | Share | 95% CI | Count |
| --- | --- | --- | --- |
| Same company and same title | 88% | 86% to 89% | 2,628 of 3,000 |
| Same current company | 93% | 92% to 93% | 2,776 of 3,000 |
| LinkedIn URL still works | 97% | 96% to 97% | 2,901 of 3,000 |

## Where the other 12% are

| Against LinkedIn | Share | Count |
| --- | --- | --- |
| Same company, same title | 88% | 2,628 |
| Same company, different title | 5% | 148 |
| Different company | 1% | 34 |
| We have a company, LinkedIn has none | 3% | 91 |
| LinkedIn URL dead (profile gone or renamed) | 3% | 99 |

Of the 148 different titles, 36 differ only in wording (one holds the other, or punctuation), 29 are the company's name in our title, and 83 are another title.

## By file and by the profile's age

| Group | Same company and title | 95% CI | Count |
| --- | --- | --- | --- |
| In the 10M+ file | 88% | 85% to 90% | 585 of 665 |
| In the 50M+ file only | 87% | 86% to 89% | 2,043 of 2,335 |
| Updated 0 to 30 days before the snapshot | 75% | 71% to 79% | 299 of 399 |
| Updated 30 to 90 days before | 87% | 84% to 90% | 512 of 590 |
| Updated 90 to 180 days before | 92% | 91% to 94% | 1,761 of 1,906 |
| Updated 180+ days before | 53% | 44% to 63% | 56 of 105 |

The profiles drawn were updated 104 days before the snapshot on average (median 123); 105 of the 3,000 were updated 180 days or more before.

## Fields, on the 2,901 profiles LinkedIn still has

| Field | Same as LinkedIn | 95% CI | Count |
| --- | --- | --- | --- |
| First name | 97% | 96% to 98% | 2,816 of 2,901 |
| Last name | 95% | 94% to 96% | 2,757 of 2,901 |
| Headline | 92% | 91% to 93% | 2,662 of 2,901 |
| Still in the US | 100% | 100% to 100% | 2,901 of 2,901 |
| State, where LinkedIn names one | 100% | 100% to 100% | 2,532 of 2,536 |
| Current job's start month, same company | 94% | 93% to 95% | 1,455 of 1,552 |

## Emails: not judged

27% of the people drawn have an email, verified 26 days before the snapshot on average. LinkedIn doesn't show emails, so this benchmark doesn't judge them.

## How it was taken

- **Sample**: 3,000 people drawn at random from the 50M+ file's people. 665 of them are also in the 10M+ file.
- **Reference**: each person's LinkedIn profile, asked by LinkedIn URL on 2026-10-08 through a LinkedIn profile API that fetches the profile from LinkedIn again when its copy is stale. Its answers were 2 days old on average when asked (median 0); 91% had been fetched from LinkedIn within the week.
- **Same company**: our current company is LinkedIn's current company.
- **Same title**: the two titles are equal once normalized (case, punctuation, accents, the spacing around & and /).
- **95% CI**: the 95% confidence interval of each share.
- No person is named here: only counts.

As CSV: [results.csv](results.csv).
