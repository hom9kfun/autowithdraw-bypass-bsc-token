# [Читать на русском](https://github.com/hom9kfun/autowithdraw-bypass-bsc-token/blob/main/READMEru.md)

# update 06.11.2024
+added a balance check for 0 value, i.e. if the balance is 0, the script will not send a transaction

+added the ability to switch the script to a manual balance and enter it yourself, it can be useful for tokens where some of the coins are blocked, to work you need to specify the correct decimals, you can find out in the smart contract of the desired coin, according to the standard there are 18

# 🛡️ Program for Bypassing Automatic Withdrawal of Funds from Hacked Wallets

This program will help you withdraw your funds from the automatic withdrawal that hackers set up on hacked wallets. If you replenish funds for the commission and they are instantly withdrawn to another wallet, leaving you no time to act - this script bypasses such situations, charging only 10% of the total withdrawal amount. In the future, if the program is in demand, I plan to reduce the commission to 1%.

## ⚙️ Getting Started

### 1. Setting up `config.json`

Before running the program, fill in the `config.json` file as follows:

- **`private_key_account`**: The private key of the wallet from which you want to withdraw the tokens.
- **`private_key_donor`**: The private key of the donor wallet from which BNB will be debited for transactions.
- **`contract_token_address`**: The contract address of the token(e.g. CAKE Token).
- **`recipient_address`**: The recipient address to which the tokens will be withdrawn.
- **`transfer_gas_price`**: Fee amount (in Gwei) for a token transfer transaction (default: 1 Gwei).
- **`rpc_url`**: it is recommended to change the address of the rpc node only if there are any problems with the default one

### Example `config.json`:
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

### 🚀 Launch

After filling in the `config.json` file, you can launch the `bsctoken.exe` program. If all parameters are specified correctly, you will see your funds on the specified wallet. 🥳

### 🔒 Safety of use

- **VirusTotal check**: Make sure the `bsctoken.exe` file is safe by checking it on [VirusTotal](https://www.virustotal.com/gui/file/162ec9b4188c2300aac925f6f1d06f2a6f55131736acbfd5a5888f9cedd9b857/detection). 🔍
- **Source code**: Unfortunately, for obvious reasons, the source code of the program is not available. ❌

### 📞 Support

If the program did not work for you or you have other questions, do not hesitate to write to me in Telegram: [@nevadalzt](https://t.me/nevadalzt). I will try to help you! 💬

or here: [lolz](https://lolz.live/resonancee/)

### ⚠️ Important

The program is intended only for personal wallets to help with the withdrawal of their funds! I am not responsible for theft or anything else committed by my program 🔥
