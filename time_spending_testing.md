# Deciding how long to spend on testing an issue #41
## What factors influence how long you should test an issue? (Complexity, risk, priority, deadlines)
Complexity – How many parts are involved? A simple text change takes minutes; a core login flow can take much longer.

Risk – How badly it can hurt users or the business.

Priority – Whether the bug is high‑priority for the release or can wait.

Deadlines – Time left in the sprint or before a release influences how much depth you can afford.

## What techniques can help prioritise testing efforts? (Risk-based testing, exploratory timeboxing)
Risk‑based testing – spend more time on high‑risk, high‑impact areas.

Timeboxing / exploratory sessions – set a fixed period to test a specific area or bug, then decide whether to expand or stop.

Checklists plus exploration – start with a short checklist of core flows, then explore edge cases if time allows.

## What is "good enough" testing, and how do you know when to stop?
Good enough”: already tested what matters most within the time and risk constraints:
- Key user flows related to the issue are working.
- Obvious edge cases and known risks have been checked.
- You’ve collected enough evidence to say whether the bug is still there or fixed.

You know it’s time to stop when:
- The bug can’t be reproduced after several reasonable attempts.
- Further testing is unlikely to reveal new high‑impact issues.
- The sprint or release deadline forces you to move on and accept the remaining risk.

## How do experienced QA testers balance depth vs. speed in real-world projects?
Experienced testers balance depth and speed by:
- Defining a “minimum test set” – a small, quick set of tests that at least verifies the core behavior.
- Layering tests – running light checks first, then diving deeper if time and risk justify it.
- Communicating risk – telling the team, “We’ve only had time for basic checks; here’s what’s still a risk.”

## How would you approach testing a small UI bug vs. a critical login issue?
Small UI bug:
- Spend a few minutes checking the visible layout, zoom levels, and different devices.
- Verify that the rest of the screen behaves as expected and no other elements are broken.
- Stop once it looks correct and no new issues appear.

Critical login issue:
- Testing all login paths.
- Checking error messages and logs.
- Trying different network conditions and device types.


## If you had limited time, how would you decide what to test first?
With limited time, I would:
- Sort by risk and priority – test blocking or high‑impact bugs first.
- Cover core user flows – make sure the main path works before polishing edge cases.
- Skip low‑impact, low‑risk items.

## What risks come with over-testing or under-testing an issue?
Over‑testing risks:
- Wasting time on low‑impact areas while higher‑risk bugs are ignored.
- Delaying releases unnecessarily.

Under‑testing risks:
- Letting important bugs slip to production.
- Missing edge cases that upset real users.


