---
description: Learn how Gitcoin Passport's scores are calculated.
---

# 🤔 How is Gitcoin Passport’s score calculated?

The Gitcoin Grants Round is a program that allows anyone to donate to open-source projects they like. However, only contributions made by individuals with high enough Passport scores will be eligible for matching funds. In order to be eligible for matching funds, participants must have a Passport score of 15 or above.

The Passport score is calculated based on the data points verified in the participant's Passport. Each data point is assigned a specific weight, which is used to determine the Passport score. \


### &#x20;Gitcoin Passport Scoring Weights:&#x20;

* BrightID: 0.71
* Civic
  * Holds a Civic CAPTCHA Pass: 0.51
  * Holds a Civic Uniqueness Pass: 3.29
  * Holds a Civic Liveness Pass: 2.27
* Coinbase: 1.37
* CyberConnect
  * Premium CyberProfile Handle (length is between 1 and 6 characters): 1.23
  * Paid CyberProfile Handle (length is between 7 and 12 characters): 1.23
  * Organization Membership: 1.23
* Discord: 0.71
* ENS: 2.2
* ETH
  * ETH Enthusiast: 2.65
  * ETH Advocate: 2.65
  * ETH Maxi: 2.65
  * ETH Pioneer: 2.65
  * ETH Maxi: 2.65
* Gitcoin Grants
  * Contributed to at least 1 Grant: 2.93
  * Contributed to at least 10 Grant: 3.66
  * Contributed to at least 100 Grant: 1.88
  * Contributed to at least 25 Grant: 2.84
  * Contributed at least $10: 2.94
  * Contributed at least $100: 2.73
  * Contributed at least $1000: 2.54
* Github
  * Account created at least 90 days ago: 1.02
  * Account created at least 180 days ago: 1.23
  * Account created at least 365 days ago: 1.43
  * Contributions on at least 30 distinct days: 1.23
  * Contributions on at least 60 distinct days: 1.23
  * Contributions on at least 120 distinct days: 1.23
* Gnosis Safe: 2.67
* Google: 1.03
* GTC Staking
  * Beginner Community Staker: 1.29
  * Experienced Community Staker: 1.29
  * Trusted Citizen: 1.29
  * Self Staking Bronze: 1.23
  * Self Staking Gold: 1.23
  * Self Staking Silver: 1.23
* Guild
  * Owner or Administrator of one or more guilds: 0.71
  * Member of more than 5 guilds and more than 15 roles: 0.71
  * Member with 1 or more roles in Gitcoin Passport Guild: 0.71
* Holonym: 5.04
* Idena
  * Identity Age more than 10 epochs: 1.5
  * Identity Age more than 5 epochs: 1.5
  * Idena Stake more than 100k iDna: 1.43
  * Idena Stake more than 10k iDna: 1.18
  * Idena Stake more than 1k iDna: 0.92
  * Idena Identity State - Human: 1.63
  * Idena Identity State - Newbie: 0.53
  * Idena Identity State - Verified: 1.37
* Lens Handle: 2.47
* Linkedin Account: 1.04
* NFT Holder: 0.71
* PHI
  * Active Rank Gold I \~ V (Earn 150,000 EXP \~ on Active Score): 1.18
  * Active Rank Silver I \~ V (Earn 65,000 EXP \~ on Active Score): 1.69
* Proof of Humanity: 1.23
* Snapshot
  * Created a DAO proposal that was voted on by at least 1 account: 2.84
  * Voted on 2 or more DAO proposals: 1.43
* Trusta Labs: 2.02
* Twitter
  * Account created at least 180 days ago: 1.02
  * Account created at least 1 year ago: 1.23
  * Account created at least 2 years ago: 1.43
* ZkSync
  * ZkSync Lite: 0.42
  * ZkSync Era: 0.42

The threshold for Gitcoin Passport Scoring is 15 and the maximum possible score is 100. Any score above 15 will be eligible for matching funding for their donations.

We encourage all users to verify as many stamps as they can to increase their Passport Score for matching funds of their donation, but a score of 15 is sufficient.&#x20;

Your score must be over the 15 threshold before the donation is made in order for it to receive matching eligibility. See [Passport Sliding Scale on Grants Stack](../../gitcoin-grants-program/passport-sliding-scale-on-grants-stack.md) for more information.

_Note: Passport stamps will automatically expire 90 days after verification. You will need to re-verify Passport Stamps periodically._

The specific weights of all the data points are here:

{% embed url="https://github.com/gitcoinco/passport-scorer/blob/main/api/scorer/settings/gitcoin_passport_weights.py" %}
Gitcoin Passport Stamp Weights
{% endembed %}
