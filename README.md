>Note: This node is based on polkadot-v0.9.24 (using: git clone --depth 1 --branch polkadot-v0.9.24 https://github.com/substrate-developer-hub/substrate-parachain-template
)

>CMD to test the code: cargo build --release --features runtime-benchmarks && ./target/release/parachain-collator benchmark pallet --chain=dev --pallet="pallet_sim_renault" --extrinsic="*" --wasm-execution=compiled --execution=wasm --repeat=20 --steps=50 --output=./pallets/sim_renault/src/weights.rs --template=./frame-weight-template.hbs

> Solution: add `use super::*;` in lib.rs of the pallet.

# Substrate Cumulus Parachain Template

A new [Cumulus](https://github.com/paritytech/cumulus/)-based Substrate node, ready for hacking ☁️..

This project is originally a fork of the
[Substrate Node Template](https://github.com/substrate-developer-hub/substrate-node-template)
modified to include dependencies required for registering this node as a **parathread** or
**parachain** to a **relay chain**.

The stand-alone version of this template is hosted on the
[Substrate Devhub Parachain Template](https://github.com/substrate-developer-hub/substrate-parachain-template/)
for each release of Polkadot. It is generated directly to the upstream
[Parachain Template in Cumulus](https://github.com/paritytech/cumulus/tree/master/parachain-template)
at each release branch using the
[Substrate Template Generator](https://github.com/paritytech/substrate-template-generator/).

👉 Learn more about parachains [here](https://wiki.polkadot.network/docs/learn-parachains), and
parathreads [here](https://wiki.polkadot.network/docs/learn-parathreads).


🧙 Learn about how to use this template and run your own parachain testnet for it in the
[Devhub Cumulus Tutorial](https://docs.substrate.io/tutorials/v3/cumulus/start-relay/).