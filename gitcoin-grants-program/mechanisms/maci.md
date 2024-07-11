# MACI

#### Minimal Anti-Collusion Infrastructure (MACI)

Vitalik's[ high-profile concern](https://vitalik.eth.limo/general/2021/05/25/voting2.html) on the shortcomings of voting systems, both traditional and digital, has helped drive interest in cryptography-native mechanisms. A zero-knowledge based system titled Minimum Anti-Collusion Infrastructure (MACI) was created in [this blog post](https://ethresear.ch/t/minimal-anti-collusion-infrastructure/5413) and serves as the basis for this mechanism.

> “MACI is an Ethereum application that provides privacy and collusion resistance for on-chain voting, both in a quadratic and non-quadratic fashion. A common problem among today’s on-chain voting (or public good funding) processes is how easy it is to bribe voters into voting for a particular option. MACI \[uses] encryption and zero-knowledge proofs (zk-SNARKs) to hide how each person voted while still publicly revealing the final result.” - [Welcome to MACI](https://maci.pse.dev/docs/introduction)

MACI works as a modification to a typical [QF](quadratic-funding.md) round. Some mechanisms previously used to help shape incentives hold reduced relevance, and new mechanisms exist to deliver unique opportunities to communities.

#### Allow List

A round’s `allowlist` is a feature that gives advantage to certain participants, known as allowlisted members. This can be based on badgeholding, [verifiable event attendance](https://medium.com/@morphlayer2/zuzalu-passport-with-attribute-based-signature-abs-2e8e979a553b), or some other property.

Maximum round contribution limits can be set for the general public and allowlist users separately. This can mean raised donation limits for the allowlist - or in the case of a $0 limit for the general public, complete exclusivity in participation.

#### Differences to Conventional QF

A matching cap is typically employed by a QF round to ensure one grantee is not afforded too large a share of the matching pool. In MACI it is not technically feasible to implement this. However, with low contribution limits, it becomes more difficult for a single project to receive a large portion of the matching pool.

The post-round analytics common to a conventional QF round are also challenged by MACI - only the coordinator can tally the votes, prove the correctness of the results, and publish the results.&#x20;

#### Round Coordinator

The round coordinator may be an individual or an organization, and exists as the only point of trust in the entire round process. Using a generated private key the round coordinator creates zk-proofs verifiable on-chain. The coordinator can decrypt the MACI-private donations (votes), but not modify or remove them.&#x20;

#### Donations/Voting

When a round is live, participants can add projects to their cart following the typical Grants Stack flow. **A donation can only be made once per round**, after which the donor will receive spendable votes proportional to their contribution. These can be distributed among as many projects as desired, and can be changed later.&#x20;

**Ending a round**

At the conclusion of the round, the coordinator will be responsible for tallying the results and proving their correctness using zk-SNARK technology.

\
