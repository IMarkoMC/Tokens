Read variable TOKEN in environment:

```py
import os
os.getenv("TOKEN") # return the token you set earlier
```

Something like:

```py
import os

TOKEN = os.getenv("TOKEN")

...

bot.run(TOKEN)
```
