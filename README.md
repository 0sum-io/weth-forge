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
export NATIVE_CURRENCY_LABEL="ETH"


forge create src/Contract.sol:WETH9 \
--private-key $PRIVATE_KEY \
--rpc-url $RPC_URL \
--priority-gas-price 8 \
--constructor-args "Wrapped $NATIVE_CURRENCY_LABEL" "W$NATIVE_CURRENCY_LABEL"
```

