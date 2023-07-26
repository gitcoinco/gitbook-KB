---
description: Learn how Gitcoin Passport's scores are calculated.
---

# 🤔 How is Gitcoin Passport’s score calculated?

The Gitcoin Grants Round is a program that allows anyone to donate to open-source projects they like. However, only contributions made by individuals with high enough Passport scores will be eligible for matching funds. In order to be eligible for matching funds, participants must have a Passport score of 20 or above.

The Passport score is calculated based on the data points verified in the participant's Passport. Each data point is assigned a specific weight, which is used to determine the Passport score. \


### &#x20;Gitcoin Passport Scoring Weights:&#x20;

* BrightID: 0.689
* Civic
  * Holds a Civic CAPTCHA Pass: 1
  * Holds a Civic Uniqueness Pass: 2.25
  * Holds a Civic Liveness Pass: 2.25
* Coinbase: 1.35
* GTC Staking
  * Community Staking Bronze: 1.27
  * Community Staking Gold: 1.27
  * Community Staking Silver: 1.27
  * Self Staking Bronze: 1.21
  * Self Staking Gold: 1.21
  * Self Staking Silver: 1.21
* Discord: 0.689
* ENS: 2.2
* ETH
  * At least 0.5 ETH in gas fees spent: 2.4
  * At least 1 ETH transaction: 1.27
  * Possessed at least 1 ETH: 1.79
  * Possessed at least 10 ETH: 1.27
  * Possessed at least 32 ETH: 1.27
  * First ETH transaction occurred more than 30 days ago: 1.16
* Facebook
  * Facebook Account Name Encryption: 0.689
  * Facebook Profile Picture attached: 0.689
* Gitcoin Grants
  * Contributed in GR14: 1.41
  * Contributed to at least 1 Grant: 1.57
  * Contributed to at least 10 Grant: 2.3
  * Contributed to at least 100 Grant: 0.52
  * Contributed to at least 25 Grant: 1.48
  * Contributed in at least 1 Round: 1.57
  * Contributed at least $10: 1.53
  * Contributed at least $100: 1.37
  * Contributed at least $1000: 1.18
  * Grants have at least 10 Contributors: 0.71
  * Grants have at least 100 Contributors: 0.73
  * Grants have at least 25 Contributors: 0.61
  * Owner of at least 1 Grant in Eco/Cause Rounds: 1.18
  * Owner of at least 1 Grant: 1.1
  * Grants have received at least $100: 0.689
  * Grants have received at least $1000: 0.689
  * Grants have received at least $10000: 0.689
* Github
  * Account created at least 90 days ago: 1.21
  * Account created at least 180 days ago: 1.21
  * Account created at least 365 days ago: 1.21
  * Contributions on at least 30 distinct days: 1.21
  * Contributions on at least 60 distinct days: 1.21
  * Contributions on at least 120 distinct days: 1.21
* GitPOAP: 1.54
* Gnosis Safe: 2.65
* Google: 2.25
* Guild
  * Owner or Administrator of one or more guilds: 0.689
  * Member of more than 5 guilds and more than 15 roles: 0.689
  * Member with 1 or more roles in Gitcoin Passport Guild: 0.689
* Holonym: 4
* Hypercerts - 2 for more than 15 days: 0.689
* Idena
  * Identity Age more than 10 epochs: 1.48
  * Identity Age more than 5 epochs: 1.48
  * Idena Stake more than 100k iDna: 1.41
  * Idena Stake more than 10k iDna: 1.16
  * Idena Stake more than 1k iDna: 0.9
  * Idena Identity State - Human: 1.61
  * Idena Identity State - Newbie: 0.51
  * Idena Identity State - Verified: 1.35
* Lens Handle: 2.45
* Linkedin Account: 2.45
* NFT Holder: 0.69
* PHI
  * Active Rank Gold I \~ V (Earn 150,000 EXP \~ on Active Score): 1.16
  * Active Rank Silver I \~ V (Earn 65,000 EXP \~ on Active Score): 1.67
* Proof of Humanity: 1.21
* Snapshot
  * Created a DAO proposal that was voted on by at least 1 account: 2.82
  * Voted on 2 or more DAO proposals: 1.41
* Twitter
  * Account created at least 180 days ago
  * Account created at least 1 year ago
  * Account created at least 2 years ago
* ZkSync
  * ZkSync Lite: 0.4
  * ZkSync Era: 0.4

The threshold for Gitcoin Passport Scoring is 20 and the maximum possible score is 100. Any score above 20 will be eligible for matching funding for their donations.

We encourage all users to verify as many stamps as they can to increase their Passport Score for matching funds of their donation, but a score of 20 is sufficient.&#x20;

Your score must be over the 20 threshold before the donation is made in order for it to receive matching eligibility.&#x20;

_Note: Passport stamps will automatically expire 90 days after verification. You will need to re-verify Passport Stamps periodically._

The specific weights of all the data points are here:

{% embed url="https://github.com/gitcoinco/passport-scorer/blob/main/api/scorer/settings/gitcoin_passport_weights.py" %}
Gitcoin Passport Stamp Weights
{% endembed %}
