# Telegram LogicApp Connector
A simple template for connecting Azure Logic Apps to Telegram. See the blogpost @ https://www.re-mark-able.net

## Prerequisites
Creating a telegram bot by following this tutorial: https://docs.microsoft.com/en-us/azure/bot-service/bot-service-channel-connect-telegram?view=azure-bot-service-4.0

## Supported Telegram API calls
* SendMessage -> Sends a plain text message to a group or chat.
* GetUpdates -> Gets the last 100 updates send to your bot. This can be controlled by setting the offset or limit.

## Getting it to work
For this to work you need to create a Azure Logic App Custom Connector. This can be done by going to the Azure portal https://portal.azure.com where you can search for it.

![LogicAppConnectorMarketPlace](https://github.com/foppenm/TelegramLogicAppConnector/blob/master/Images/LogicAppCustomConnector.png)

Start creating a connector like below and let Azure do its job

![CreateApp](https://github.com/foppenm/TelegramLogicAppConnector/blob/master/Images/CreateTheApp.png)

After the creation is done we can start editing it by going here

![EditConnector](https://github.com/foppenm/TelegramLogicAppConnector/blob/master/Images/EditConnector.png)

Simply import the Telegram.json from this repository 

![ImportTempalte](https://github.com/foppenm/TelegramLogicAppConnector/blob/master/Images/Importfile.png)

Now you only have to press "Update Connector" and you can start using it in your logic apps. Optionally you can pick a color and choose an icon to use for this. This determines how it is presented in the logic apps designer

## Using it
Create a logic app and go to "Custom" where the connector will appear

![ImportTempalte](https://github.com/foppenm/TelegramLogicAppConnector/blob/master/Images/UseConnector.png)

After adding it you can add the accesstoken and chatid (acquired in the prerequisite tutorial) and start sending messages.

![ImportTempalte](https://github.com/foppenm/TelegramLogicAppConnector/blob/master/Images/SendMessage.png)
