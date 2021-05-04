# How to import @TestStripePaymentBot to my own bot?

## Repository import
You can import this repository by: [Use as templete](https://github.com/Muaath5/TestStripePaymentBot/generate).
And make sure that repository in GitHub is **_private_**, To hide the bot configurations.

## Edit configurations
All configurations are in `config.php` file.
It was stored in a PHP file for more security.
| Property        | Value                                                 |
|-----------------|-------------------------------------------------------|
| `Token`         | Bot token obtained via @BotFather                     |
| `ProviderToken` | A payment provider token obtained via @BotFather      |
| `LogsChatID`    | A Telegram chat id if private, Or username if public. |

## Edit translitions [Optional]

## Add custom invoices [Optional]
All invoices is stored in `invoices` property as array of objects.
Each invoice contains:
| Property        | Value                                                 |
|-----------------|-------------------------------------------------------|
| `title`         | Invoice title, Or object that sells. []               |
| `description`   | Invoice description                                   |
| `LogsChatID`    | A Telegram chat id if private, Or username if public. |

## Link with Heroku
1. Create an app in Heroku.
2. Use GitHub as the app source.
3. Link repository you made with Heroku.

## Set webhook
Use a software like `curl` Or `postman` to do this easy.
Or you can use `GET` request to set webhook via browser.

The link in bowser should be like this:
```
https://api.telegram.org/bot<bot_token>/setWebhook?url=https://<heroku_app_name>.herokuapp.com/webhook.php
```
But replace `<bot_token>` and `<heroku_app_name>` with your owns.
