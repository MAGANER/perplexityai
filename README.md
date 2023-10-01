# perplexityai
A python api to use labs.perplexity.ai

#NOTE:
This stopped working due to Javascript/Bot checks after they moved to Cloudflare.<br>
For a working version using Selenium see: https://github.com/ShaneOss/perplexitylabs/

# Usage
You can just import the Perplexity class and use it like this:
```python
from Perplexity import create_perplexity

ai = create_perplexity()
if ai is not None:
    answer = ai.search("What is the meaning of life?")
    print(answer)
else:
    print("unable to connect to server!")

```
# The model used can be updated in Perplexity.py
    #Available Models
    # llama-2-7b-chat
    # llama-2-13b-chat
    # llama-2-70b-chat
    self.model = "llama-2-70b-chat"

# Note on websocket dependency
Don't use ```pip install websocket```, but ```pip install websocket-client```, since it's the correct package that is used by this class.


