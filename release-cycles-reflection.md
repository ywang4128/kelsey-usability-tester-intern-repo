# Understanding Release Cycles & Version Control

## What are the typical stages in a software release cycle (development, testing, staging, production)?
planning - build - testing - deployment prep - production - post-release

## How does QA work differ between a feature release and a hotfix?
Feature release: has large changes, QA test it with comprehensive suite at scheduled timing.
Hotfix: has small critical fix, QA test it with more targeted and focus on core flows during UAT smoke test or when it's urgent.

## What is version control (Git), and how does it impact testing?
version control is using Git to track code over time via commits in a repo.
It helps QA see diffs and commits for change scope and help us to clone latest code for testing.

## What are Git branches, and why do testers need to be aware of them?
branches are parallel code versions.
testers watch them to test specific features on branch, avoid mixing changes, and trace bugs to exact code versions.

## How does QA handle rollbacks if a release causes major issues?
1.detect via monitoring or user reports  
2.tag builds, store artifacts  
3.re-deploy previous version  
4.post-mortem  

## How would you adjust your testing strategy for a major feature release vs. a small bug fix?
major release: full regression + non-functional
bug fix: targeted repo + smoke test

## If a developer says, “This bug only happens on an older branch,” how would you handle it?
switch to that branch, repro, and report with steps and version

## Why is it important for testers to know which version of the app they are testing?
match exact code and deploy
prevents " works on my machine" mismatches
