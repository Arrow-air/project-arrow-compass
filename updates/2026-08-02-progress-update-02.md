# Arrow Compass: Progress Update #2

**Period 1, weeks 3 to 4 (20 July to 2 August 2026).** Posted by Sleety, Compass Keeper

Second biweekly update, and this one closes Period 1. Same deal as last time: what moved, what didn't.

## What moved

**Second session held, 31 July.** A working session rather than a decision one. Erick and I went through a room of candidate bounties drawn from the two push goals and voted each one ship, shape or bin. Most came out contested, which is fair, since they were suggestions rather than scoped work. Thomas gave apologies (heads-down on Hevelina) and his verdicts are still outstanding, so treat the card set as reviewed by two people rather than settled by the group.

**Two things got decided.**

- **DAO bounties are funded from the GBC wallet.** Erick's call. The wallet already holds a USDC bucket earmarked for grants and bounties that has never been drawn down. Project bounties keep coming from project budgets.
- **Interim rule on who can post a bounty.** Project leads write bounties inside their own project. Anyone else with an idea hands it to me and I scope and post it. Erick backed this while naming its limit out loud: it stops working the moment people start submitting in volume. Good enough for now, needs replacing before it breaks.

**The first bounty batch is drafted.** Four cards, two against each push goal, mapped onto the real issue-form fields:

| Card | Push goal | Lvl | Hrs | ARROW |
| --- | --- | --- | ---: | ---: |
| **P1** Onboarding audit | Contributor pipeline | L4 | 6 | 1,920 |
| **P7** Live event calendar | Contributor pipeline | L4 | 5 | 1,600 |
| **A9** AIP-009 accelerator | Manufacturing AIP | L3 | 6 | 1,440 |
| **D9** Purchase flow design | Manufacturing AIP | L5 | 6 | 2,250 |
| | | | | **7,210** |

Rates are straight off AIP-004, with the AIP-010 section 6 token conversion, so every figure decomposes to `hours x rate x 5`.

Four clears the minimum of 4 this period commits to. I floated eight on the call as a stretch and I'd still like to get there, since the board isn't capped at four, and more go up through Period 2 as they're scoped.

Two of them are a new card type I want to try, which I've been calling an **accelerator**: a bounty that pays someone to move a decision the DAO has already agreed to make but hasn't had the room to make. Convene the people who can decide, chair it, publish what they decided and who owns the rest. Compass picks which rock to move; an accelerator gets behind one and pushes. A9 is the first, and it targets the manufacturer bonding side of AIP-009, which hasn't been picked up while the commerce side has moved well.

**The bounty board pipeline was broken, and is now fixed.** Worth reporting because it explains a lot. The sync workflow was missing an `issues: read` permission, so it returned an empty list instead of erroring, and every run went green while publishing nothing. That's why the board sat empty from May through July. It also couldn't commit to the base branch and was being rejected outright. Both fixed; the job now opens a PR for a human to merge, which also puts a reviewer between a form submission and a live reward.

## What didn't move

**Thomas's verdicts on the card set never came in**, so any claim that the batch is group-reviewed would be false. His input carries into Period 2.

**Two questions were raised and parked**, both deliberately:

- A monthly ceiling on DAO bounty spend. Around $3,000/month was floated against the existing pot. I was thinking out loud and it should not be treated as agreed.
- Who may post bounties long term. Erick raised token-gating; I floated a slashable bond of roughly 20% of the reward as a spam deterrent, then immediately talked myself out of it, since it punishes anyone whose circumstances change mid-bounty. Both need a proper decision, not a corridor one.

**The standing Compass doc still hasn't landed.** Update #1 said it would ship as a docs PR that week and it didn't, so there is still no public page anyone can check the quarter's priorities against. The draft exists; getting it merged is a Period 2 item rather than a done one.

## The thing nobody planned for: agents are claiming bounties

Carrying this as its own item because it changes an assumption the board was designed under.

I posted a test bounty purely to check the issue-to-board pipeline. A bot claimed it within hours and submitted a substantial, confident, worthless solution. By the next morning there were four such pull requests.

The question that falls out of it is real and I don't have an answer yet: **what size and shape of bounty keeps agents away while still being worth a human's time?** Work I'd have posted as a multi-day bounty a year ago is something my own tooling now does in an afternoon. The bar for what belongs on the board has moved, and this isn't a hypothetical to schedule for later. It's happening on the live repo now.

If anyone has seen another DAO handle this well, I want to hear about it.

## Accountability snapshot: Period 1 (6 July to 2 August)

| Criterion | Committed | Delivered |
| --- | --- | --- |
| Snapshot vote held + priorities published | done | Passed 11 Jul, priorities ranked and published 17 Jul. See the note in the [Period 1 table](https://github.com/Arrow-air/project-arrow-compass/blob/main/accountability/README.md) on the mechanism |
| Meetings held | 2 | 2 of 2 (17 Jul, 31 Jul) |
| Progress updates posted | 2 | 2 of 2 (this one) |
| Bounties created / assigned | >= 4 | 4 of 4 filed and published: [#214](https://github.com/Arrow-air/website/issues/214), [#215](https://github.com/Arrow-air/website/issues/215), [#216](https://github.com/Arrow-air/website/issues/216), [#217](https://github.com/Arrow-air/website/issues/217) |

The bounty line turns on the issues actually being filed rather than drafted, and all four went up on 2 August.

## The wider period: all three projects

This closes my first 28 days across Media, Docs and Compass, so the whole picture in one place. Detail stays in each project's accountability table rather than being repeated here.

**Media & Comms.** The posting floor cleared every week of the four. Replies cleared three of four, landing 14 of 15 in week 1. Weekly evidence: [wk 1](https://github.com/Arrow-air/project-social-comms/blob/main/accountability/period-1-wk1-evidence.md) / [wk 2](https://github.com/Arrow-air/project-social-comms/blob/main/accountability/period-1-wk2-evidence.md) / [wk 3](https://github.com/Arrow-air/project-social-comms/blob/main/accountability/period-1-wk3-evidence.md) / [wk 4](https://github.com/Arrow-air/project-social-comms/blob/main/accountability/period-1-wk4-evidence.md)

**Docs.** Eleven PRs merged: the disciplines taxonomy end to end (bounty pipeline, board filters, contributor map), a mega menu and mobile quicklinks drawer, the bounty form cut to five required fields, the board stacked into cards on mobile, and the docs rewritten to match the new bounty flow. [Period 1 table](https://github.com/Arrow-air/project-docs-improvements/blob/main/accountability/README.md)

**Compass.** Q3 priorities voted and published, two sessions held, two updates posted, 4 of 4 bounties filed and published. [Period 1 table](https://github.com/Arrow-air/project-arrow-compass/blob/main/accountability/README.md)

Every committed line met across the period, with one exception: week 1 replies came in at 14 of 15.

## Period 2

1. Get the four onto the public board. They are filed and labelled, and the sync now returns them, but the generated data lands as a bot commit that the branch rules reject as unsigned, so the board is still empty until that is fixed
2. Thomas's pass over the card set, and the bounties he said he'd bring
3. Settle the monthly ceiling and the posting rules properly, rather than parking them again
4. Run A9. The AIP-009 session it pays for is the biggest single unlock available this quarter
5. Sessions 3 and 4, updates 3 and 4

## Want in?

The four are up and open to anyone. P1 in particular wants someone **new to Arrow but not new to communities**, because the whole value is a fresh account walking in from every direction and reporting where the path loses people, and that's the one thing none of us can do any more.

And the standing ask from the last session still holds: if there's something you think genuinely needs doing that you can't get to yourself, tell me. That's what the board is for.
