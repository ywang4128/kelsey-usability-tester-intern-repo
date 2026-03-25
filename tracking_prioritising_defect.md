# Tracking and Prioritising Defects
## What is the difference between bug severity and bug priority?
bug severity is about how broken the feature is technically. High severity like the bug breaks core functioanality, low severity like a small glitch or cosmetic issue.
bug priority is about how quickly the team should fix it. Hogh priority like the bug must be fixed soon, low priority like it can wait or be scheduled for later.

## How do teams decide which bugs to fix first? (Business impact, risk, effort, etc.)
bugs are usually triaged using factor like business impact, risk, or effort and timing.

## What tools can QA use to track defects in an Agile workflow?
tools such as Jira, Azure DevOp to track bugs as "issues" linked to sprints, Github issues, and Test Rail to link test cases and defects.

## What happens when QA, developers, and product teams disagree on priority?
disagreement usually get resolved in a meeting, each role brings their perspective to the meeting:
QA emphasizes user impact and risk , Developers explain effort and technical risk, and product focuses on business value and release goals. Through discussion, the group agrees on a final priority. If still have disagreement , the Product Owner or scrum teamlead often has the final say.

## How would you prioritise a cosmetic UI issue vs. a login failure?
For Focus Bear, I would treat a login failure as high priority and high severity because users cannot use the app at all, which directly affects trust and retention. A cosmetic UI issue would be lower priority unless it clearly confuses users or break accessibility.

## If a developer says a bug is too minor to fix, how would you respond?
I'd explain the user-impact angle and ask questions like "how many users are likely to see this behavior?", "Could this confuse someone with ADHD or Autism who relies on consistent UI?". 

## How can testers ensure that low-priority bugs don’t get forgotten?
To keep low-priority bugs visible, I log them in the tracker with clear severity, priority, and short note about impact, and suggest a regular bug-triage session where the team quickly reviews old or low-priority issues and decides which ones to finally fix, close, or keep.
