# TODO

- plan.json

```
pages:
    onboarding:
        explain the site page
        sign waiver
        set user settings/skip

    login page:
        login w/ email/SSO
        make an account
        forgot my password

    user settings pages:
        notifications
        dark/light/system theme
        preferred email

    core functionality:
        local||national issues||proposals boards
        post page (embedded on boards as cards but exists as a page to make comments on)

components:
    navbar/sidebar
    search
    post card
    comment thread
    comment card

services:
    nextauth
    custom service for gmc api/scraping
    mailgun nhs valid verification emails
    mailgun email providers (ensure we support the main ones)
    posts api (board id)
    comments api (post id | comment parent id ?)
    postgres server for saving post/comment content
    recaptcha

tests:
    api routes
    mailgun test send to:
        nhs uk emails
        gmail
        hotmail
        etc
    nextauth gmc api/scraper test
    db tests:
        read
        edit
    playwright UI tests:
        card button functionalities (upvote/downvote websockets)
```