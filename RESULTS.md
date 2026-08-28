# GitHub achievements: what actually still works

GitHub does not publish the criteria for profile achievements, and most guides
online repeat advice that stopped being true. These are measurements, not claims
from a blog post. Every number below came from one real account (`@loris307`)
on 2026-08-28/29.

## The achievements that exist

| Achievement | Criteria | Tiers |
|---|---|---|
| Quickdraw | Close an issue or PR within 5 minutes of opening it | none |
| Pull Shark | Merged pull requests | 2 / 16 / 128 / 1024 |
| Pair Extraordinaire | Co-authored commits on merged pull requests | 1 / 10 / 24 / 48 |
| Galaxy Brain | Discussion replies accepted as the answer | 2 / 8 / 16 / 32 |
| YOLO | Merge a pull request with no review | none |
| Starstruck | Stars on a repository you created | 16 / 128 / 512 / 4096 |
| Public Sponsor | Sponsor someone through GitHub Sponsors | none |

`Heart On Your Sleeve` and `Open Sourcerer` appear in the badge assets but have
never been released. `Arctic Code Vault Contributor` and `Mars 2020 Contributor`
are historical and cannot be earned.

## Finding 1: pull requests merged in your own repositories do not count

This is the important one, because it invalidates essentially every
"get Pull Shark in 5 minutes" tutorial.

Measured on `@loris307`:

- 34 pull requests authored and merged by the account in `loris307/twohrs`,
  a public repository, all merged into the default branch, spread over
  14 distinct calendar days in March 2026.
- 6 more of the same shape in `loris307/AI_to_Anki` in July 2025.
- Pull Shark on the profile five months later: still tier `x2`, the base tier.
  Reaching bronze requires 16.

A second, independent signal from the same account:

- 26 of those pull requests were authored by the account, merged by the account,
  and had zero reviews — the exact definition of YOLO.
- The account has never been awarded YOLO.

Two different achievements, both eligible many times over across 13 months,
neither granted. The repositories were public at the time: the Wayback Machine
has a 200 snapshot of `github.com/loris307/twohrs` from 2026-03-17.

### Hypotheses this rules out

- *"You need one merge per calendar day."* The account has merged pull requests
  on 18 distinct days. That is past the 16 threshold, and the badge is still `x2`.
- *"The repository has to be public."* It was, and it is archived as proof.
- *"It has to be the default branch."* Every one of them targeted `main`.
- *"It just takes 24 hours."* It has been five months.

## Finding 2: private repositories do not count either

The same account has roughly 25 merged pull requests in repositories owned by
*other* people — `cedric-len/link-up`, `gianlucahe/vacation.ai`,
`MoDeinBro24/Project-Battlerap` — going back to 2024. All private. None of them
moved the counter either.

So the requirement is the conjunction: **public, and not owned by you.**

## Finding 3: the profile only exposes the tier, not the count

The achievements tab renders `x2`, `x16`, `x128`. The hovercard endpoint
`/users/<user>/achievements/<name>/detail?hovercard=1` carries a `tier-count`
attribute, but it repeats the tier multiplier rather than the underlying total.
There is no public API for achievements at all — not REST, not GraphQL.

The practical consequence: between two tiers you are flying blind. You cannot
tell "counting, but not there yet" apart from "not counting at all", which is
exactly why the bad advice survives.

## Finding 4: co-author trailers are matched by email

`Co-authored-by:` is matched to an account by the email address. A trailer
pointing at an address with no GitHub account behind it renders as plain text
and credits nobody. The same account has 213 commits carrying
`Co-authored-by: Claude <noreply@anthropic.com>` and Pair Extraordinaire sitting
at tier 1.

Use the account's own no-reply form, which always resolves:

```
Co-authored-by: username <ID+username@users.noreply.github.com>
```

## Method

Everything here is reproducible. The scripts open a branch per note, one commit
per branch, then create and merge the pull request through the REST API, pacing
below the 80-per-minute secondary rate limit for content-creating requests.
The discussions are created, answered and marked through the GraphQL API.
