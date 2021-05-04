# TestStripePaymentBot
This is the source code of the Telegram bot: [@TestStipePaymentBot](https://t.me/TestStripePaymentBot), By [Muaath Alqarni](https://t.me/Muaath_5).
This bot is based on Bot API 5.2, And uses Payments 2.0.
If you need a translitions of the bot, You can see the versions below from this source:
* [@TestStipePaymentBot](https://t.me/TestStripePaymentBotAr)

If you want to add a translition, Send to [Muaath Alqarni](https://t.me/Muaath_5) in English, with `settings.json` file contains all translitions.

## Bot commands
| Command     | Description                                                       | Allowed users | Style                              |
|-------------|-------------------------------------------------------------------|---------------|------------------------------------| 
| `/start`    | Sends start message with Main bot keyboard                        | Any           | `/start`                           |
| `/invoice`  | Sends main Invoice in `settings.json`                             | Any           | `/invoice` & `/invoice {$payload}` |
| `/inline`   | Sends a message with an `InlineKeyboardMarkup` for inline queries | Any           | `/inline` & `/start inline`        |
| `/project`  | Returns the developer info and the Github source code repo link   | Any           | `/project` & `/start project`      |
| `/help`     | Returns info about commands and what can bot do                   | Any           | `/help` & `/start help`            |
| `/settings` | Returns info about current invoices                               | Admin         | `/settings`                        |
| `/admin`    | Shows admin keyboard (Selective)                                  | Admin         | `/addinv {$JSON}`                  |
| `/addinv`   | Adds an invoice                                                   | Creator       | `delinv {$payload}`                |
| `/delinv`   | Deletes an invoice by payload


## FAQ
| Question                            | Answer |
|-------------------------------------|--------|
| What's used Bot API version?        | 5.2    |
| What's the project language         | PHP.   |
| Where's The Bot hosted in           | [Heroku](https://heroku.com) |
| Does it needs a database?           | No, It only uses `settings.json` file to store invoices and translitions |
| Which library is used?              | `telegram-bot-api.php` file |
| Is the Bot supports inline queries? | Yes.   |
| Does it real payment?               | No, It's a test payment, But you can import the bot to a real payment bot. |
| Can the Bot get the payment info?   | No, It's not accessed by Bot API. You can check the source code file. |
| What's the data that bot collects?  | The bot collects User info, Shipping info, Invoice info. |
| Which place bot stores the data in? | The bots sends the data to the _Logs chat id_, It could be a channel or a group or a private chat. |

## How the bot works?
The bot is getting updates using _webhook_ via `webhook.php` file.
For more info, Read: [How @TestStipePaymentBot works?](url).

## Import the bot
Anyone can import the bot, But developer suggested to import the bot to your own bot.
Read: [How to import @TestStripePaymentBot to my own real?](url).

## Issues & Pull requests
Issues are welcome.

Pull requests are welcome, but should follow these instructions:
1. Link the pull request with an opened issue.
2. Contains **Only** one fix/feature implement.

Questions should be in [Discussion tab](url), Not an issues.

## License
This project is under [MIT License](), By Muaath Alqarni.
