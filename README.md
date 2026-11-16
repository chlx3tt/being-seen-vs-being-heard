# Employee Communications Analytics — Fall 2026 Briefing

**Video briefing:** [PASTE UNLISTED YOUTUBE LINK HERE]

Analysis of Viva Engage post performance, September 1 – November 30, 2026
(42 posts), prepared for the CIBC Data Analyst, Employee Communications
Platforms exercise. The data is fictional and was provided with the exercise.

## Headline findings

1. **Announcements buy reach, not engagement.** Announcement posts (which push
   a notification to every member) reached a median of ~66% of their target
   audience, vs ~23% for standard posts. But per viewer, standard posts earned
   about twice the engagement (median 6.4% vs 3.0% of viewers reacting,
   commenting or sharing). Being pushed to open a post is not the same as
   choosing to engage with it.
2. **On the fall's most action-critical campaign, reach and action came
   apart.** The benefits enrolment announcement (Oct 13) was the most-viewed
   post of the fall — 12,780 unique viewers, 71% reach — but produced only
   178 enrolment-link clicks (1.4% of viewers, the lowest click rate of any
   announcement; the others ranged 5–9%). The standard-post reminder on
   Oct 28 reached only 19% of employees but drew 314 clicks (9.2% of
   viewers) — nearly double the clicks from a quarter of the audience.
3. **Conversation and people drive real engagement.** The town hall recap
   (a standard post) drew 312 comments — six times the next-highest post —
   a 15.5% engagement rate and 1.9 views per viewer (people came back to
   it). The CEO's Thanksgiving message and the CFO's Ask Me Anything were
   next for comments. Small, well-targeted community posts also reached
   56–74% of their audiences with no push at all.

**Recommendation:** for campaigns where employees must act (enrol, train,
sign up), plan two announcement touches from the start — the launch and a
deadline reminder — and judge the campaign on click-through, not views.

**Before firm conclusions, I would want:** actual enrolment completions to
set against clicks (a click is not an enrolment; some employees may act
through other channels); a look at why the enrolment announcement converted
so poorly (link placement, wording, timing); and a breakdown of viewers by
team/location, because this export cannot show who is being missed.

## Data notes

- The export contained 43 rows; one post (C109, "Hybrid work guidelines
  refreshed," Sep 21) appeared twice as an exact duplicate and was counted
  once, giving the 42 posts the workbook describes.
- All other checks passed: day-of-week matches the calendar, link clicks are
  present exactly where a link existed, and no post reports more unique
  viewers than its target audience.
- Raw shape of the data: 8 announcements vs 34 standard posts; 32 posts went
  to all 18,000 employees and 10 to smaller communities (smallest: 380).
  Engagement totals were 8,107 reactions, 1,109 comments and 673 shares —
  mostly a tap, rarely a comment.
- Comparisons use rates (reach %, engagement per viewer, clicks per viewer),
  not raw counts, because audience sizes range from 380 to 18,000 and
  announcements are push-notified while standard posts are not.

## Files

- `analysis.py` — full analysis (Python / pandas); prints every table behind
  the findings and regenerates the charts.
- `findings.py` — the three briefing findings, one short block each, with the
  output noted in the comments.
- `charts.py` — the three charts as a standalone script; regenerates the PNGs
  in `charts/`.
- `Employee_Comms_Analytics_Exercise_Dataset.xlsx` — the dataset as provided.
- `charts/reach_by_post_type.png` — median reach, announcements vs standard.
- `charts/engagement_rate_by_type.png` — median engagement per viewer.
- `charts/benefits_enrolment.png` — enrolment announcement vs reminder:
  viewers and clicks.

## Tools

Analysis in Python (pandas, matplotlib), with an AI assistant used to help
run the analysis. Interpretation and presentation are my own.
