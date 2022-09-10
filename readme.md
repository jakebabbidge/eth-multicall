# eth-multicall
Multicall Contract Based On MakerDAO Multicall To Handle Invalid Target Addresses Gracefully

## Difference between MakerDAO Multicall
The multicall contract allows web clients / blockchain ingestion systems to query multiple read-only `eth_call`'s in a single request, **where the validity of the target address is not known ahead of time**.

Rather than failing the whole multicall if one address is invalid (as MakerDAO Multicall does), `Multicall` will simply return no result for that specific call.

## Usage
This multicall contract will work on any chain using the Ethereum Virtual Machine (EVM)

## Attributions
The multicall contract is based on and heavily reuses code from [MakerDAO Multicall](https://github.com/makerdao/multicall)