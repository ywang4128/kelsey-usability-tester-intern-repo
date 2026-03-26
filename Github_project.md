# Get familiar with GitHub Projects #40
## What are GitHub Projects, and how do they work?
GitHub Projects are customizable boards or tables that display and organize issues and pull requests (like a Kanban or roadmap). Teams typically use columns such as To Do, In Progress, and Done to show the status of each item. As developers and QA pick up work, issues are dragged between columns, so everyone can see what’s happening at a glance.

## How are issues created, assigned, and moved through different project columns (To Do, In Progress, Done)?
Creating an issue:
In a repository, click Issues → New issue, add a clear title, description, steps, and environment, then save.

Assigning:
Use the Assignees field to assign the issue to a developer or QA member.

Moving through columns:
In the associated GitHub Project board, drag the issue card from To Do → In Progress → Done as work progresses. Status changes are connected back to the underlying issue.

## What are labels, milestones, and assignees in GitHub issues?
Labels – tags like bug, enhancement, ui, priority‑high, qa, used to filter and group issues.

Milestones – time‑boxed targets that group issues planned for the same release.

Assignees – the person responsible for the issue, which keeps ownership clear and prevents tasks from being ignored.

## How can you use GitHub Projects to keep track of testing progress?
QA can:

- Create a separate QA / Testing project board or view inside the main project.
- Add issues for bugs, test ideas, and regression tasks.
- Use custom columns like “Needs Testing”, “In Test”, “Verified” to track whether a feature or bug fix has been checked.

Filter by labels such as bug, qa-review, or regression to see what’s pending.

## How would you create a new issue for a bug found during testing?
Click Issues → New issue in the correct repository.
Use a clear title.
Describe expected vs. actual behavior, steps to reproduce, environment, and attach screenshots or logs.
Add relevant labels and assign it to the appropriate developer or QA owner.
Link the issue to the current sprint milestone if the team uses milestones.

## How can you prioritise issues in a GitHub Project?
To prioritize issues:

Use labels (priority‑high, priority‑medium, priority‑low) and sort or filter by them.
Use Columns / Views or Tables to show issues by priority or status.
Discuss priorities in backlog or bug‑triage meetings and then rearrange cards or update labels accordingly.

## What are some advantages of using GitHub Projects for tracking QA tasks?
Using GitHub Projects for QA tasks helps:
Visualize QA progress (what is ready to test, what is in progress, what is verified).
Keep everything traceable – every bug or test task is linked to an issue, which can be connected to pull requests and code changes.
Improve transparency – developers and product owners can see what QA is working on and whether anything is blocked.
Align QA work with sprints by grouping tasks and bug fixes under the same milestone or project board.
