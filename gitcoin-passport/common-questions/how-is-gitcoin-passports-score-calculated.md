---
description: Learn how Gitcoin Passport's scores are calculated.
---

# 🤔 How is Gitcoin Passport’s score calculated?

The Gitcoin Grants Round is a program that allows anyone to donate to open-source projects they like. However, only contributions made by individuals with high enough Passport scores will be eligible for matching funds. In order to be eligible for matching funds, participants must have a Passport score of 21.8 or above.

The Passport score is calculated based on the data points verified in the participant's Passport. Each data point is assigned a specific weight, which is used to determine the Passport score. \


### &#x20;Gitcoin Passport Scoring Weights:&#x20;

* BrightID: 1.6
* GTC Staking
  * Self Staking Bronze: 2.67
  * Self Staking Silver: 0.56
  * Self Staking Gold: 1.5
  * Community GTC Staking Bronze: 2.6
  * Community GTC Staking Silver: 2.2
  * Community GTC Staking Gold: 1.8
* Discord: 1.6
* ENS: 1.7
* ETH
  * Possessed at least 1 ETH: 1.7
  * Possessed at least 10 ETH: 2.7
  * Possessed at least 32 ETH: 1.6
  * First ETH transaction occurred more than 30 days ago: 1.6
  * At least .5 ETH in gas fees spent:&#x20;
* Facebook
  * Facebook Account Name Encryption: 1.6
  * Facebook Friends Greater than 100:&#x20;
  * Facebook Profile Picture attached: 1.6
* GitHub
  * GitHub account: 1.6
  * Five or more GitHub Repos: 1.7
  * At least 1 GitHub repo forked by another user: 1.7
  * At least 1 Github rep starred by another user: 1.8
  * Ten or more GitHub followers: 1.6
  * Fifty or more GitHub followers: 1.5
* GitPOAP: 2.8
* Gitcoin Grants
  * Contributed to at least 1 Grant: 1.6
  * Contributed to at least 10 Grant: 1.6
  * Contributed to at least 25 Grant: 1.5
  * Contributed to at least 100 Grant: 1.5
  * Contributed to at least $10: 1.7
  * Contributed to at least $100: 1.6
  * Contributed to at least $1000: 1.9
  * Contributed in GR14: 1.7
  * Contributed in at least 1 Round: 1.6
  * Owner of at least 1 Grant: 2.7
  * Grants have at least 10 Contributors: 1.9
  * Grants have at least 25 Contributors: 2.2
  * Grants have at least 100 Contributors: 2.3
  * Grants have received at least $100: 2.5
  * Grants have received at least $1000: 0.07
  * Grants have received at least $10000: 0.5
  * Owner of at least 1 Grant in Eco/Cause Rounds: 2.7
* Gnosis Safe: 1.6
* Google Account: 1.6
* Lens Handle: 1.7
* Linkedin Account: 1.7
* NFT Holder: 1.6
* POAP owned for over 15 days: 1.6
* Proof of Humanity: 1.7
* Snapshot
  * Snapshot Voter: 1.7
  * Snapshot Proposal Creator: 1.6
* Twitter
  * Twitter Account: 1.7
  * More than 10 Tweets: 1.6
  * More than 100 Followers: 1.6
  * More than 500 Followers: 1.6
  * More than 1000 Followers: 1.7
  * More than 5000 Followers: 1.6
* ZkSync: 1.6
*   GTC

    * Possessed 10 GTC: 1.6
    * Possessed 100 GTC: 1.7



The threshold for Gitcoin Passport Scoring is 21.76 and the maximum possible score is 100. Any score above 21.76 will be eligible for matching funding for their donations.

We encourage all users to verify as many stamps as they can to increase their Passport Score for matching funds of their donation, but a score of 21.76 is sufficient.&#x20;

Your score must be over the 21.76 threshold before the donation is made in order for it to receive matching eligibility.&#x20;

The specific weights of all the data points are here:

{% embed url="https://github.com/gitcoinco/passport-scorer/blob/main/api/scorer/settings/gitcoin_passport_weights.py" %}
Gitcoin Passport Stamp Weights
{% endembed %}
