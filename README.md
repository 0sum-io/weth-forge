## WETH Forge 

# Install forge

```
curl -L https://foundry.paradigm.xyz | bash
```

# Build

```
forge build
```

# Deploy

```
RPC_URL=""
PRIVATE_KEY=""

forge create --rpc-url $RPC_URL --private-key $PRIVATE_KEY src/Contract.sol:WETH9
```

