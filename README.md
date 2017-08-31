# hackbot

A Discord bot for the Cascades Tech Club [Discord](http://discordapp.com) server.

## Setup

To work on _hackbot_, you should:

1. Clone this repository: `git clone https://github.com/osu-cascades/hackbot.git`
2. Install the latest [node.js](https://nodejs.org).
3. Install the dependencies: `cd hackbot && npm install`
4. Log in to Discord, visit the Developer resources interface, and navigate to [the _My Apps_ screen](https://discordapp.com/developers/applications/me).
5. Add a new app and give it a name, eg. _hackbot-myname-dev_.
6. Click the _Create a Bot User_ button.
7. Notice the Client ID, reveal your app's Token, and record them both for later.
8. Visit [https://discordapp.com/oauth2/authorize?client_id=INSERT_CLIENT_ID_HERE&scope=bot&permissions=0](https://discordapp.com/oauth2/authorize?client_id=INSERT_CLIENT_ID_HERE&scope=bot&permissions=0), replacing the placeholder with your real Client ID.
9. Select the server that you want the bot to join.
10. Copy the **config-example.json** file to **config.json**, and replace the keys with your own.[1]
11. Run the bot from the command line: `npm start`
12. Hack...

[1] _the !search command requires a Google API key from the [Google API Console](https://console.developers.google.com) and the !weather command requires an API key from [OpenWeather.org](https://openweathermap.org/)_

## Suggested Workflow

In a nutshell, work in the [dev](https://github.com/osu-cascades/hackbot/tree/dev) branch and don't merge to [master](https://github.com/osu-cascades/hackbot/tree/master) unless:

1. You've communicated your changes to others and given folks a _little_ time to respond (or ideally, do a code review).
2. Your changes are innocuous.

In all cases, be sure to run the test suite to make sure all tests pass. _All tests should be passing before you merge dev to master_.

You should embrace testing. _hackbot_ uses the [Jest](https://facebook.github.io/jest/) test framework. Have two console panes open: one for running and watching the test suite, and the other for everything else you need to do. You can run the test suite once with `npm test`. Once you get tired of running `npm test` manually, use the watcher by running `npm test -- --watch`. It is sweet and people will think you are a super hacker.

## References

[Creating a Discord bot and getting a token](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token)

[Tutorial: Creating a Simple Discord Bot](https://medium.com/@renesansz/tutorial-creating-a-simple-discord-bot-9465a2764dc0)

[Video Series: Creating a Discord bot with Discord.js!](https://youtu.be/rVfjZrqoQ7o)

(c) 2017 [Justin Tappert](https://github.com/JWTappert), [Adam DuQuette](https://github.com/DukeOfEtiquette), [Steven Harding](https://github.com/Otis0620). All rights reserved.
