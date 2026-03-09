---
name: content:today
description: Daily content briefing — what you need to do today
argument-hint: "<workspace-name>"
---
<objective>
Daily content operations briefing. Shows what needs attention right now.

Workspace: $ARGUMENTS
</objective>

<execution_context>
@./.claude/contentos/references/defaults.md
</execution_context>

<process>
1. Display: `<< CONTENT:OS // TODAY >>`
2. Load workspace context — CALENDAR.md, CHANNELS.md, BRAND.md, METRICS.md, LEARNINGS.md
3. Load content calendar for today and this week

## Publishing schedule
4. Show content due today:
   - Blog posts scheduled for publish
   - Social posts queued
   - Newsletter drafts due
   - Content in review/approval pipeline

## Content pipeline
5. Show pipeline status:
   - Briefs waiting for writing
   - Drafts in progress
   - Content in review
   - Approved and ready to publish
   - Overdue items (flagged)

## Performance pulse
6. Show key metrics from last 24-48 hours:
   - Top performing content (engagement, traffic, shares)
   - Underperforming content (flag if below benchmarks)
   - SEO movement (ranking changes, new keywords)
   - Social engagement rate

## Engagement
7. Show pending engagement:
   - Comments needing replies
   - Community posts needing response
   - Competitor content worth noting

## This week ahead
8. Show upcoming deadlines this week
9. Flag any gaps in content calendar

## Actions
10. Suggest top 3 actions for today based on urgency:
    - Overdue items first
    - Publishing deadlines
    - Engagement opportunities

11. Display:
```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  Quick actions:
  >> /content:write — draft content
  >> /content:publish — publish ready content
  >> /content:social — create social posts
  >> /content:calendar — manage content calendar

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```
</process>
