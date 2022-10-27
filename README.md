# WorldCupChain Swap Interface

An open source interface for WorldCupChain Swap -- a protocol for decentralized exchange of ERC20 tokens.

- Website: [worldcupchain.com](https://worldcupchain.com/)
- Interface: [swap.worldcupchain.com](https://swap.worldcupchain.com)
- Docs: [docs.worldcupchain.com](https://docs.worldcupchain.com)

## Listing a token

Please see the
[@worldcupchain/default-token-list](https://github.com/worldcupchain/default-token-list) 
repository.

## Development

### Install Dependencies

```bash
yarn
```

### Run

```bash
yarn start
```

### Configuring the environment (optional)

To have the interface default to a different network when a wallet is not connected:

1. Make a copy of `.env` named `.env.local`
2. Change `REACT_APP_NETWORK_ID` to `"{YOUR_NETWORK_ID}"`
3. Change `REACT_APP_NETWORK_URL` to e.g. `"https://{YOUR_NETWORK_ID}.infura.io/v3/{YOUR_INFURA_KEY}"` 

Note that the interface only works on testnets where both 
[worldcupchain V2](https://worldcupchain.org/docs/v2/smart-contracts/factory/) and 
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.** 
CI checks will run against all PRs.

## Accessing worldcupchain Interface V1

The worldcupchain Interface supports swapping against, and migrating or removing liquidity from worldcupchain V1. However,
if you would like to use worldcupchain V1, the worldcupchain V1 interface for mainnet and testnets is accessible via IPFS gateways 
linked from the [v1.0.0 release](https://github.com/worldcupchain/worldcupchain-interface/releases/tag/v1.0.0).
