# 2023-dsrv-sarangbang-workshop
- https://docs.sui.io/testnet/build/fullnode
- https://github.com/MystenLabs/sui/tree/main/docker/fullnode#readme
- https://hub.docker.com/r/mysten/sui-node/tags

### docker-compose.yaml
```
wget https://raw.githubusercontent.com/MystenLabs/sui/main/docker/fullnode/docker-compose.yaml
```

### fullnode-template.yaml
```
wget https://github.com/MystenLabs/sui/raw/main/crates/sui-config/data/fullnode-template.yaml
```

### genesis.blob
- mainnet
```
wget https://github.com/MystenLabs/sui-genesis/raw/main/mainnet/genesis.blob
```
- testnet
```
wget https://github.com/MystenLabs/sui-genesis/raw/main/testnet/genesis.blob
```
- devnet
```
wget https://github.com/MystenLabs/sui-genesis/raw/main/devnet/genesis.blob
```

### Metrics
```
http://localhost:9184/metrics
```


### Test Query
```
curl localhost:9000 \
--request POST \
--header 'Content-Type: application/json' \
--data-raw '{ "jsonrpc":"2.0", "method":"rpc.discover","id":1}'
```
