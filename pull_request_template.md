 - [ ] :heart_on_fire: production is broken, business critical bug
 - [ ] :mending_heart: fixes a bug in some circumstances
 - [ ] :sparkling_heart: removes technical debt
 - [ ] :revolving_hearts: is blocking dependent PRs
 - [ ] :gift_heart: adds a new feature
(if your PR does more than one of these, consider splitting it up!)

# Description

[IssueLink](url)

# Submitter

Please be patient with the reviewer. They have their own tasks to do and may not be able to switch context to your review immediately.

Try to make the process as easy as possible for the reviewer. This should include reviewing your PR yourself first. Consider letting the reviewer you have in mind know that you'll be asking them to review your PR, particularly for large and/or time-sensitive PRs. Make sure the issue accurately reflects what you have solved, and that there is documentation in the code that explains why it has been solved this way (that could include links to external Figma or other diagrams)

Vary your reviewers. They can be people you think are either more or less experienced than you, and varied reviewers is a good way to spread knowledge across the team. Do take the reviewers skillset into account though, do not ask a pure Frontend dev to review Backend code or visa versa!

If in doubt, put a time in the reviewers calendar to have a Zoom discussion with screen sharing.

# Reviewer

Please try to be objective and stick to the changes in this PR and how they solve the issue linked above.

Consider putting a time in the submitters calendar to have a Zoom discussion with screen sharing. Also consider reserving a time in your own calendar to review the PR - this means the submitter can see you're going to be working on it, and stops other meetings being dropped into your calendar and displacing review time.

If you you think you are too busy to review a PR in a timely manner (2 working days for bugs, a week for features) let the submitter known as soon as possible so they can find an alternative reviewer.

Don't worry if you don't understand all the changes, but if so clearly communicate this to the submitter so they can explain those parts of the codebase to you or get another reviewer for those changes. Try to avoid "bike shedding" (i.e. heavily criticizing the small part you understand and ignoring the large parts you don't).

Review it once and add comments on the relevant areas. Afterwards, follow up on issues identified with replies and avoid creating new comment threads. It is frustrating for a submitter to have some feedback initially, and then a separate set of feedback later from the same reviewer.

## :tada: Highlight

Acknowledge the best piece of this PR with a comment. What taught you something new, or you thought was particularly elegantly structured, or well commented and explained?

## Documentation

 - [ ] Do the changes have comments?
 - [ ] Do the comments add information and context (not repeating the code)?

## Testing

 - [ ] Do the changes have "golden path" test coverage?
 - [ ] Do the changes have handled exception test coverage?
 - [ ] Do the changes cover common failure cases you can foresee?
 - [ ] Has it passed CI?
 - [ ] (server) Is overall coverage increasing?
 - [ ] (server) Are fixtures and/or builders used to reduce duplication of test setup?

## Danger points

 - [ ] (server) Are the changes database alone, or non-database changes alone? Database changes should not be mixed with other changes.
 - [ ] (server) Are the changes migration(s) alone, or non-migration(s) alone? Migrations should not be mixed with other changes.
 - [ ] (server) Are the server dependencies unchanged?
