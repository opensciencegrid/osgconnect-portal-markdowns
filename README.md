# ci-connect-portal-markdowns

Separate repo to keep track of editable markdown files. These markdown files
will render in the connect portal.

## Instructions to set up Webhooks:

1. Go to the settings of your repo:

![screenshot_1](/readme_images/screenshot_1.png)

2. Click on the Webhooks tab:

![screenshot_2](/readme_images/screenshot_2.png)

3. Then click on the button labeled "add a webhook":

![screenshot_3](/readme_images/screenshot_3.png)


You will be asked the following:

1. Payload URL
2. Content Type
3. Which events would you like to trigger this webhook?

For the Payload URL, just add the following url endpoint: `https://www-dev.ci-connect.net/webhooks/github`.

For the Content Type, select `application/json`

For "Which events would you like to trigger this webhook", select "Just the `push` events"

Press save and your webhook is officially set up! Updating the markdown files
in this repo will now automatically trigger the web portal to pull the latest
files from this repo and update itself accordingly. Instructions/guide to the
relevant markdown files below.


## Form Descriptions:

Files located in the `form_descriptions` directory.

These markdown files pertain to the content that appears on form input pop-overs
(on hover). For best UI/UX, each should be limited to a one sentence description if possible.

## Home Content:

Files located in the `home_content` directory.

`home_text_headline.md` will update/contain the main page's headline

`home_text_rotating.md` will update/contain the rotating text on the main page.

Each rotating text must be separated by a `/`

For example:

`Access free opportunistic cycles/ Researcher facilitation/ High throughput computing`

## Sign-up Content:

Files located in the `signup_content` directory.

`signup.md` will update/contain the headline of the sign-up page.

`signup_instructions.md` will update/contain the sign-up instructions in a listed order.

`signup_modal.md` will update/contain the acceptable use policy.
