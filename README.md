# DeveMyteParkingExpenser
An internal tool used to expense receipts in MyTe.

Note: This software is provided without warranties. You should host this Azure template on your own private Azure Subscription so other users can't extract passwords or other secrets from the AppSettings of the application.

## Create an Azure Docker Instance that hosts a Telegram Bot

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fdevedse%2FDeveMyteParkingExpenser%2Fmaster%2FDeveMyteParkingExpenser.ARM%2FWebSite.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fdevedse%2FDeveMyteParkingExpenser%2Fmaster%2FDeveMyteParkingExpenser.ARM%2FWebSite.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## Settings

| Setting | Description | Example |
| -- | -- | -- |
| accentureUserName | The username you use within Accenture to login (without @accenture.com) | heinz.doofenshmirtz |
| accenturePassword | Your password | .... |
| telegramBotToken | The token used by your bot. Can be created by talking to the BotFather: [Botfather](https://telegram.me/botfather) | 123456789:AAAAAAAAAAAA_BBBBBBBBBBBBB_cccccc |
| telegramUserId | Your Telegram UserId, on telegram search for [@userinfobot](https://telegram.me/userinfobot), start the chat and it will reply with your user id | 123456789 |
| symantecSecret | Your Symanted secret. Can be created using this tool: [VIPAccess](https://github.com/dlenski/python-vipaccess). Make sure to then trust this secret using this url: [Symantec Self Service Portal](https://federation-sts.accenture.com/vip/ls/symantec/signon) | GFH39GH2L5GH2GI4853HL9ASG5O2HGIR |
| subscriptionKeyFormRecognizer | The Subscription key for an instance of Form Recognizer that's trained on Receipts (Basically ask Devedse) | 0000000000aaaaaaaaaa1111111111bbbb |
| modelIdFormRecognizer | The guid of the Model in Form Recognizer that's trained on Receipts (Basically ask Devedse) | 00000000-1111-2222-3333-444444444444 |
