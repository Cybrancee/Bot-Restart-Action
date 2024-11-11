# Bot-Restart-Action

This GitHub Action is designed to automatically restart a bot hosted on Cybrancee whenever there's a push to your repository. This can be useful for automatically deploying updates, fixing bugs, or simply refreshing the bot's environment.

</br>

# Requirements

For this you will need: 
- A Cybrancee panel API key. You can get yours [here](https://panel.cybrancee.com/account)
- Your server ID found from the Dashboard of your bot.

# Set-up

### A detailed guide can be found [On the Cybrancee Knowledge Base](https://cybrancee.com/learn/knowledge-base/how-to-automatically-restart-your-bot-after-pushing-changes-to-github/)

The GitHub action requires 1 secret and 1 variable to be setup in your repository. To do this navigate to your repository settings and click on "Secrets and Variables" and then click "Actions"
</br>

The secret is your Cybrancee panel Api ket and will need to be called `PTERODACTYL_API_KEY`
</br>

The variable is your server ID and will need to be called `SERVER_ID`
</br>

After setting up your Secret and Variable, head to the repository actions and create a new action. Then paste the contents of [main.yml](/main.yml) into your action and commit the changes.
</br>

Now after each commit to your `main` branch your bot will automatically restart and pull the new changes from github.
</br>
