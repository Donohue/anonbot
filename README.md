# anonbot

![anonbot screenshot](/anonbot.png "anonbot in action")

anonbot is a Slack [slash command](https://api.slack.com/slash-commands) and [incoming webhook](https://api.slack.com/incoming-webhooks) for letting your team post anonymous messages.

## Setup

- Clone this project
- Run `heroku create`
- Create a [slash command](https://api.slack.com/slash-commands)
    - Set the command to be `/anon` or whatever you prefer
    - Set the URL to your new Heroku domain and append `/webhook` (e.g. `https://wailing-winds-0421.herokuapp.com/webhook`)
    - Add the slash command token to Heroku: `heroku config:set SLACK_OUTGOING_WEBHOOK_TOKEN=<token>`
- Create an [incoming webhook](https://api.slack.com/incoming-webhooks)
    - Add the incoming webhook URL to Heroku: `heroku config:set SLACK_INCOMING_WEBHOOK_URL=<webhook URL>`

## Copyright

Copyright &copy; Brian Donohue

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

