# Py-Block-Chain

A python block chain demo.

# Use

```bash
python3 blockchain.py
```

GET Mine: `curl http://127.0.0.1:5000/mine`

GET full chain: `curl http://127.0.0.1:5000/chain`

POST new transaction: 

```bash
curl -X POST -H "Content-Type: application/json" -d '{
    "sender": "<sender>",
    "recipient": "<recipient>",
    "amount": <amount>
}' "<node_url>/transactions/new"
```

POST resigster node: 

```bash
curl -X POST -H "Content-Type: application/json" -d '{
    "nodes": ["<node_url>"]
}' "<node_url>/nodes/register"
```

GET nodes resolve: `curl http://127.0.0.1:5000/nodes/resolve`

# Ref

[A blockchain in 200 lines of code](https://medium.com/@lhartikk/a-blockchain-in-200-lines-of-code-963cc1cc0e54)