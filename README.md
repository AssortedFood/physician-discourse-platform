# Physician Discourse Platform

## Features

- only doctors (GMC registered) can write but anyone can read
- operates on the local (trust/site denoted by GMC Designated body) and national levels separately (two sets of parallel boards)
- anonymised
  - users are given random ids that persist
  - users are tagged with their trust region
- unmoderated
  - users are allowed to post anything - totally uncensored
  - the expectation is that the high bar of a GMC registration will prevent serious issues from arrising here
- designed to allow physicians to come together and unite on issues/priorities
- 2 phase system (where n is a small number e.g. 1 to 5)
  - week 1 crowdsource issues
  - weekend 1 vote on crowdsourced issues to select n
  - week 2 crowdsource solutions
  - weekend 2 vote on crowdsourced solutions to select n
- each user gets one vote per issue (up/down)
- users can leave comments on issues in youtube style threads
- comments can be up voted/down voted
- comment/issue/suggestion bodies support simple markdown formatting
- clarify that upvotes/downvotes indicate agreement (unlike reddit where they were supposed to promote valuable contributions)
- issues page that shows currently open issues, filter and sort options (open/closed|votes|date|etc)
- issues can be tagged (not data validated, up to the author, suggest popular tags while typing)
- to close an issue (50% ?) of the total upvotes need to vote as closed
- closing an issue requires a comment explaining how it was closed, this comment? needs to reach 50% of the original votes
- closed issues are listed on an archive page
- notifications/poll newsletter to reduce voting friction (e.g. get a link to upvote/downvote/skip on that week's issues)
- users can opt out of a notification that tells them when issues they voted on have changed in status (e.g. issue added, suggestion added, closed, etc)
- bulletins that highlight successes, demographics, and make users aware of the power of the platform to drive engagement
- Profile page (GMC status, trust region, notification preferences)
- Notification settings (email cadence, issue-status alerts opt-in/opt-out)
- typo tolerant search bar for issues/suggestions
- onboarding:
  - platform goals, explanations, CLA style "I promise not to be a dick" waiver

| Field                         | Character Limit |
|-------------------------------|-----------------|
| Issue/Solution Title          | 100             |
| Issue/Solution Body           | 5 000           |
| Comment Body                  | 2 000           |


## Tech Stack

- next js
- nextauth
- typescript
- postgres db
- prisma
- vitest/playwright
- redis
- Meilisearch
- socket.io
- BullMQ
- Mailgun
- Pino
- gh actions
- docker compose
- tailwind css
- shadcn
- ESlint