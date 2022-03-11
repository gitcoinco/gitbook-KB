# How do you prevent Sybil attacks?

**1. We use aged Github accounts, SMS verification, BrightID, a few other undisclosed vectors, and \(soon\) Idena Network/ other DID solutions, as an identity solution for Gitcoin Grant contributions. Check out the trust tab of your profile to increase your trust level.**

**2. In addition to Github's native anti-sybil technology, we programmatically check these accounts for signs of Sybil attacks. Each contribution is assigned a trust score according to the likelihood that it's part of a Sybil attack. Right now we do not take any action against Sybil attacks \(other than the most egregious cases\), but we are quietly collecting data to use in the future.**

**3. We use Vitalik Buterin's pairwise bonding formula to dampen Sybil attacks**

{% embed url="https://ethresear.ch/t/pairwise-coordination-subsidies-a-new-quadratic-funding-design/5553" %}

**More on our anti-sybil growth strategy here:**

{% embed url="https://twitter.com/owocki/status/1273458452900151296" %}

