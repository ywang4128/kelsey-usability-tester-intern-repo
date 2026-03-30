# Understanding how to do manual QA #48

## What is manual QA testing, and how does it differ from automated testing?
Manual testing uncovers usability issues through exploration, while automated handles repetition.
| Aspect     | Manual Testing                               | Automated Testing                          |
| ---------- | -------------------------------------------- | ------------------------------------------ |
| Approach   | Human-led, intuitive for edge cases testrail | Scripted scripts for regression testrail+1 |
| Strengths  | Usability, exploratory insights testrail     | Speed, volume, no fatigue geeksforgeeks    |
| Weaknesses | Time-intensive, error-prone geeksforgeeks    | Misses visual/UX bugs testrail             |

usually use manual for new features; automate stable ones.

## What is context-driven testing, and how does it challenge traditional QA approaches?
Context-driven testing is a mindset and approach to software testing that emphasizes adapting practices to the specific context of each project, rather than following rigid, universal "best practices." 

Traditional QA often relies on exhaustive checklists, standardized processes, and metrics like code coverage, assuming one-size-fits-all methods ensure quality.

## What are the seven principles of context-driven testing?
7 principles are:
- Value depends on context.
- Good practices exist, not universal "best."
- Humans central.
- Projects unpredictable.
- Product solves problems.
- Testing intellectual challenge.
- Judgment + skill + cooperation key.

## How do exploratory testing and scripted testing differ, and when should each be used?
Exploratory designs or executes tests simultaneously for discovery
scripted pre-plans steps for consistency.

## What skills make a great manual tester, according to James Bach and other experts?
great tester usually has folloeing skills:
Critical thinking, rapid learning, communication, oracles, self-management.
Great testers question assumptions, collaborate, distinguish testing (human) from checking (machine).

## Why is context important in testing, and how might testing Focus Bear differ from testing another app?
Context shapes risks.
Focus Bear testing prioritizes ADHD distractions

## How can manual testing be both structured and adaptable at the same time?
Manual testing balances structure and adaptability through frameworks like session charters and risk analysis, allowing guided exploration that pivots based on findings. 

## How would you approach testing a new feature in Focus Bear without a predefined test script?
I would start with reviewing app context (neurodivergent users), map user journeys, explore edge cases like offline mode, and record sessions, log heuristics, collaborate via GitHub issues with videos/steps.
Also debriefing risks priority and fixes suggestions in the report.

## How do you decide what to test when no detailed requirements are provided?
I would do the risk assessment, identifying risks via project context: Talk to devs, users, or product owners about goals (e.g., Focus Bear's distraction blocking for neurodivergent users). Prioritize what breaks focus or loses data over cosmetics.
