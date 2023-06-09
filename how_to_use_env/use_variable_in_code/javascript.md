# Use your environment variable in JavaScript

## If you are using a `.env` file

Skip this if you are not using `.env` file

### Step 1: Install `dotenv`

```
npm install dotenv
```

### Step 2: Load variables from `.env` file

```js
require("dotenv").config(); // if you are using CJS

import { config } from "dotenv"; // if you are using ES6
config()
```

## Read variable in environment:

```js
process.env.YOUR_VARIABLE_NAME // token you set earlier
```

Something like:
```js
client.run(process.env.TOKEN)
```
