# Changelog

All notable changes to this project will be documented in this file.
## [v1.2.4] - 2026-06-18

### Bug Fixes

- Something else

### Features

- Somehting

## [v1.2.3] - 2026-06-18

### Features

- (**node**) Removed somehting

### Refactor

- (**node**) Added it again
- (**node**) Remove tokio::task for axum (#802)

## [v1.2.1] - 2026-06-17

### Bug Fixes

- (**node**) Fixes a test-cases (#787)
- Oprf release process (#782)
- (**oprf-node**) Add humantime serde for ttl/tti config (#742)
- (**oprf-nodes**) Correctly constructs internal errors (#672)
- (**authenticator**) Normalize sparse indexer pubkey slots before key set validation (#447)
- Temporarily remove decompressed zkey disk caching (#431)
- Don't update oprf key id in RpRegistryWatcher (#416)
- OprfKeyId cannot be safely updated (#414)
- Fix crates release workflow (#381)
- Remove test contracts (#378)
- Update MerkleWatcher after fix of infinite validity window (#345)
- Add root validity window (time-to-live) to MerkleWatcher cache (#232)

### Features

- (**node**) Differentiate between unknown/invalid merkle root (#768)
- (**oprf-node**) Add tti for watchers + add auth_error event to logs (#741)
- (**oprf-node**) Use jemalloc as global allocator (#723)
- Support session proof generation (#712)
- (**oprf-nodes**) Added WIP101 support at the nodes (#634)
- Improve docs for OPRF errors (#606)
- (**oprf-node**) Add session route for OPRF (#596)
- Session proofs & rp signature (#547)
- Rust Proof Input verification with nicer errors (#338)
- Remove circuits feature flags on primitives crate (#425)
- Make world-id-signer wasm compatible (#383)
- Add OPRF request authentication tests (#350)
- Update taceo crates (#333)
- Update names of OPRF node auth modules and types for new OprfModule names (#332)
- Add OPRF module for credential blinding factor generation, rename old one to nullifier, integrate into authenticator (#293)
- Update taceo crates (#302)
- Align MerkleWatcher with WorldIdRegistry contract root valid validity check (#282)
- Split nullifier & proof generation (#278)
- Update taceo deps (#276)
- Add metrics for world-id-oprf-node (#259)
- New rp_signature module and include action (#243)
- Contract interface updates (#208)
- Use moka cache (#217)
- Integrate and update RpRegistry to load and verifiy ecdsa signature in oprf-node (#197)
- (**api**) Standardize success/error responses (#204)
- Update circuits, cred.id hashing & sub blinding factor (#162)

### Miscellaneous Tasks

- (**main**) Release world-id-oprf-node 1.2.1 (#792)
- (**world-id-oprf-node**) Release v1.2.0 (#776)
- Explicit oprf-node release (#726)
- Clp + recursion (#746)
- Bump alloy to 2.0.1 (#687)
- (**node**) Unset env variables on start (#681)
- Update docs & clarify around Authenticator management (#673)
- Introduce registries crate (#671)
- (**primitives**) Move circuit_inputs to world-id-proof (#667)
- Use default to create empty AuthenticatorPublicKeySet (#460)
- Add more tracing for world-oprf-node (#409)
- Consolidate deps (#354)
- Rust nits (#211)
- Use a docker hub token for CI (#207)
- Release 0.3.0 (#147)
- Cleanup build dependencies (#170)

### Performance

- (**signature-history**) Use lru cache (#231)
- (**merkle-watcher**) Use lru cache to store merkle roots (#230)

### Refactor

- (**node**) Small logging/metrics cleanup (#781)
- (**oprf**) Info for invalid merkle errors (#769)
- (**node**) Add retry logic for RPC requests + bump oprf deps (#764)
- (**oprf-node**) Updated metrics call; use telemetry-batteries (#724)
- Audit resutls oprf-node (#658)
- (**oprf-nodes**) Uses the nodes_common rpc provider over ws provider everywhere + removes AWS deps (#617)
- (**oprf-node**) Misc stuff for oprf-nodes (v1.1) (#608)
- (**nodes**) Add fine-grained error types for nodes (#585)
- Store nonces instead of signatures in OPRF node (#588)
- Removed auth counter metrics in OPRF (#418)
- Oprf-node main wraped into run function for tracing clarity (#396)
- Updated taceo deps and restructured binary to get actual errors (#359)

## [v0.1.0] - 2026-01-09

### Bug Fixes

- (**oprf-node**) Don't cache invalid roots (#169)

### Features

- Update oprf client workflow in authenticator, add oprf node, add justfile with setup (#129)

