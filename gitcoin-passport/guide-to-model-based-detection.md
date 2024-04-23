# Guide to Model-Based Detection

As part of our ongoing commitment to both enhancing security and reducing user friction within the identity verification processes of our partners, we have introduced an innovative feature: Model-Based Detection. This system seamlessly determines whether Ethereum addresses are likely controlled by humans or automated bots, known as Sybil entities, without requiring any user interaction.

## What is Model-Based Detection?

This verification method utilizes a variety of models to analyze the historical transactions associated with an Ethereum address. Initially, the system assigns scores ranging from 0 to 100 based on transaction activities to assess whether an address is more likely controlled by a human or a Sybil entity. For example, the first model deployed, known as the ETH Activity Model, specifically examines a user's Level 1 (L1) Ethereum transaction history.

## How It Impacts You

1. **Scoring System**: When you interact with a program or dApp that integrate this feature, your Ethereum address is automatically scored based on past and current activities. This reduces the need for user engagement in Passport as we have confidence they are real humans.
2. **Access Control:** The score could affect your access to various features or programs. A higher score generally means fewer restrictions and smoother access, while a lower score might limit certain activities or require additional verification steps. For users with low MBD scores, earning stamps in the Passport UX will offer an alternative to proving one's unique humanity. \*Note: not all Passport integrations use both the MBD and the Unique Humanity Score\*

## Benefits for Users

1. **Improved Security:** This model-based approach helps to prevent fraudulent activities and reduces the risks associated with Sybil attacks in the apps you use, enhancing the overall safety of the ecosystem.
2. **Enhanced Inclusion:** Active users benefit from a hassle-free experience where their regular engagement automatically improves their access to features. This system acknowledges their dedication effortlessly, requiring no extra steps from the users themselves.

## What You Need to Know

1. **Automatic Process:** The verification is automatic, requiring no active participation from you. Your Ethereum address is evaluated whenever you interact with supported dApps.
2. **Influence on User Experience:** Be aware that your score could influence how you are able to engage with certain features within the dApp ecosystem. High scores facilitate easier access, while lower scores might necessitate additional steps to verify your identity.

The Ethereum Model-Based Detection is a significant step forward in securing and streamlining user interactions within the Ethereum dApp space. By understanding and being aware of how your activities influence your score, you can enhance your experience across various platforms.
