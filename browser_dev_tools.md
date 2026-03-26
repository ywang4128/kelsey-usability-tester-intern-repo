# Learn how to use browser developer tools #39
## What are the main features of browser developer tools in Chrome and Firefox?
main features of browser developer tools in Chrome and Firefox include:
Elements / Inspector – view and tweak the HTML and CSS live.
Console – see JavaScript errors and warnings, plus run quick JS commands.
Network – inspect all API requests, responses, and timings.
Sources – debug JavaScript.
Performance / Memory / Application tabs – monitor speed, memory, and local‑storage data.

## How can you check for JavaScript errors in the console?
Open DevTools -> Go to the Console tab. -> Look for red lines (errors) or yellow lines (warnings).

## How do you use the Network tab to monitor API requests?
To inspect API calls:

1.Open DevTools → Network tab and make sure the record button is on.
2.Interact with the app to trigger API calls.
3.Filter by type (XHR or Fetch) to see requests.
4.Click an entry to view:
5.Status code (e.g., 200, 400, 500).
6.Request body, headers, and response body.

## How can you simulate different network conditions (e.g., slow connections) to test performance?
Most browsers let us simulate slow or unstable networks:

In Chrome DevTools, open the Network tab and use the Online / Slow 3G / Fast 3G / Offline presets.

In Firefox, similar tools are available under Network or via add‑ons.

## How would you use DevTools to confirm if an API call is successful or failing?
1.Go to the Network tab and locate the relevant request.
2.Check the status code and response body:
200–299 = usually success.
4xx = usually client‑side issue (e.g., invalid data).
5xx = usually server‑side issue.

If it fails, capture the request/response and share it with the developer, including headers, payload, and the error message.

## How can DevTools help you debug a UI issue that only happens in one browser?
If a UI bug only appears in one browser:

- Use Elements / Inspector to see if styles differ or elements are missing.
- Check the Console for any JavaScript errors or warnings in that browser.
- Compare computed styles, rendered layout, and DOM between Chrome and Firefox to spot differences.

## When reporting a frontend bug, what information from DevTools would be most useful for a developer?
For a frontend bug, information usually include:
- Console error messages.
- Network tab info for the failing API call.
- Elements / Inspector details.
- Steps + screenshots plus a brief note about browser/version and device size.
