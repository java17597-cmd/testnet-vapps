🎯 Goal

Enable users to prove eligibility/identity (e.g. DAO member, token holder, testnet participant) without revealing personal data.


---

🔧 Components

ZK Circuit (Circom): proves user’s address or credential is in an allowlist (Merkle proof).

Smart Contracts:

IdentityRegistry → stores commitments / Merkle root.

Verifier → checks zk-SNARK proof.


Frontend: connect wallet, generate proof, submit proof to claim access.



---

🌀 Flow

1. Admin builds an allowlist (token holders, addresses, roles).


2. User generates ZK proof → “I’m in the allowlist” without revealing which entry.


3. Contract verifies proof → grants access (e.g. mint pass, join testnet, claim reward).




---

✅ Success Criteria

Eligibility proven privately.

No leaking of wallet, balance, or role.

Simple demo: user connects wallet → proves eligibility → unlocks gated action.
