# How Manual QA Fits into the Overall Testing Approach vs. Automated QA #38
## What are the key differences between manual and automated testing?
Key differences between manual and automated testing is manual testing is better for thinking, judging, and exploring; automation is better for repeating and scaling known checks.

## What types of testing are best suited for manual QA vs. automation?
Manual QA is best for: Exploratory testing, Usability and accessibility checks, and ad‑hoc and one‑off tests, new‑feature first‑time checks.

Automation is best for: Regression testing, smoke and sanity tests before release, performance, load, and cross‑browser or device checks.

## Why do some teams focus too much on automation and neglect manual testing?
Teams sometimes over‑automate because they chase efficiency and continuous‑delivery speed, think “all tests should be automated” and underestimate how much discovery and intuition matter, and ignore usability, edge cases, and real‑user behavior because scripts can’t easily capture them.

## How do manual testers collaborate with automation engineers in an Agile team?
They work together by sharing test ideas, helping refine senarios, running exploratory sessions and then handing over break often paths to the automation engineer, and reviewing automated tests to make sure they actually reflect real‑world usage and not just happy‑path expectations.

## If Focus Bear had 100% test automation, why would manual QA still be needed?
Even with 100% automation, manual QA would still be needed because:
- Automation can’t fully judge usability or comfort, especially for users with ADHD or autism.
- Users interact with Focus Bear in messy, unpredictable ways that scripts are unlikely to cover.
- New design, wording, or flow changes still need a human to check whether they feel calming, clear, and easy to use.

Automation would protect the basics, but manual QA would guard the user experience and edge‑case behavior.

## What are some limitations of automated testing that manual testing can cover?
Common limitations of automation include:

Inability to see subtle UX or accessibility issues.
Only testing what’s scripted—so new or unexpected bugs stay hidden.
Struggling with dynamic UIs, timing, and visual changes without constant maintenance.

Manual testing can:
Spot confusing flows or patterns that “feel wrong” but still pass the script.
Try combinations of actions and interruptions that no one anticipated.
Give feedback on how the app feels to use, not just whether it technically works.

## How can manual testers help improve automated test coverage over time?
Manual testers can enhance automation by:

Logging patterns: tracking which bugs keep appearing in the same area and suggesting that path be automated.
Turning exploratory findings into test cases.
Reviewing automation scripts to make sure they test realistic, user‑like scenarios, not just happy paths.
Maintaining a “risk list” of high‑impact areas where automation coverage is still weak.
