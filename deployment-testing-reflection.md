# Understanding Deployment & Hotfix Testing 
## What is the difference between a scheduled release, a rollback, and a hotfix?
scheduled release: a planned feature updates on a set schedule.
rollback: revert to previous stable version after issues
hotfix:urgent small patch for critical production bugs

## What should QA test immediately after a deployment?
Post-deployment smoke tests verify core functionality hasn't broken.   
For instance, I'd immediately test Focus Bear's login, routine creation, distraction blocking, and offline mode. This catches 80% of showstopper issues before users notice.

## How does QA handle hotfix testing when a critical bug is found after release?
1.reproduce bug - Record screen, note environment. This gives devs precise context.
2.verify fix and minimal critical suite in staging - Test ONLY the bug + 3-5 high-risk regressions.
3.post-deploy smoke on prod and state untested risks - Transparency builds dev trust when minor issues emerge later.


## What strategies help prevent new bugs from being introduced in urgent fixes?
1.minimal changes only - Fix ONLY the bug line + unit test. Smaller scope = fewer regressions.
2.fast critical regression suite - Pre-defined 15min suite (e.g. login, save, sync, block)
3.code review + rollback plan
4.feature flags

## How do other teams approach post-release monitoring?
They might use dashboards track errors, latency, + user metrics in real-time, alerting prevents surprises, and user feedback loops.

## If a release goes live and users immediately report issues, what should QA do?
1.Triage severity
2.check logs + reproduce 
3.escalte with repro
4.rollback if critical - Better short-term pain than long-term reputation damage.

## What’s the best way to prioritize testing when working under time pressure for a hotfix?
1.use risk-based testing and pre-defined priorities
for instance, P0: crashes/data loss/security; P1: core flows (login/save/sync); P2: everything else.
2.Impact × likelihood matrix guides decisions. High-impact/low-likelihood waits; high-impact/high-likelihood tests first.
3.Team alignment via shared doc prevents "test everything" panic. 

## How can QA help ensure stability in production while still allowing fast bug fixes?
1.defined hotfix and rollback rules
2.always-green smoke suite - e.g.10 critical tests run on every deploy
3.safty nets e.g.flags - Caught regression before full rollout
4.post-mortems after every incident - Even "successful" hotfixes get 15min review: "What broke? QA gap? Process fix?"
