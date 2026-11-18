# Learning log

## About me

- Windows user; already has a GitHub account.
- Starting confidence, from 1 (never done it) to 5 (regular use): terminal 2, coding 1, git/GitHub 1, AI tools 3.5, product/business work 1.
- Prefer short steps, plain definitions, and small code examples. Clearly label PowerShell commands versus JavaScript shown only for explanation.

## Project 2 progress — November 17, 2026

- Committed the game, installed the GitHub CLI, signed in personally, created a public repository, and pushed local history.
- Explicitly accepted publishing the author email already attached to the original commits.
- Enabled GitHub Pages from master and the root folder.
- Deliberately created separate local and remote changes, observed a rejected push, pulled to merge, and pushed successfully.
- Watched Player 1 play; recorded anonymous feedback in FEEDBACK.md.
- Prioritized a snake appearance improvement, wrote and revised the builder's brief, tested locally, and deployed it.
- Checked every live reviewer finding personally, including self-collision and smoothness the reviewer could not conclusively verify.
- Moved the snake story to Done after live verification. Phone controls remain in Backlog.
- Feedback from all five players is now documented anonymously in FEEDBACK.md, including one observed playtest. The five-player outreach goal is complete. Phone testing was deferred.
- Reviewed the new feedback: two of the four new replies explicitly questioned the timer. Separated the single explicit speed request from requests for variety or rewards. Added timer clarity to Backlog without expanding the completed redesign's scope.

## What I learned

The learner evidence below is drawn from answers and actions during the lesson. Vocabulary notes include the corrections discussed; they are not all verbatim learner statements.

### Local and cloud

Learner explanation: in the cloud, people with the link can play even when my computer is off.

Local files live on my computer. A cloud copy lives on computers reachable over the internet. A local file address does not point another person's phone to my computer.

Business equivalent: a document on my desk versus an online copy the team can access.

### Server

Learner identified the hosting company's server as the computer that sends the game to players.

A server answers requests. A browser asks for the game's files and the server sends them back.

Business equivalent: a service desk responding to a request for a brochure.

### URL and domain

Learner correctly identified a domain after a second example and described the path as telling the server what folder to look at. Constructing a full URL still needed guidance.

In https://example.github.io/my-game/, https:// specifies the secure connection, example.github.io is the domain, and /my-game/ is the path. A domain is a readable internet name; the path selects a location within the site.

Business equivalent: the business's directory name and a location within it.

### Deploying, hosting, production, and staging

Learner compared stored code to a recipe and the deployed game to the finished product. Correctly identified the old color as production when a new color existed only locally. Final explanation: the game needs to work in production too.

Deploying makes a working version available on a server. Hosting keeps it available. Local is the computer's copy; production is the live version players use; staging is a separate test environment teams may use. Publishing an update normally keeps the same URL.

Business equivalent: a draft, a test proof, and the brochure in the shop window. Delivery is complete when the customer receives it.

### GitHub and remotes

Learner found both project files and the commit history on GitHub.

A repository contains the project and its git history. GitHub stores an online copy called a remote. A public repository can be viewed by anyone, not just followers. GitHub's repository view and the playable GitHub Pages site serve different purposes.

Business equivalent: a local document and its shared team copy.

### Commits, push, and pull

Learner explained that a commit records a snapshot and that later edits require another commit. Correctly said a local commit does not reach GitHub automatically.

git add stages selected changes; git commit saves that selected snapshot locally; push sends commits to the remote. Learner's explanation of the rejected push: GitHub had commits the local copy did not, and pull brought down the commit and combined the work. The lesson used a merge to retain both histories.

Business equivalent: labeled document versions, uploading them to a shared folder, and combining edits from separate copies.

### User stories, acceptance criteria, and backlog

Learner selected the need for a more appealing snake and chose a realistic, scary visual direction.

A user story describes a user's need and why it matters: As a player, I want a more visually appealing snake, so that the game feels more enjoyable to play. Acceptance criteria are testable conditions for accepting the work, not implementation steps. Learner correctly rejected calling the story complete if the appearance passed but Restart failed.

The backlog holds possible future work. User stories, acceptance criteria, and backlogs are longstanding product-team vocabulary used by product managers, engineers, designers, and QA testers in tickets, planning meetings, and tools such as Jira or Linear.

Business equivalent: a customer's need, delivery conditions, and a waiting list of proposed work.

### Kanban and prioritization

Learner identified Doing as the place for work being started, and later correctly placed phone controls in Backlog and the verified snake redesign in Done.

Backlog is waiting work; Doing is current work; Done requires deployed and verified work. Our board limits Doing to one story.

Learner's prioritization reason: a design change can benefit laptop and phone viewers while new controls require separate input behavior. Correction: the appearance update alone does not enable phone play. Choosing by value and effort is prioritization.

Business equivalent: a team's waiting, active, and completed work queues. Product managers prioritize; teams track work with kanban boards in regular planning and delivery meetings.

### Writing a prompt or team ticket

Learner wrote the builder's brief, including goal, appearance checks, permitted files, boundaries, and reporting requirements. After a question about the missing Restart check, the learner revised it with specific length, score, timer, and best-score checks.

A useful brief defines the goal, acceptance criteria, scope, constraints, and evidence expected in the report. The resulting design matched the learner's intention; the later confusion was about typing an explanatory JavaScript snippet into PowerShell, not the builder's interpretation.

Business equivalent: a ticket or contractor brief with a clear definition of delivery. Tickets and specs are used by product managers and engineers, not only with AI.

### Adversarial review, QA, and code review

After correction, learner described the reviewer's purpose as reviewing mistakes. A fresh reviewer independently checks claims and acceptance criteria instead of trusting the builder's finished report. The learner checked the reviewer's claims on production before accepting them.

Reviewer browser play confirmed appearance, direction controls, a tested immediate-reversal case, one pellet collection and empty-cell respawn, wall collision, end statistics, and Restart preserving best score. Self-collision was inconclusive and background throttling prevented a fair smoothness check; the learner verified both in the live browser.

Business equivalent: inspecting a contractor's delivery before accepting it. QA and code review are established engineering and testing practices.

### Permission modes and sandbox

Learner explained that publishing should allow a review first. A sandbox enforces limits on local access and actions; it does not itself grant permission to publish. Network or publishing actions can cross those boundaries and require approval. Committed local edits can usually be recovered through git; public publication has external consequences.

Business equivalent: restricted access to a contractor's work area, with separate approval for public release. Project 3 introduces running commands within a sandbox's enforced limits.

## Things I still need to practice or confirm

- Distinguishing protocol, domain, and path, and constructing a URL independently.
- Distinguishing a user need, an implementation instruction, and a testable acceptance criterion.
- Recognizing PowerShell commands versus JavaScript that belongs inside the game. Explanatory JavaScript was accidentally entered in PowerShell; no game damage was reported.
- Independently explaining staging; it was introduced but not tested with an explain-back.
- Testing the game on a phone later; touch controls remain unimplemented.
- Following up with players about what changed and clarifying requests before implementing them. Feedback from five players is now recorded.

## Next project

Project 3 is a watcher chosen by the learner: nearby shows by artists they like, or class action settlements they could claim. It pulls information from a public source through APIs, with attention to keeping any access keys secret.
