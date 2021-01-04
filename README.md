# discord-ext-forms
### An easier way to make forms and surveys in discord.​py.
![Downloads](https://img.shields.io/github/downloads/isigebengu-mikey/discord-ext-forms/total)
[![Documentation Status](https://readthedocs.org/projects/discord-ext-forms/badge/?version=latest)](https://discord-ext-forms.readthedocs.io/en/latest/?badge=latest)
This module is a very simple way to ask questions and create complete forms in discord.py without using an entire 30 lines!

## Example:
```py
from discord.ext.forms import Form
from discord.ext import commands
bot = commands.Bot(command_prefix="!")

@bot.command()
async def testform(ctx):
    form = Form(ctx,'Title')
    form.add_question('Question 1')
    form.add_question('Question 2')
    form.add_question('Question 3')
    result = await form.start()
    return result


>> [{'Question 1','user input'},{'Question 2','user input'},{'Question 3','user input'}]
```
![Example GIF](https://mikey.has-no-bra.in/eWrLkN.gif)
Using this module, you can make a 3 question form with only 5 lines of code.

## How to contribute
If you want to contribute to the project, submit a PR! I really don't care if you don't really know what you're doing, I'll help you through it ;D! For more info, visit the [How To Contribute](contribute.md) guide.