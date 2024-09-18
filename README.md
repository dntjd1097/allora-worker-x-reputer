Allora Worker Node x Reputer 

## 1. Clone the code from this repository

```bash
git clone https://github.com/hiephtdev/allora-worker
cd allora-worker
```

## 2. Install Docker and necessary libraries

```bash
chmod +x init.sh
./init.sh
```

## 3. Proceed with the faucet

- Go to the link and paste the Allora wallet address in the format allo1jzvjewf0... https://faucet.testnet-1.testnet.allora.network/

## 4. Run the worker
- Run the worker => wait until it reports success, then it’s done.
```bash
cd allora-node
```

- If this is your first time, enter the command below, providing the wallet_name, mnemonic - seed phrase of the wallet, and cgc_api_key - API key obtained from CoinGecko
```bash
./init.config.sh "wallet_name" "mnemonic" "cgc_api_key"
# example: ./init.config.sh "MysticWho" "gospel guess idle vessel motor step xxx xxx xxx xxx xxx xxx" "GC-xxxxxx"
```

## 5. Build Your Worker Node
```bash
docker compose up --build -d 
```

Check Logs to Make Sure its Running
```bash
docker compose logs -f 
```
