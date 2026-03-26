# Understanding Logs & Debugging Tools for QA #31

## What are logs, and how do they help with debugging?
logs are messages written by the app and server that record what happened, like "request sent", "user logged in". They help QA and developers to see steps the app took behind the scenes, spot crashes, failed API calls, or odd behavior that isn't obvious in the UI, and reproduce issues by matching patterns in the log with steps taken.

## How can you capture logs from a web app (browser DevTools)?
open DevTools -> in the console tab can see JavaScript errors and log messages -> in the Network tab can see all API calls, and can even save the activity as a HAR file.

## How can you capture logs from a mobile app (Android/iOS debugging tools)?
on IOS: use Xcode's Console or tools loke iTools to view device logs while running the app
on Android: enable Developer Options and use Logcat to see app-specific logs, including crashes and errors.

## What are some common error messages and log patterns testers should recognize?
4xx HTTP status codes(e.g. 400,401,403,404): usually client or auth-related issues.
5xx status code(e.g. 500,502,503): server-side problems
Lines containing error, exception, crash, timeout, or failed to... in logs
duplicate or repeated errors right before the app freezes or closes

## How do network requests in browser DevTools help diagnose API failures?
in the Network tab can see every API call the app makes, can also see status code, response bodies , and headers reveal what went wrong. We can filter by type and inspect the exact request parameters and timing.

## If Focus Bear crashes on a user’s device but not on yours, how would you use logs to investigate?
in this case, I would ask the user to send a device log or crash report, compare the log with my own test device to look for differences, or look for lines containing FATAL EXCEPTION, Crash, or unhandled error and note the stack trace and timestamp.  
If I can't get logs fromm the user right away, I'd at least reproduce a similar senario and capture logs during that test to see if the same pattern appears.

## What are some useful log messages that should be included when reporting a bug?
It should include a short snippet of the relevant log section, the HTTP status code and URL of the failing API call, any user-visible error message shown in the app, and the timestamp and environment.

## If an API call returns an unexpected response, what steps would you take to analyze the issue?
open DevTools -> Network tab and find that request, check status code, response body, and request headers and playload.
-> try to replay the same request with valid data to see if the behavior changes. -> document the exact request and response and share it with the developer, asking whether the API should accept this input or if it needs clearer validation.
