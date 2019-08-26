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

| Setting | Description | Sample |
| -- | -- | -- |
| accentureUserName | The username you use within Accenture to login (without @accenture.com) | heinz.doofenshmirtz |
| accenturePassword | Your password | .... |
| telegramBotToken | The token used by your bot. Can be created by talking to the BotFather: [Botfather](https://telegram.me/botfather) | 123456789:AAABABABAABA_JJDJARHAHR93F_fww84h |
| telegramUserId | Your Telegram UserId, not sure how to find this | 123456789 |
| symantecSecret | Your Symanted secret. Can be created using this tool: [VIPAccess](https://github.com/dlenski/python-vipaccess). Make sure to then trust this secret using this url: [Symantec](https://federation-sts.accenture.com/adfs/ls?wa=wsignin1.0&wtrealm=https://federation-sts.accenture.com/vip/ls/&wctx=rm=0&id=passive&ru=%2fvip%2fls%2fsymantec%2fsignon) | GFH39GH2L5GH2GI4853HL9ASG5O2HGIR |
| subscriptionKeyFormRecognizer | The Subscription key for an instance of Form Recognizer that's trained on Receipts (Basically ask Devedse) | a00b1c2222d44e55555555ffffff1aa323 |
| modelIdFormRecognizer | The guid of the Model in Form Recognizer that's trained on Receipts (Basically ask Devedse) | 1005bb2b-550f-40e7-816c-caf3c74abf2a |
