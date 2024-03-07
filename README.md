# PI-Chan
Get prompts/descriptions of images uploaded on discord.

# You can add PI-Chan into your server without hosting!
Just join the [touhouai](https://discord.gg/touhouai) discord, and click on PI-Chan's profile to see the "Add to Server" button. Click it and you'll invite it!

![Discord Server](https://discordapp.com/api/guilds/930499730843250783/widget.png?style=banner2)

## Functionality

This Discord bot reacts to any image with generation metadata from the most/all popular webuis. (Create an issue if your favorite webui doesn't have it!)
If you want to get a *rough* prompt, react with ❔

Install [this](https://github.com/ashen-sensored/sd_webui_stealth_pnginfo) if it breaks!

## Setup

1. Clone the repository
2. Install the dependencies with `pip install -r requirements.txt`
3. Create a Discord bot and invite it to your server
4. Enable the `Message Content Intent` in the Discord developer portal
5. Enable the `Server Members Intent` in the Discord developer portal
6. Create a file named ".env" in the root directory of the project
7. Set `BOT_TOKEN=<your discord bot token>` in the .env file
    7.1. So like `BOT_TOKEN=HFBVSAOa876vat764bq8967fgh8d8a76`
8. Add the channel IDs you want the bot to work in into the `config.toml` file
9.  Run the bot with `python3 PromptInspector.py`

## Examples
![1](images/mag_glass.png)
![2](images/cui_md.png)
![3](images/predicted.png)

## Webui Support

|              Webui             | Supported? |
|:------------------------------:|:----------:|
| Automatic 1111, sd.next, forge |      ✅     |
|             ComfyUI            |     🟨*     |
|          Stable Swarm          |      ✅     |
|             NovelAI            |      ✅     |
|             Fooocus            |     ✅**    |

*It returns the workflow and tries to extract the prompt, loras and checkpoints used

**Please test in TouhouAI, I think it will work though
