![Alt text](/candid-ui.png?raw=true "Candid UI")

## `token_transfer_backend`

I have adapted this project from the examples provided [here](https://github.com/dfinity/examples/tree/master/motoko/token_transfer) for my learning.

To learn more before you start working with `token_transfer`, see the following documentation available online:

- [Quick Start](https://internetcomputer.org/docs/current/developer-docs/setup/deploy-locally)
- [SDK Developer Tools](https://internetcomputer.org/docs/current/developer-docs/setup/install)
- [Motoko Programming Language Guide](https://internetcomputer.org/docs/current/motoko/main/motoko)
- [Motoko Language Quick Reference](https://internetcomputer.org/docs/current/motoko/main/language-manual)

If you want to start working on your project right away, you might want to try the following commands:

```bash
cd token_transfer_backend/
dfx help
dfx canister --help
```

## Running the project locally

If you want to test your project locally, you can use the following commands:

```bash
# Starts the replica, running in the background
dfx start --background

# Deploys your canisters to the replica and generates your candid interface
dfx deploy
```

Once the job completes, your application will be available at `http://localhost:4943?canisterId={asset_canister_id}`.

If you have made changes to your backend canister, you can generate a new candid interface with

```bash
npm run generate
```

at any time. This is recommended before starting the frontend development server, and will be run automatically any time you run `dfx deploy`.

If you are making frontend changes, you can start a development server with

```bash
npm start
```

Which will start a server at `http://localhost:8080`, proxying API requests to the replica at port 4943.

### Interact with this canister on ICP mainnet

#### canister ID: 
7lxqp-sqaaa-aaaak-qimfa-cai

````bash
URLs:
  Backend canister via Candid interface:
    icrc1_ledger_canister: https://a4gq6-oaaaa-aaaab-qaa4q-cai.raw.icp0.io/?id=7cu3t-eyaaa-aaaak-qimeq-cai
    token_transfer_backend: https://a4gq6-oaaaa-aaaab-qaa4q-cai.raw.icp0.io/?id=7lxqp-sqaaa-aaaak-qimfa-cai
```
