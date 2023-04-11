# Workshop-year-end-project
How to get into a year-end project ?

## Groups
figure out:
* the abilities of each members,
* what they like,
* the projects they're working on at the same time

## Organisation and tools

### Github - Branches
* have the same norm (ex: feature/...)
* merge branches ONLY with Github pull requests
* you can protect the `main` branch in the settings to only be able to make changes on it after a verified pull request
* you can assign people to look at the pull request and only merge after they approved
* comment the pull requests
example of a pull request:
![](https://cdn.discordapp.com/attachments/902981758197301318/1095394370947125330/image.png)

### Github - Commits
* have the same norm for the whole group => [ex](https://github.com/Gradrien/Git-Shortcuts)
* detail commits:
    * first line for type of commit (addition, modification, fix of a bug, ...), file(s) modified and overlook
    * second line is gonna detail more what you did

### Github - Projects
* issues
* project template
* roadmap
* link branches / pull requests to issue
* link CLI to issues
* explanations [here](https://github.com/Lukacms/Workshop-end-year-project/blob/main/Projects.md)

### Github - Actions (or CI/CD)
You already did the `Chocolatine` ;)
* mirroring
* compilation (you wouldn't want a build failed on the last TA)
* criterion tests

### Discord
To use Discord as a notifier for each action of your repository, you'll need to make a server with different channels for different topics; ex:

* `general`
* `webhook`
* `voice channel`

Now we can start to configure the Discord server :

- Go to the server's settings
- Click on "Integrations"
- Click on "Webhooks"
- "New webhook", then copy the url

<img src="https://media.discordapp.net/attachments/902981758197301318/1095392000251023411/image.png" width="600">

<!-- ![](https://media.discordapp.net/attachments/902981758197301318/1095392000251023411/image.png | width=250) -->

*Don't forget to give it a name and to choose the channel where you want to receive the messages...*

Now you need to go to the settings of your Github repository :

- Go to "Webhook" on the left sidebar
- "Add webhook"
- Paste the url and add a /github at the end of it
- Switch from "application/x-www-form-urlencoded" to "application/json"
- Then you choose which notification you want to receive on the discord channel
- After this, click on "Add webhook"

<img src="https://cdn.discordapp.com/attachments/902981758197301318/1095391072248664084/image.png" width="600">

<!-- ![](https://cdn.discordapp.com/attachments/902981758197301318/1095391072248664084/image.png) -->

You'll see that it works if after adding the webhook, there's a validation sign on the left side of the webhook
