---
description: Learn how Gitcoin Passport's scores are calculated.
---

# 🤔 How is Gitcoin Passport’s score calculated?

The Gitcoin Grants Round is a program that allows anyone to donate to open-source projects they like. However, only contributions made by individuals with high enough Passport scores will be eligible for matching funds. In order to be eligible for matching funds, participants must have a Passport score of 15 or above.

The Passport score is calculated based on the data points verified in the participant's Passport. Each data point is assigned a specific weight, which is used to determine the Passport score. \


### &#x20;Gitcoin Passport Scoring Weights:&#x20;

* BrightID: 0
* GTC Staking
  * Self Staking Bronze: 2.78
  * Self Staking Silver: 0.58
  * Self Staking Gold: 1.56
  * Community GTC Staking Bronze: 2.29
  * Community GTC Staking Silver: 0.83
  * Community GTC Staking Gold: 0.83
* Discord: 1.67
* Coinbase: 1.67
* ENS: 2.4
* ETH
  * Possessed at least 1 ETH: 1.77
  * Possessed at least 10 ETH: 2.81
  * Possessed at least 32 ETH: 1.04
  * First ETH transaction occurred more than 30 days ago: 1.6
  * At least .5 ETH in gas fees spent: 1.56
* Facebook
  * Facebook Account Name Encryption: 0.52
  * Facebook Friends Greater than 100: 0.83
  * Facebook Profile Picture attached: 0.83
* GitHub
  * GitHub account: 0.52
  * Five or more GitHub Repos: 1.77
  * At least 1 GitHub repo forked by another user: 1.77
  * At least 1 Github rep starred by another user: 1.8
  * Ten or more GitHub followers: 2.4
  * Fifty or more GitHub followers: 3.12
* GitPOAP: 2.92
* Gitcoin Grants
  * Contributed to at least 1 Grant: 1.67
  * Contributed to at least 10 Grant: 1.67
  * Contributed to at least 25 Grant: 1.5
  * Contributed to at least 100 Grant: 1.67
  * Contributed to at least $10: 1.7
  * Contributed to at least $100: 2.6
  * Contributed to at least $1000: 1.04
  * Contributed in GR14: 1.77
  * Contributed in at least 1 Round: 1.6
  * Owner of at least 1 Grant: 2.81
  * Grants have at least 10 Contributors: 1.98
  * Grants have at least 25 Contributors: 2.29
  * Grants have at least 100 Contributors: 2.4
  * Grants have received at least $100: 2.5
  * Grants have received at least $1000: 1.98
  * Grants have received at least $10000: 0.52
  * Owner of at least 1 Grant in Eco/Cause Rounds: 3.44
* Gnosis Safe: 1.67
* Google Account: 1.67
* Lens Handle: 1.77
* Linkedin Account: 1.77
* NFT Holder: 1.67
* POAP owned for over 15 days: 1.67
* Proof of Humanity: 1.77
* Snapshot
  * Snapshot Voter: 1.77
  * Snapshot Proposal Creator: 1.67
* Twitter
  * Twitter Account: 0.52
  * More than 10 Tweets: 1.67
  * More than 100 Followers: 1.67
  * More than 500 Followers: 1.67
  * More than 1000 Followers: 1.77
  * More than 5000 Followers: 0
* ZkSync
  * ZkSyncLite: 0.835
  * ZkSyncEra: 0.835
* GTC
  * Possessed 10 GTC: 1.67
  * Possessed 100 GTC: 1.77

The threshold for Gitcoin Passport Scoring is 15 and the maximum possible score is 100. Any score above 15 will be eligible for matching funding for their donations.

We encourage all users to verify as many stamps as they can to increase their Passport Score for matching funds of their donation, but a score of 15 is sufficient.&#x20;

Your score must be over the 15 threshold before the donation is made in order for it to receive matching eligibility.&#x20;

_Note: Passport stamps will automatically expire 90 days after verification. You will need to re-verify Passport Stamps periodically._

The specific weights of all the data points are here:

{% embed url="https://github.com/gitcoinco/passport-scorer/blob/main/api/scorer/settings/gitcoin_passport_weights.py" %}
Gitcoin Passport Stamp Weights
{% endembed %}
