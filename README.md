# vite-tools

## wallet-utils

### build
```
cd wallet-utils
docker build -t vite-wallet-utils .
```

### create mnemonic

```
docker run --rm vite-wallet-utils random_mnemonic
```

### extract private key from mnemonic

```
cd wallet-utils
# edit .env file
vim .env 
# extract private key for index=0
docker run --env-file .env --rm vite-wallet-utils extract_private

# extract private key for index=1
docker run --env-file .env --rm vite-wallet-utils extract_private 1
```

## faucet 

### build

```
cd wallet-utils
docker build -t vite-faucet .
```

### run

```
cd wallet-utils
vim .env
docker run --env-file .env --rm vite-faucet
```