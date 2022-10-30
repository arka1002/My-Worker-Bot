# My-Worker-Bot
## What does it do?
This bot sends alerts to users in a slack group regarding issues opened, edited, deleted, transferred, pinned, unpinned, closed, reopened, assigned, unassigned, labeled, unlabeled, milestoned, demilestoned, locked, or unlocked.
## How to use it?
Currently, this bot is in a condition where a person have to self host it in order to use it. Further modifications will be planned.
The steps to self host are listed below:
### Making a Clouflare account 
- Make a cloudflare account from [here](https://dash.cloudflare.com/sign-up/workers)
- Install Wrangler by `npm install -g wrangler`
- Authenticate Wrangler by `wrangler login`
### Configuring Slack
- Kindly go to this [link](https://api.slack.com/apps) and select **Create New App**.
- On the sidebar of Slack’s UI, select **Incoming Webhooks**.
- In **Webhook URLs for your Workspace**, select **Add New Webhook to Workspace**.
- On the following screen, select the channel that you want your webhook to send messages to (you can select a room, like #general or #code, or be messaged directly by your Slack bot when the webhook is called.)
- Authorize the new webhook URL.
- On the Slack sidebar, select **Slash Commands**.
- Create your first slash command.
![image](https://user-images.githubusercontent.com/105232141/198863836-cf6b966f-00c3-4603-8bc9-b4159fcc5991.png)  
Request URL should be = The router url generated(discussed after a few paras) + /lookup
