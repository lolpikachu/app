# chatbot


In BOT_CONFIG.py is a dataset.  It is organized into a dictionary that has two items: **intents** and **failure phrases**.

The **intents** item is a nested dictionary. It contains collections of different intent phrases. 
Every intent item inside **intents** is a dictionary that has two items — **examples** and **responses**.  
**examples** key is a list of possible user inputs. **responses** key is responses of the bot to the user's phrases.

In chat_bot.py is a logic of chatbot.

bot() function gets intent from the user. If it can find a response by intent it returns intent. If it can't it returns failure phrase.☠☠☠


get_intent() function returns response. To calculate an accurate response was used Levenshtein edit distance [algorithm]https://en.wikipedia.org/wiki/Edit_distance.
