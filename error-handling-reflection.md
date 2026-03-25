# Testing Error Handling & Edge Cases #23

## What is boundary value analysis, and why is it useful for testing?
Boundary value analysis means testing the edges of allowed values, like the smallest, largest, and " just outside" numbers.
This helps catch bugs where the app behaves differently at the limits. It's useful because many bugs hide at these boundaries instead of in the middle of the range.

## What are common edge cases that testers should check in forms, authentication, and app flows?
Common edge cases in forms, authentication, and app flows include empty or extremely long inputs, invalid data like typing letters into numeric field, and multiple failed login attempts, expired sessions, or using the app while logged out.

## How should QA test network failures, offline mode, and slow connections?
QA could simulate different network conditions to see how the product behaves in those scenarios:
- turning on airplane mode
- using slow orr spotty wifi or mobile data
- turing the network back on and checking if routines and distraction-blockingrules sync correctly

## What happens when an app encounters an unexpected input or invalid data?
If the app receives data it doesn't expect, it should not crash or hang, instead, it should reject the input gracefully, show a clear error message, amd keep the rest of the app working.

## How can error messages be tested to ensure they are helpful and user-friendly?
good error messages are clear, specific, and playful when appropriate. I'd test if the message is easy to read(simple language, no jargon), if tit suggests a next strp, and if the tone matches the app's friendly, guiding style.

## What edge cases could break Focus Bear’s onboarding flow?
possible edge cases in FocusBear's onboarding are user cancels onboarding halfway and then returns later, user skips multiple screens or goes back and forth repeatedly, user signs up and then immediately turns flight mode on.

## If the app fails midway through a critical action, how should it behave?
save what it can locally if possible, show a clear and calm message, and not lose the user's data or reset them to the begining of the flow.

## How would you test for network instability and ensure Focus Bear handles it gracefully?
To test network instability and take Focus Bear for example, I would use slow-network or throttling tools, start actions like creating a new routine or enabling distraction-blocking, then drop the connection, and check if app saves local changes, show an understandable status, sync correctly when the network returns without duplicating data.
