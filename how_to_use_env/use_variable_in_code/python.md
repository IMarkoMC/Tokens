# How to use environment variables in Python

## If you are using `.env`

Skip this if you are not using `.env` file

### Step 1: Install `python-dotenv`

```
pip install python-dotenv
```

### Step 2: Load your `.env` file

```
from dotenv import load_dotenv

load_dotenv()

load_dotenv("your .env file name") # if your .env file name is different than ".env"
```

## Read variable in environment:

```py
import os
os.getenv("YOUR_ENVIRONMENT_VARIABLE_NAME") # return the token you set earlier
```

Something like:

```py
import os

TOKEN = os.getenv("TOKEN")

...

bot.run(TOKEN)
```
