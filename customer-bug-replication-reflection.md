# Replicating Bugs Reported by Customers #28

## What steps should QA take when a customer reports a bug that can’t be easily reproduced?
1.acknoledge
log the bug in the tracker, mark it as "cannot reproduce yet" and note all known details.
2.gather missing details, ask support for environment, account type, exact steps, and whether it happened once or repeatedly
3.try to narrow it down by vary inputs, network conditions, and timing. or try the same flow on different devices or user profile.
4.involve dev team, share evidence and ask them to review likely code paths.
5.decide on next actions, keep the bug open with a clear status.

## What information should QA request from customer support to help diagnose an issue?
QA should ask customer support what the user was doing, when it happened, environment, screenshots, screen recordings, or error messages taken by user.

## How can logs, screenshots, and error messages help with bug reproduction?
logs show what the app and server were doing under the hood, including errors, API calls, and timing.  
screenshots and recordings help QA see exactly what the user saw.  
visible error messages give clues about what failed.

## When should QA recommend adding more logging to capture hard-to-reproduce issues?
QA should recommend adding more logging when the bug is intermittent and hard to catch in testing, existing logs are too vague or missing important context, or the bug only happens for small set of users and there's no clear pattern yet.

## How do other teams handle "Cannot Reproduce" customer bugs effectively?
many teams handle this by keeping these bugs open but tagging them clearly, using centralized logging or monitoring tools to watch for similar error patterns across many users, running targeted tests on the same environment or user profile when the bug is reported again.

## If a customer reports a crash but you can’t reproduce it, what are your next steps?
1.document everything from support
2.try to match the environment exactly
3.ask the user to send a screen recording and crash logs from the device
4.work with developers to review logs around the crash and check for error spikes in anaytics
5.if it's rare but serious, recommend adding more logging aroumd the suspected area and then monitor foe similar reports.

## When should you ask developers to add more logging, and what kind of logs would help?
I would ask for more logging when the bug is critical or painful for users but rarely reproducible or existing logs only say "error" without context. For focus bear, useful logs might include timestamps amd inputs when saving a routine or error messages when enabling or disabling distraction-blocking

## What are some common patterns in bugs that only occur for some users but not others?
some typical patterns for these bugs are environment-specific issues, data-dependent bugs, network-related behaviors, and race conditions or timing issues.
