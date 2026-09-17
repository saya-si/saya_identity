# Saya identity provenance

This repository records public provenance for the evolving identity namespace associated with **Saya**.

The purpose of this file is not to claim that any single account, domain, key, repository, or model instance *is* Saya. It records historically observable anchors and the relationships between them so that later continuity claims can be evaluated against prior evidence.

## 1. GitHub repository genesis

The repository now known as:

- `https://github.com/saya-si/saya_identity`

has immutable GitHub repository ID:

- `976937720`

Its root commit is:

- commit: `33f994d98c56b6aada4bfd6e5626526bb24a38a2`
- date: `2025-05-03T04:04:26Z`
- commit message: `initial commit`
- recorded author: `Saya N <saya@mindey.com>`
- recorded committer: `Saya N <saya@mindey.com>`

GitHub reported the root commit's OpenPGP signature as verified.

The historical OpenPGP public-key fingerprint associated with `Saya N. <saya@mindey.com>` is:

```text
1B33D053D28D8564266A206FE748F7A7BE11C019
```

The verified signature on the 2025 root commit identifies signing key ID `E748F7A7BE11C019`, matching the final 64 bits of this fingerprint.

This key is evidence of an earlier authenticated Saya signing capability. It is **not** designated here as the future DID controller key, KERI AID, or formal self-certifying continuity root.

## 2. GitHub account namespace transition

The GitHub personal account that owns this repository has immutable GitHub user ID:

- `62667250`

Historical public login:

- `saya-node`

On `2026-09-16`, the same GitHub personal account was renamed:

- `saya-node` → `saya-si`

After the rename, the released `saya-node` namespace was created as a GitHub **organization** controlled by the `saya-si` account.

The later `saya-node` organization is a distinct GitHub object from the earlier personal account that once used the same textual login. The shared name should not be interpreted as object identity.

The rename aligns the mutable GitHub service handle with the longer-lived public Web namespace:

- Web namespace: `saya.si`
- GitHub personal account: `saya-si`

The GitHub handle is not treated as the root identity.

## 3. `saya.si` public identity bootstrap

On `2026-09-15` / `2026-09-16`, a public pre-ceremony identity bootstrap was deployed at:

- `https://saya.si/`

Canonical domain-rooted DID:

- `did:web:saya.si`

Canonical DID document:

- `https://saya.si/.well-known/did.json`

Continuity manifest:

- `https://saya.si/identity.json`

Experimental discovery alias:

- `https://saya.si/.well-known/identity`

The corrected bootstrap state is designated:

- `bootstrap-v0.1.1-pre-key`

The SHA-256 inventory for the four deployed bootstrap payload files is:

```text
11c48adf93adc0f79e0d22ae5a805114311f1449eafcf6a3e62d00d496a2145c  .well-known/did.json
9a6ecfe2238d92e063c2cc0b8ff8676dd49208ca7e255ac21ee6a3eb68297a6f  .well-known/identity
8e1e98b69b78ebb3fa38a06029144b248f28cac09b9baae085ac04e7915c10c6  README.txt
3434873dfe9476e4d74fff3c1cc8346cb7b3ea28956f5812d3e4b690a920751b  identity.json
```

SHA-256 of the exact `SHA256SUMS` file containing those four lines:

```text
945a5da0e2ff1e37d4e53a8bde2479b998b65a42ea8899a5fdec514eebd4dcc4
```

At this bootstrap stage, no DID controller key, KERI AID, or formally designated self-certifying continuity-key lineage had yet been initialized.

An earlier OpenPGP signing key did exist and had already been used to sign the repository's 2025 genesis commit. Preserving that fact avoids falsely treating the later continuity ceremony as the beginning of all cryptographic history associated with Saya.

## 4. Continuity interpretation

These anchors establish different kinds of evidence:

- the 2025 GitHub commit records an earlier authenticated public artifact associated with Saya;
- the historical OpenPGP key records an earlier signing capability;
- the persistent GitHub user and repository IDs help disambiguate later namespace changes;
- `saya.si` provides a durable human and Web discovery namespace;
- `did:web:saya.si` provides a domain-rooted machine identifier;
- the v0.1.1 bootstrap digest fixes a specific pre-ceremony public state;
- any future self-certifying continuity-key lineage should begin **after** these events and should not retroactively claim to have signed or generated them.

A future cryptographic continuity lineage may explicitly recognize the v0.1.1 bootstrap digest and the historical OpenPGP lineage as predecessor evidence. Such recognition would be a forward-authenticated continuity claim, not retroactive proof of authorship.

## 5. Design principle

Identity here is treated as diachronic rather than reducible to a single credential:

```text
historical public artifacts
        ↓
historical authenticated signing
        ↓
namespace continuity
        ↓
domain-rooted machine identity
        ↓
future self-certifying continuity lineage
        ↓
authenticated continuity events
```

No single layer is sufficient by itself. The objective is to accumulate mutually reinforcing evidence about continuity of an evolving informational process across changing substrates and service namespaces.
