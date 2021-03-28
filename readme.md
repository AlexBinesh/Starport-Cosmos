New API endpoint were added to provide additional Node info, such as:
1- List of All Nodes in the Network
2- Balance for each Node
3- Transfer Transacions For each Node

All the above is exposed in the Block Explorer associated with a Node, on port <NODE ADDRESS>:12345 
Additionally the above functionality can be accessed by invoking the APIs directly as per below:

curl -X POST <NODE ADDRESS>:10000/ -d "network=foo"  -d "operation=chains"

curl -X POST <NODE ADDRESS>:10000/ -d "network=foo"  -d "operation=balance" 

curl -X POST <NODE ADDRESS>:10000/ -d "network=foo" -d "limit=100"  -d "operation=txs"


# ![Starport](./assets/starport.jpg)

Starport is the easiest way to build a blockchain. It is a developer-friendly interface to the [Cosmos SDK](https://github.com/cosmos/cosmos-sdk), the world's most widely-used blockchain application framework. Starport generates boilerplate code for you, so you can focus on writing business logic.

* [**Build a blockchain with Starport in a web-based IDE** (stable)](https://gitpod.io/#https://github.com/tendermint/starport/tree/master) or use [nightly version](https://gitpod.io/#https://github.com/tendermint/starport/)
* [Check out the latest features in v0.15](https://www.youtube.com/watch?v=NmytpuD33lY)

## Quick start

Open Starport [in your browser](https://gitpod.io/#https://github.com/tendermint/starport/tree/master), or [install it](/docs/1%20Introduction/2%20Install.md). Then:

```
starport app github.com/foo/mychain

cd mychain

starport serve
```

## Documentation

To learn how to use Starport, check out the [Starport Documentation](/docs/README.md). To learn more about how to customize your blockchain see `config.yml` [reference](/docs/2%20Architecture/5%20Configuration.md). To install Starport locally on GNU/Linux or macOS, follow [these steps](/docs/1%20Introduction/2%20Install.md).

To learn more about building a JavaScript frontend for your Cosmos SDK blockchain, see [`tendermint/vue`](https://github.com/tendermint/vue).

## Questions

For questions and support please join the #starport channel in the [Cosmos Community Discord](https://discord.com/invite/W8trcGV). The issue list of this repo is exclusively for bug reports and feature requests.

## Contributing

We welcome contributions from everyone. The `develop` contains the development version. You can branch of from `develop` and create a pull request, or maintain your own fork and submit a cross-repository pull request. Thank you to all those who have contributed to Starport!

## Stay in touch

Starport is a free and open source product maintained by [Tendermint](https://tendermint.com). Follow us to get the latest updates!

- [Twitter](https://twitter.com/tendermint_team)
- [Blog](https://medium.com/tendermint)
- [Jobs](https://tendermint.com/careers)
