---
description: Learn how Gitcoin Passport's scores are calculated.
---

# 🤔 How is Gitcoin Passport’s score calculated?

The Passport score is calculated based on the data points verified in the participant's Passport. Each data point is assigned a specific weight, which is used to determine the Passport score.&#x20;

#### Passport Scoring Weights:

* BrightID: 0.802
* Civic
  * Holds a Civic CAPTCHA Pass: 1.014
  * Holds a Civic Uniqueness Pass: 6.005
  * Holds a Civic Liveness Pass: 3.004
* Coinbase: 16.042
* Discord: 0.516
* ENS: 0.408
* ETH
  * ETH Enthusiast: 10.012
  * ETH Advocate: 2.001
  * ETH Maxi: 2.009
  * Active on over 50 distinct days: 0.507
  * Execute over 100 transactions: 0.51
  * Spend more than 0.25 ETH on gas: 1.003
* Gitcoin Grants
  * Contributed at least $10: 0.523
  * Contributed at least $100: 2.017
  * Contributed at least $1000: 5.018
* Github
  * Contributions on at least 30 distinct days: 2.020
  * Contributions on at least 60 distinct days: 2.021
  * Contributions on at least 120 distinct days: 3.019
* Gnosis Safe: 0.822
* Google: 0.525
* GTC Staking
  * Beginner Community Staker: 1.513
  * Experienced Community Staker: 2.515
  * Trusted Citizen: 4.041
  * Self Staking Bronze: 1.036
  * Self Staking Gold: 3.037
  * Self Staking Silver: 2.038
* Guild
  * Owner or Administrator of one or more guilds: 0.724
  * Member with 1 or more roles in Gitcoin Passport Guild: 0.54
* Holonym: 16.026
* Idena
  * Idena Identity State - Human: 2.027
  * Idena Identity State - Newbie: 6.028
  * Idena Identity State - Verified: 2.029
* Lens Handle: 0.93
* Linkedin Account: 1.531
* NFT
  * NFT Holder: 0.71
  * Digital Collector: 10.033
  * Art Aficionado: 2.034
  * NFT Visionary: 2.035
* Snapshot
  * Created a DAO proposal that was voted on by at least 1 account: 0.839
* Trusta Labs: 0.511
* ZkSync
  * Verified Transactor: 0.606
  * Engagement Explorer: 1.67
  * Blockchain Believer: 1.67
  * zkSync Champion: 1.67\


The threshold for Gitcoin Passport Scoring is 20 and the maximum possible score is 100. We encourage all users to verify as many stamps as they can to increase their Passport Score but a score of 20 is sufficient.

_Note: Passport stamps will automatically expire 90 days after verification. You will need to re-verify Passport Stamps periodically._

The specific weights of all the data points are here:

{% embed url="https://github.com/gitcoinco/passport-scorer/blob/main/api/scorer/settings/gitcoin_passport_weights.py" %}
Gitcoin Passport Stamp Weights
{% endembed %}
