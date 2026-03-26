# Testing Performance & Responsiveness #36
## What are the key factors that impact app performance (CPU, memory, network, database queries, etc.)?
performance is usually affected by CPU usage, memory usage, network, database, API queries, and rendering and UI complexity.

## How can QA testers measure app speed and responsiveness?
QA usually checks app launch time, screen transitions, interactive delays, and resource usage.

## What tools can be used for basic performance testing (e.g., Chrome DevTools, Lighthouse, mobile profiling tools)?
tools like Chrome DevTools for web views or hybrid-style apps, Lighthouse gives a quick performance score and recommendations, Android Profiler for measuring CPU, memory, and network usage on mobile apps, and Mobile-focused tools for real-device performance data.

## What common performance issues appear in web apps vs. mobile apps?
Web apps often suffer from:
- large bundles or unoptimized JavaScript
- slow API calls and uncached data
- render-blocking resources or inefficient layout
mobile apps often have:
- long app-launch times or slow screen transitions
- memory leaks or clashes from too many background tasks
- poor battery or network handling

## How can QA test app behavior under high load or low resources (low RAM, slow CPU, unstable network)?
to test under stress or low-end conditions, QA can simulate slow CPU or network in Chrome DevTools, test on older devices with limited RAM and storage, or perform bulk actions to see if the app lags or crashes.

## How would you test Focus Bear’s performance on an older device or a slow internet connection?
I would put the phone in slow-network mode, test launch time, saving routine while offline, then sunc back online,  and watch for slow transitions, UI freezes, or crashes.

## If a user reports that the app feels slow, what steps would you take to investigate?
I would ask for details, like device, app version, network, and which screen or sction feels slow, and try to reproduce on the same device type or similar specs, use profiling tools to record app-launch time, screen-load times and UI responsiveness, CPU and memory usage, compare the measured metrics against reasonable targets, and create a bug or improvement report with clear data and screenshots.

## What performance optimizations could help Focus Bear run smoothly on low-end devices?
optimizations such as reducing heavy animations or unnecessary UI updates, compressing images and assets, or monitoring memory usage and fixing leaks so the app doesn't crash on low-RAM phones.
