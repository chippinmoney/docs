# ChippIn Docs | Rapyd Client

> This module provides methods to make use of Rapyd APIs while abstracting away all authentication headers for the developers.

The [Rapyd Docs - Getting Started Page](https://docs.rapyd.net/build-with-rapyd/docs) provides complete tutorial on fetching the API keys: `access key` and `secret key` along with creation of their Sandbox Environment. Paste the keys in `/.env` file of this project.

That's all you need to configure Rapyd API in this project.

## How It Works
The `/src/rapyd` folder contains the all modules and there are 2 files:
* **util.js**: Here, the `https` and `crypto-js` packages are used to generate request headers and timestamp for each API call. The method to generate the headers are found in the Rapyd API Docs. After generating all headers, the request parameters and body are attached and the API call is made.

* **client.js**: Here, all wrapper methods are defined that follow the [Rapyd API Reference](https://docs.rapyd.net/reference) and use `util.js` as described above to make the API calls.
