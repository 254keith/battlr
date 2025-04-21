# Bot Battlr

Welcome to **Bot Battlr**, the one and only spot in the known universe where you
can custom build your own Bot Army!

Here's the scenario: a galactic overlord has hired you, a galactic web developer, to develop a galactic web app that will allow them to browse through a list of robots, view a robot's details, and, enlist a bot into their army.

## Instructions

For this project, you’ll be building out a React application that displays a list of available bots, among other features.

Part of what this code challenge is testing is your ability to follow given instructions. While you will definitely have a significant amount of freedom in how you implement the features, be sure to carefully read the directions for setting up the application

### project setup


1. Run this command to get the backend started: npx json-server --watch db.json --port 8002
2. In a new terminal, run npm start. This will run your React app in a new port.

### Endpoints

The base URL for the backend is: http://localhost:3000

### deliverables
The should be able to:


1. See profiles of all bots rendered in BotCollection.
2. Add an individual bot to my army by clicking on it. The selected bot should render in the YourBotArmy component. The bot can be enlisted only once. The bot does not disappear from the BotCollection.
3. Release a bot from my army by clicking on it. The bot disappears from the YourBotArmy component.
4. Discharge a bot from their service forever, by clicking the red button marked "x", which would delete the bot both from the backend and from the YourBotArmy on the frontend.

# Author && License
[Bob Oyier](https://github.com/oyieroyier)


### ISC License (ISC)
[![License: ICL](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)
