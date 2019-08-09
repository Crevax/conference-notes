# Quality is Job One - Ensuring Automation in Your Teams Quality Process by Eric Landes

## Definitions

Continuous Testing - Testing is integrated into everyting the team does: in conjunction with coding (e.g. Unit Testing), et. al.

## Concepts

Everyone is a tester:

- Developers
- Business Analysts
- Security Team

Write tests before code (TDD).

### Types of Testing

- Exploratory
- Regression / Smoke
- Acceptance
- Unit

### Unit Tests

For developers (product owner doesn't need to see them). Should only test one thing (and thus be quick). Not testing integration with anything.

### Smoke Test

Ran after a build: ensure that app is at least running.

## Regression Test

Missed this, whoops.

## Benefits

- Repeatability for quality (catch regressions)
- Reduce total test time

## Behavior Driven Development

Using the Gherkin Syntax can be useful for writing stories. Can be beneficial even without automation.

## Misc

No such thing as a QA sprint; the product should be ready to ship at the end of a sprint.
Automate as much as possible.

User stories (or PBIs??) should be kept small. Make sure estimates are for full completion, not just code completion.

Introduce the testing plan witin the backlog; ensure automation is a requirement for a story to be considered "done". If testing can be added to stories, consider adding them in as technical debt.

## Introducing into a Legacy App

Start with intigration tests (like with Selenium), as code doesn't need to change to support automated tests.

## Overcoming TDD Resistance

???
