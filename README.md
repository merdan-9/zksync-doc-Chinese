# zkSync：以太坊的扩展和隐私引擎

[![Logo](zkSyncLogo.svg)](https://zksync.io/)

[![Live on Mainnet](https://img.shields.io/badge/wallet-Live%20on%20Mainnet-blue)](https://wallet.zksync.io)
[![Live on Rinkeby](https://img.shields.io/badge/wallet-Live%20on%20Rinkeby-blue)](https://rinkeby.zksync.io)
[![Live on Ropsten](https://img.shields.io/badge/wallet-Live%20on%20Ropsten-blue)](https://ropsten.zksync.io)

zkSync is a scaling and privacy engine for Ethereum. Its current functionality scope includes low gas transfers of ETH and ERC20 tokens in the Ethereum network.

zkSync是以太坊的扩展和隐私引擎。它目前的功能范围包括在以太坊网络中以低gas费转移ETH和ERC20代币。

## Description 描述

zkSync is built on ZK Rollup architecture. ZK Rollup is an L2 scaling solution in which all funds are held by a smart contract on the mainchain, while computation and storage are performed off-chain. For every Rollup block, a state transition zero-knowledge proof (SNARK) is generated and verified by the mainchain contract. This SNARK includes the proof of the validity of every single transaction in the Rollup block. Additionally, the public data update for every block is published over the mainchain network in the cheap calldata.

zkSync建立在ZK Rollup架构上。ZK Rollup是一种L2扩展解决方案，在这种方案中，所有资金都由主链上的智能合约持有，而计算和存储则在链下执行。对于每个Rollup块，主链合约会生成并验证一个状态转换的零知识证明（SNARK）。此SNARK包括Rollup块中每个单独交易的有效性证明。此外，每个块的公共数据更新在主链网络上以便宜的calldata形式发布。

This architecture provides the following guarantees:

该架构提供以下保证：

- The Rollup validator(s) can never corrupt the state or steal funds (unlike Sidechains).
- Rollup验证器永远不能破坏状态或窃取资金（与侧链不同）。
- Users can always retrieve the funds from the Rollup even if validator(s) stop cooperating because the data is available (unlike Plasma).
- 即使验证器停止合作，用户也可以随时从Rollup中检索资金，因为数据是可用的（与Plasma不同）
- Thanks to validity proofs, neither users nor a single other trusted party needs to be online to monitor Rollup blocks  in order to prevent fraud.
- 由于有效性证明，为了防止欺诈，用户或单个其他受信任的方需要在线监视Rollup块。

In other words, ZK Rollup strictly inherits the security guarantees of the underlying L1.

换句话说，ZK Rollup严格继承了基础L1的安全保证。

To learn how to use zkSync, please refer to the [zkSync SDK documentation](https://zksync.io/api/sdk/).

要了解如何使用zkSync，请参阅[zkSync SDK文档](https://zksync.io/api/sdk/)。

## Development Documentation 开发文档

The following guides for developers are available:
下面向开发者的指南可供使用：

- Installing development dependencies: [docs/setup-dev.md](docs/setup-dev.md).
- Launching zkSync locally: [docs/launch.md](docs/launch.md).
- Development guide: [docs/development.md](docs/development.md).
- Repository architecture overview: [docs/architecture.md](docs/architecture.md).

## License

zkSync is distributed under the terms of both the MIT license and the Apache License (Version 2.0).

See [LICENSE-APACHE](LICENSE-APACHE), [LICENSE-MIT](LICENSE-MIT) for details.