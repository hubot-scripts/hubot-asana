# Asana for Hubot

Add tasks to Asana using Hubot.

## Installation

Add `hubot-asana` to your `package.json` file:

    "dependencies": {
      "hubot": ">= 2.5.1",
      "hubot-scripts": ">= 2.4.2",
      "hubot-asana": ">= 0.0.0"
    }

Then add "hubot-asana" to your `external-scripts.json` file:

    ["hubot-asana"]

Finally, run `npm install hubot-asana` and you're done!

### Configuration

- ASANA_WORKSPACE_ID - Your workspace's ID.
- ASANA_TEAM_ID - Your team's ID.
- ASANA_DEFAULT_PROJECT_ID - Your default project's ID.
- ASANA_DEFAULT_PROJECT_NAME - Your default project's name.

### Usage

To use the bot, you'll have to create an api token.
Open Asana, go to "My Profile Settings" , then "Apps", and create a new "Personal Access Tokens".
Then you can talk 1-1 to asana with your token

    asana: HERE_IS_MY_TOKEN

now your are good to go.

A task added to Asana must have a name. Both an assignee and a project are optional. Some examples:

    asana: ship some code
    asana: ship some code #bugs
    asana: @travis ship some code
    asana: @steve ship some code #bugs
