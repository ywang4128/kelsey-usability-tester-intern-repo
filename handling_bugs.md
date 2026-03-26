# Handling Hard-to-Reproduce Bugs #35

## What are common causes of intermittent bugs in software?
flaky bugs often come from:
- race conditions: when two or more actions interfere because of timing
- network or server instability: slow or dropped connections, timeouts, or third-party service failures
- environment differences: different OS, device, memory, oe battery levels
- resource issue: low memory, high CPU, or full storage
- Uninitialized or cached data: reading old or missing values that only show up under certain conditions

## What tools can help capture debug logs, network requests, and app crashes?
QA can use Android Studio Logcat or Xcode Console, Browser DevTools, Cloud-testing tools, and Crash-reporting services.

## What strategies can testers use to make flaky bugs more reproducible?
testers can re-run the exact same steps many times to see if the failure appears more often, vary one thing at a time, add more logging around the area where the bug is suspected , and use stress or bulk-data tests to trigger resource-related failures.

## How do teams handle "Cannot Reproduce" issues?
Teams usually keep the bug open but mark it clearly, add labels or tags so they can filter and review these bugs periodically, or occasionally ship a defensive change or extra logging if the bug is serious and multiple users report it.

## How would you report a bug that only happens occasionally?
I would write a clear title with "intermittent" or "occasional" in it and also describe as much as detail as possible and how often it seems to happen, and if there's any logs or screenshots captured during the failure.

## If a developer marks a bug as "Not reproducible", what’s your next step?
I would re-check the environment and steps to make sure nothing missed, ask for their exact steps, and attach any logs, recording, or notes showing the bug appeared at least once.

## What tools or techniques can help capture extra details for unpredictable bugs?
Tools like crash-reporting or error-tracking tools, screen recordings or session-replay tools, or repeating the test many times in a script to see if the bug appears more frequently under stress.
