# How to Test Accessibility #32
## What is WCAG (Web Content Accessibility Guidelines), and what are its key principles?
Web Content Accessibility Guidelines is the international standard for making digital content usable for people with disabilities. There are four principles, often called POUR:  
- Perceivable - users must be able to perceive content.
- Operatable - user must be able to operate the interface.
- Understandable - content and navigation should be clear and consistent.
- Robust - content should work well with current and future assistive technologies

## How do screen readers (e.g., NVDA, VoiceOver, TalkBack) work, and how can QA test with them?
Screen readers are tools that read out screen content for blind or low-vision users.  
As QA, I can 
- turn on the screen reader and try to use the app without seeing the screen, relying only on headings, labels, and announced states.
- check that buttons and links have clear , meaningful names
- ensure the reading order matches the visual layout so users don't get confused.

## What are some common accessibility issues in apps and websites?
- missing or unclear alternative text on icons and images
- poor color contrast
- non-keyboard-accessible controls
- missing or wrong focus indicators
- confusing or inconsistent navigation

## How can you test keyboard navigation and focus management?
use tab and shift+tab to move through elements, making sure every interactive control can be reached, watch for visible focus indicators so users know where they are, and check that the tab order follows a logical flow.

## What tools can help automate basic accessibility checks?
1.Browser accessibility inspectors that flag contrast, missing labels, and keyboard issues.
2.extensions like axe DevTools or WAVE
3.mobile tool that test contrast, touch-target size, and focus order for apps

## How would you test if Focus Bear is usable with a screen reader?
I would use VoiceOver on Ios or Talkback on Android while navigating the app as a first-time user. Check that all buttons and options have clear labels, headings and sections make sense, and error messages and confirmations are read out clearly.

## What accessibility barriers could affect someone with ADHD or Autism using the app?
for users with ADHD or autism, common barriers include:
- overly busy or cluttered UIs with too many options or flashing effects that distract or overwhelm.
- unclear, inconsistent instructions or labels that make it hard to know what to do next.
- sudden change or unexpected sounds that cause anxiety or lost focus.
- lack of structure or feedback

## If a developer says "this doesn't impact most users", how would you advocate for fixing an accessibility issue?
I would explain that accessibility is a legal and ethical requirement, not just "nice to have", and matters for users with ADHD, autism, low vision, or motor disabilitiess. Also show concrete examples and highlight that acessibility improvements often help everyone.
