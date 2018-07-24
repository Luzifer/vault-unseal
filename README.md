[![Go Report Card](https://goreportcard.com/badge/github.com/Luzifer/vault-unseal)](https://goreportcard.com/report/github.com/Luzifer/vault-unseal)
![](https://badges.fyi/github/license/Luzifer/vault-unseal)
![](https://badges.fyi/github/downloads/Luzifer/vault-unseal)
![](https://badges.fyi/github/latest-release/Luzifer/vault-unseal)

# Luzifer / vault-unseal

This small utility is a helper to automatically unlock a [Vault](https://www.vaultproject.io/) instance by having an amount of servers having access to one or multiple tokens.

## Features

- Provide one or multiple tokens for the unseal command
- `vault-unseal` does check whether the vault instance is locked and tries to unlock if it is locked

## Usage

```bash
# ./vault-unseal --help
Usage of ./vault-unseal:
      --instance="http://127.0.0.1:8200": Vault instance to unlock
  -1, --oneshot[=false]: Only try once and exit after
      --sleep=30: How long to wait between sealed-state checks
      --tokens="": Tokens to try for unsealing the vault instance
```
