# CryptoCubera

Decision support for **BTC / ETH / SOL** index-style crypto options GEX.

Signal venue: **Deribit** (option chain / tape). Execution venue: **Delta Exchange India** (INR). Manual Decision / paper path — **no auto-place**.

Split from [`cubera-gex-cockpit`](https://github.com/jagadish-nsr/cubera-gex-cockpit) (CRY-23) so equity Cubera (Nifty / Bank Nifty / Sensex) stays in its own repo.

## Quick start

```bash
python3 -m pip install -r requirements.txt
./run_crypto.sh              # Advisory / mock → http://localhost:8760
./run_crypto_paper.sh        # Manual Decision + ETH/SOL + Gemma + public MD
```

See [`crypto/README.md`](crypto/README.md) and [`crypto/docs/`](crypto/docs/) for paper runbook, latency notes, and feed fields.

## Quote currency

GO card / Manual Decision instruments use Delta pairs: **BTCUSD · ETHUSD · SOLUSD**.

## Tests

```bash
python3 -m pytest -q tests/cryptocubera
```

## Disclaimer

Decision-support tooling, not financial advice. You confirm all decisions.
