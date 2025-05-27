# TODO

- plan.json

frontend pages:
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

backend services:
    nextauth
    custom service for gmc api/scraping
    mailgun nhs valid verification emails
    mailgun email providers (ensure we support the main ones)
    posts api (board id)
    comments api (post id | comment parent id ?)
    postgres server for saving post/comment content