# BYOAI Corp.

Open, verifiable building blocks for AI work. Everything published here is sealed: each release
carries `MANIFEST.sha256` and a signed `RECEIPT.json`, and anyone can check it with
[byoai-corp/verify](https://github.com/byoai-corp/verify).

| Repository | What it is | Licence |
|---|---|---|
| [skills](https://github.com/byoai-corp/skills) | Agent skills for building software with AI | MIT |
| [dictionary](https://github.com/byoai-corp/dictionary) | The AI coding dictionary, in BYOAI's own words | CC BY 4.0 |
| [verify](https://github.com/byoai-corp/verify) | The open checker for every BYOAI release | Apache-2.0 |

## BYOAI release key

```
bb1de39b94a44708e3abf583a9689fa3658e247ff7dbd96703f0c216ab8e7154
```

This is the Ed25519 key every BYOAI release is signed with. A repository's `BYOAI_RELEASE_PUBKEY`
must match it; if it does not, do not trust that copy.

```bash
cargo install --locked --git https://github.com/byoai-corp/verify byoai-release
byoai-release verify . --pubkey bb1de39b94a44708e3abf583a9689fa3658e247ff7dbd96703f0c216ab8e7154
```
