# How to Write Effective GitHub Issues #27

## What are the key components of a good GitHub issue?
It usually includes a clear, descriptive title, a description explaining what happens, what should happen, and why it matters, steps to reproduce, environment details, screenshots, logs, or a short screen recording, and appropriate labels.

## What is the difference between a bug report, feature request, and technical task?
bug report: the software does something wrong compared to its expected behavior.
feature request: a new capability the app should have that it doesn't promise yet.
technical task: an internal engineering task that doesn't appear as a user-facing feature.

## How do labels, milestones, and assignees help organize issues in GitHub Projects?
labels: like tags so the team can filter and group issues by type, area, or urgency.
milestones: it links issues to a specific release or sprint, so the team can see what's planned for specific version or topic.
assignees: this show who is responsible for working on the issue, which keeps ownership clear and reduces confusion.

## What are some examples of well-written vs. poorly written GitHub issues?
well-written issue is short but complete, focused on one problem, and uses clear language. For example:  
"Bug: App crashes when tapping 'Save' after creating a distraction-blocking rule with 15+ apps." and wih steps of reproduce, environment and screenshots attached.
poor written issue is vague or too broad, for example:  
"The app is broken on the routine screen" with no steps, no screenshots, and no environment info.

## How would you write a bug report for a crash in Focus Bear?
Title:
[Bug] App crashes when enablng distraction-blocking on IOS 17
Description:
when a user turns on distraction-blocking for more than 10 apps, the app crashes instead of showing the confirmation screen. 
Expected behavior - the app should have the settings and return to the routine screen without crashing.
Steps to reproduce:
1.open Focus Bear on an iphone with IOS 17
2.go setting blocking apps section and select 15 apps
3.go to "start focus session" and press start
4.observe the app crash
Environment: IOS 17.4/device-iphone 15/app version- 1.3.5
Attachments: screenshot of the step-before crash and a short screen recording and any crash logs
Severity: User cannot use the distraction-blocking safely, which affects Focus Bear's core promise

## How can adding steps to reproduce help developers fix issues faster?
It helps the developers see the same problem in the same way. Without it, dev team has to guess what might happened, which waste time and can lead to the issue being "not reproducible" and closed.

## If a developer asks for more details on an issue you created, what might you have missed?
I might have missed:
- exact environment
- full steps to reproduce
- expected vs. actual behavior described clearly
- screenshots, logs, or a video of the failure

