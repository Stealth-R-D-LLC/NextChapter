# Stealth: The Next Chapter

**Private Payments, Final Settlement and Quantum Security**

📄 **[Read the whitepaper (PDF)](Stealth-NextChapter-Whitepaper.pdf)** ·
[Download the latest release](https://github.com/Stealth-R-D-LLC/NextChapter/releases/latest/download/Stealth-NextChapter-Whitepaper.pdf)

## Abstract

Stealth is a proof-of-stake cryptocurrency whose ordinary transactions need
no fee. This paper describes the new Stealth protocol, run by a node written
in Rust, and the two problems it answers. A public ledger exposes every
payment: anyone can read who paid whom and how much, for as long as the
ledger exists. And a large quantum computer breaks the signatures that
protect coins and the encryption that protects private data, while encrypted
data recorded today can be read once such a computer exists.

Stealth answers the first problem with a second chain beside the transparent
one: a shielded sidechain in which coins are notes that appear on the ledger
only as commitments, are spent by publishing markers that cannot be linked to
them, and move under zero-knowledge proofs that show a payment to be valid
without revealing its sender, its recipient or its amount. It answers the
second by building the shielded chain from hash-based proofs and post-quantum
encryption, by signing blocks and finality votes with post-quantum
signatures, and by letting holders of transparent coins protect them with a
spend that commits to its destination before it reveals its key. A committee
of stakers makes blocks final, and the chain itself holds the coins that
cross between the two chains, releasing them only against proof that their
shielded counterpart was destroyed. What follows is a payment system in which
a payment can be private, final and free of fees, and in which value held
privately stays confidential and unforgeable against an adversary with a
quantum computer. The same foundations carry a private messenger, a light
client that trusts no server and per-request payments by software agents.

## Contents

- **Part I. Introduction**
- **Part II. The Node**: the Rust node; one thread, one clock
- **Part III. Privacy and the Sidechain**: the XSS shielded sidechain; the sidechain architecture
- **Part IV. Security**: post-quantum security; BFT finality; consensus custody and the XST ↔ XSS bridge
- **Part V. Applications**: private messenger; commit-reveal ("enclave") addresses; the trustless light client; StealthPay and x402 agentic payments
- **Part VI. The Chain**: pruning; feework hardening and block space; microtx; the +100 StealthNodes
- **Part VII. Closing Remarks**

## Discussion

Questions, comments and errata are welcome in
[Issues](https://github.com/Stealth-R-D-LLC/NextChapter/issues).

## Related

- [Stealth](https://github.com/Stealth-R-D-LLC/Stealth): the Stealth
  node source code

## Disclaimer

This paper describes a protocol and is not investment advice. Anyone who uses
the Stealth protocol or its software does so at their own risk. Nothing in
this paper is a promise.

## License

This paper is licensed under the
[Creative Commons Attribution 4.0 International licence (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
