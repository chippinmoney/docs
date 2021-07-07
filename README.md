# ChippIn Docs

> The ChippIIn server is written using `Express.js` and uses `MongoDB` as a database. It uses `Rapyd API` for handling all money transactions. Besides, there is a Node Rapyd SDK developed only to support ChippIn requirements that could be built as an independent package.

## How It Works
There are primarily 2 areas to focus on: `Groups` and `Wallets`. The project requires a buissness account that would be accessible only by project-owners. All chippin users ang groups are given a new ewallet that is added to the provided buissness account in the project. 

The following sections contain workflow of each user activity possible through the app:
* [Users](Users/index.md)
* [Group](Groups/index.md)

The following sections contain documentation of Node SDK for Rapyd API:
* [Rapyd Client](Rapyd/index.md)

## Overview
The source code of the project can be found [here](https://github.com/chippinmoney/backend). In the root of the project, you'll find `.env` file for your environment and `logs` directory where the server places all logs.

The `src` folder contains the all modules and there are 3 major modules in the project:
* **CONFIG**: Here, all constants are defined. The environment variables are imported here first before being used in any part of the project.

* **RAPYD**: Here, a Node SDK for Rapyd API is implemented containing all tools needed for this ChippIn Project only. It would be developed further into a public package to be used in other Rapyd Projects.

* **SERVER**: Here, all routes, models, services and utilities are defined that run the server. The starting point of the server is `src/server/app.js`.

Find the complete [Chippin API Reference here](https://github.com/chippinmoney/backend/blob/main/api_reference/api.pdf).