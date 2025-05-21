# Physician Discourse Platform

## Features

### Access & Scope

Only GMC-registered doctors may contribute content, while anyone may read. Discussions take place on parallel boards at both local (site/trust, as defined by GMC Designated Body) and national levels.

### Anonymisation & Identity

All contributors are assigned a persistent, randomly generated identifier and tagged with their NHS trust region. No personal details are exposed, preserving anonymity while still allowing regional grouping of concerns.

### Posting & Content

The platform is completely unmoderated. Users may post without restriction, relying on the professionalism implied by GMC registration. All submissions support simple Markdown formatting, and authors may assign their own tags (with popular suggestions shown as they type) to help categorise issues.

### Discussion Structure

Conversations unfold in threaded, YouTube-style comment streams beneath each issue. Every comment and suggestion may be up-voted or down-voted, where votes signify agreement or disagreement, rather than quality scores.

### Phased Crowdsourcing & Voting

Physicians first crowdsource issues during the opening week, then vote over the weekend to select the top concerns. In the second week they propose solutions, and again vote on the weekend to choose the leading proposals. Each user has one up/down vote per issue.

### Issue/Suggestion Lifecycle

The issues page displays all open issues/suggestions with filters and sorts (by status, vote count, date, etc.). To close a issue/suggestion, a user must submit a close request that includes a title and body explaining how the issue/suggestion was closed. To pass, this close request must recieve up-votes totalling at least 50 per cent of the amount of the open issue/suggestion. Closed issues/suggestions are archived for reference.

### Search & Navigation

A typo-tolerant search bar lets users quickly locate issues or proposals by keywords and tags.

### Notifications & Outreach

Weekly poll newsletters deliver direct links for up-voting, down-voting or skipping each issue, reducing friction in participation. Users may opt out of status-change alerts for issues they’ve engaged with. Periodic bulletins highlight platform successes, demographic insights and the impact of physician engagement.

### User Pages & Settings

Each user has a profile page showing GMC verification status, trust region and notification preferences. In settings they control email cadence, preferred email (e.g. if they wish to recieve poll emails on a gmail account rather than their nhs mail), opt-ins for issue alerts, and may toggle between light and dark modes (defaulting to the system theme).

### Onboarding & Legal

New users encounter a concise onboarding flow explaining platform goals and agreeing to a simple code-of-conduct “I promise not to be a dick” waiver before participation.

### Character Limits

Issue and solution bodies are capped at 5 000 characters, comments bodies at 2 000 characters, and all titles are capped at 100 characters to balance expressiveness with readability and performance.

## Tech Stack

| Category               | Technology / Framework                       |
|------------------------|----------------------------------------------|
| **Language & Runtime** | TypeScript (Node.js)                         |
| **Web Framework**      | Next.js                                      |
| **Authentication**     | NextAuth.js                                  |
| **Database**           | PostgreSQL                                   |
| **ORM**                | Prisma                                       |
| **Caching**            | Redis                                        |
| **Search**             | Meilisearch                                  |
| **Real-Time**          | Socket.io                                    |
| **Background Jobs**    | BullMQ                                       |
| **Email Delivery**     | Mailgun                                      |
| **Logging**            | Pino                                         |
| **Testing**            | Vitest (unit) & Playwright (E2E)             |
| **CI/CD**              | GitHub Actions                               |
| **Containerisation**   | Docker Compose                               |
| **Styling**            | Tailwind CSS & shadcn                        |
| **Linting**            | ESLint                                       |

## Contributing

Contributions are welcome. Feel free to fork the repo and open a pull request.

## License

This project is licensed under the terms found in the [LICENSE](./LICENSE) file.