# Understanding Deployment & Hotfix Testing 
## What is the difference between a scheduled release, a rollback, and a hotfix?
scheduled release: a planned feature updates on a set schedule.
rollback: revert to previous stable version after issues
hotfix:urgent small patch for critical production bugs

## What should QA test immediately after a deployment?
QA should runs smoke tests: basic navigation, core flows, key changes, logs,etc.

## How does QA handle hotfix testing when a critical bug is found after release?
1.reproduce bug
2.verify fix and minimal critical suite in staging
3.post-deploy smoke on prod and state untested risks


## What strategies help prevent new bugs from being introduced in urgent fixes?
1.minimal changes only
2.fast critical regression suite
3.code review + rollback plan
4.feature flags

## How do other teams approach post-release monitoring?
Dachboards for errors, latency, metrics.

## If a release goes live and users immediately report issues, what should QA do?
1.Triage severity
2.check logs
3.escalte with repro
4.rollback if critical

## What’s the best way to prioritize testing when working under time pressure for a hotfix?
use risk-based testing and pre-defined priorities

## How can QA help ensure stability in production while still allowing fast bug fixes?
1.defined hotfix and rollback rules
2.always-green smoke suite
3.safty nets e.g.flags
4.post-mortems
