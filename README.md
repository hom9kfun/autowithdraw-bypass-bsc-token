# [Читать на русском](https://github.com/hom9kfun/autowithdraw-bypass-bsc-token/blob/main/README_RU.md)

# 🛡️ Program for Bypassing Automatic Withdrawal of Funds from Hacked Wallets

This program will help you withdraw your funds from the automatic withdrawal that hackers set up on hacked wallets. If you replenish funds for the commission and they are instantly withdrawn to another wallet, leaving you no time to act - this script bypasses such situations, charging only 10% of the total staking withdrawal amount. In the future, if the program is in demand, I plan to reduce the commission to 1%.

## ⚙️ Getting Started

### 1. Setting up `config.json`

Before running the program, fill in the `config.json` file as follows:

- **`private_key_account`**: The private key of the wallet from which you want to withdraw the stake.
- **`private_key_donor`**: The private key of the donor wallet from which BNB will be debited for transactions.
- **`contract_token_address`**: The contract address of the token that is in the stake (e.g. CAKE Token).
- **`recipient_address`**: The recipient address to which the tokens from the stake will be withdrawn.
- **`transfer_gas_price`**: Fee amount (in Gwei) for a token transfer transaction (default: 1 Gwei).
- **`rpc_url`**: it is recommended to change the address of the rpc node only if there are any problems with the default one

### Example `config.json`:
```json
{
    "private_key_account": "yourprivatkey",
    "private_key_donor": "yourdonorkey",
    "contract_token_address": "contract_token",
    "recipient_address": "your_recipient_adr",
    "transfer_gas_price": "1 gwei",
    "rpc_url": "https://rpc-bsc.48.club"
}
```

### 🚀 Launch

After filling in the `config.json` file, you can launch the `bsctoken.exe` program. If all parameters are specified correctly, you will see your funds on the specified wallet. 🥳

### 🔒 Safety of use

- **VirusTotal check**: Make sure the `bsctoken.exe` file is safe by checking it on [VirusTotal](https://www.virustotal.com/gui/file/96a6e2bc52fb1e0d0cb1f6df47f16eedda32a502de8a247c7539b706230bf1ac). 🔍
- **Source code**: Unfortunately, for obvious reasons, the source code of the program is not available. ❌

### 📞 Support

If the program did not work for you or you have other questions, do not hesitate to write to me in Telegram: [@nevadalzt](https://t.me/nevadalzt). I will try to help you! 💬

or here: [lolz](https://lolz.live/resonancee/)

### ⚠️ Important

The program is intended only for personal wallets to help with the withdrawal of their funds! I am not responsible for theft or anything else committed by my program 🔥
