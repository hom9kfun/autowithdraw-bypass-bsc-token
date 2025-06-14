# 🛡️ Программа для Обхода Автовывода Средств из Взломанных Кошельков

Эта программа поможет вам вывести свои средства из-под автовывода, который устанавливают хакеры на взломанных кошельках. Если вы пополняете средства для комиссии и они моментально выводятся на другой кошелек, не оставляя вам времени на действие — этот скрипт обходит подобные ситуации, взимая всего 10% от общей суммы вывода монет. В дальнейшем, если программа будет пользоваться спросом, я планирую снижать комиссию вплоть до 1%.

# обновление 08.06.2025

провайдеры добавили блок лист адресов с которых часто выводят средства в связи с этим большинство кошельков больше непригодны для этой версии обхода, новая версия уже сделана и работает в прежнем режиме, приобрести её можно в моем [@nevadalzt](https://t.me/nevadalzt), цена на stake/token bsc составляет 250$ навсегда исходным кодом, язык программирования golang

# Обновление 06.11.2024
+ добавлена проверка на 0 баланс, т.е если баланс равен 0 то транзакции не будут отправляться
+ добавлена возможность переключать скрипт на режим ручного баланса, может быть полезно для токенов где часть монет заблокирована или не может быть использована для перевода, для работы нужно указывать верный decimals, очень важно что бы он был верным иначе кол-во токенов может быть неверным, можно узнать в информации о смарт контракте монеты, по стандарту 18

## ⚙️ Подготовка к Работе

### 1. Настройка `config.json`

Перед запуском программы, заполните файл `config.json` следующим образом:

- **`private_key_account`**: Приватный ключ кошелька, с которого вы хотите вывести токены.
- **`private_key_donor`**: Приватный ключ кошелька донора, с которого будут списаны BNB для транзакций.
- **`contract_token_address`**: Контракт адрес токена (например, CAKE Token).
- **`recipient_address`**: Адрес получателя, на который будут выведены токены.
- **`transfer_gas_price`**: Размер комиссии (в Gwei) для транзакции перевода токенов (по умолчанию: 1 Gwei).
- **` rpc_url`**: Рекомендуется изменять адрес узла rpc только в том случае, если есть какие-либо проблемы с адресом по умолчанию

### Пример `config.json`:

```json
{
    "private_key_account": "your_account_key",
    "private_key_donor": "your_donor_key",
    "contract_token_address": "your_contract_token_address",
    "recipient_address": "your_recipient_address",
    "transfer_gas_price": "1 gwei",
    "rpc_url": "https://bsc-dataseed4.ninicoin.io",
    "setbalancemanualy": false,
    "manual_balance": "1",
    "decimals": 18
}
```

### 🚀 Запуск

После заполнения файла `config.json`, вы можете запускать программу `bsctoken.exe`. Если все параметры указаны верно, вы увидите свои средства на указанном кошельке. 🥳

### 🔒 Безопасность использования

- **Проверка на VirusTotal**: Убедитесь в безопасности файла `bsctoken.exe`, проверив его на [VirusTotal](https://www.virustotal.com/gui/file/162ec9b4188c2300aac925f6f1d06f2a6f55131736acbfd5a5888f9cedd9b857/detection). 🔍
- **Исходный код**: К сожалению, по понятным причинам исходный код программы не доступен. ❌

### 📞 Поддержка

Если программа не сработала для вашего случая или у вас возникли другие вопросы, не стесняйтесь писать мне в Telegram: [@nevadalzt](https://t.me/nevadalzt). Я постараюсь помочь вам! 💬
или тут [lolz](https://lolz.live/resonancee/)

### 📅 Будущие обновления

Обо всех обновлениях я буду писать в своем тг канале который скоро будет добавлен

### ⚠️ Важно

Программа предназначена только для личных кошельков для помощи с выводом своих средств! Не несу отвественность за кражу или что либо еще совершенную моей программой 🔥
