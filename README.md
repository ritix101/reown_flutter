# **Reown - Flutter**

Reown is a communications protocol for web3 that brings the ecosystem together by enabling hundreds of wallets and apps to securely connect and interact. This repository contains the Flutter implementation of the WalletConnect protocol for Flutter applications.

## SDK Chart

| [Core SDK](packages/reown_core) | [Sign SDK](packages/reown_sign) | [WalletKit](packages/reown_walletkit) | [AppKit](packages/reown_appkit) |
|--------------------------|---------------------------|--------------------------------|--------------------------|
| 1.0.0                    | 1.0.0                     | 1.0.0                          | 1.0.0                    |

## License

Reown is released under the Apache 2.0 license. For more details, see the [LICENSE](/LICENSE).

### Generate Project Dependencies

To generate dependencies, run the following command in the root folder:

```bash
sh scripts/generate_all.sh


### Run WalletKit Sample

1. Run `cd packages/reown_walletkit/example`
2. Run `flutter run --dart-define=PROJECT_ID=0123... --flavor internal --debug`

You can add your own keys for testing purposes as follows:

--dart-define=ETH_SECRET_KEY=your mnemonic phrase....

--dart-define=KADENA_SECRET_KEY=5fgQC1.........

--dart-define=KADENA_ADDRESS=5fgQC1.........

--dart-define=SOLANA_SECRET_KEY=5fgQC1.........

--dart-define=SOLANA_ADDRESS=DbfmtKwL.........

--dart-define=POLKADOT_MNEMONIC=your mnemonic phrase....

--dart-define=POLKADOT_ADDRESS=DbfmtKwL.........


_NB: WalletKit sample is intended to be used just as an explanatory project_


### Run AppKit Sample

AppKit has two samples, `base`, which is made with `ReownAppKit` UI-less SDK, and `modal`, which is made with `ReownAppKitModal`

1. Run `cd packages/reown_appkit/example/base`
2. Run `flutter run --dart-define=PROJECT_ID=0123... --flavor internal --debug`

or

1. Run `cd packages/reown_appkit/example/modal`
2. Run `flutter run --dart-define=PROJECT_ID=0123... --debug`