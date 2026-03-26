# Exploratory Testing vs. Regression Testing #37

## What is exploratory testing, and how does it differ from scripted testing?
exploratory testing means testing the app freely, combining learning, test design, and execution in real time. You ask questions instead of following a strict script, try unusal paths, and change your approsch as you learn.  
Scripted testing follows pre-defined steps and expected results. So, exploratory testing is about discovering unknown issues, while scripted testing is about cerifying known behavior.

## What is regression testing, and why is it important in software development?
refgression testing checks that existing features still work after new changes or bug fixes. It's important because it prevents developers from accidentally breaking something that used to work, helps catch hidden side effects of small changes, and builds confidence in releasing new features safely.

## When should exploratory testing be used instead of regression testing (or vice versa)?
use exploratory testing when a failure is new or unstable, after scripted tests to chase hunches and edge cases, and when we want to see if the app behaves realistically under messy, user-like inputs.

## How can exploratory testing reveal bugs that scripted tests might miss?
because exploratory testing lets us try unusual timing, inputs, and interruptions, while scripted test only follow a narrow, expected path.

## Why is exploratory testing particularly useful for an app like Focus Bear?
because it helps discover usability and distraction-related issues that a typical expected path wouldn't cover, and uncover timing and interaction bugs that mirror real-world focus-and -distraction patterns.
For example, while a scripted test might only check that a session can start and end normally, exploratory testing can reveal that the app becomes overwhelming or confusing if a user toggles many distractions quickly or restarts sessions in rapid succession.

## What risks come with relying too much on exploratory testing vs. only doing regression testing?
Too much exploratory testing without regression risks missing regression bugs, because the same checks are not repeated in a consistent way; core features can quietly break between releases.

Only regression testing risks missing subtle, non‑linear, or user‑like issues, since scripts rarely try “weird” combinations of actions or edge‑case timing.

## How would you document and report issues found during an exploratory testing session?
I would Keep a test charter or mission, take quick notes: what I did, what I saw, and what surprised me.

For each bug, turn those notes into a proper bug report with:
1.A clear title and severity.
2.Steps to reproduce (as close as possible).
3.Environment, screenshots, and logs if available.
