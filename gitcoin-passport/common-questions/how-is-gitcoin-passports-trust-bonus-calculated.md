---
description: Learn how Gitcoin Passport's scores are calculated.
---

# 🤔 How is Gitcoin Passport’s score calculated?

The Gitcoin Grants Round is a program that allows anyone to donate to open-source projects they like. However, only contributions made by individuals with high enough Passport scores will be eligible for matching funds. In order to be eligible for matching funds, participants must have a Passport score of 21.8 or above.

The Passport score is calculated based on the data points verified in the participant's Passport. Each data point is assigned a specific weight, which is used to determine the Passport score. \
\
Some example of scoring weights for each data point are listed below:

GITCOIN\_PASSPORT\_WEIGHTS = { \
"Brightid": 1.6, \
"CommunityStakingBronze": 2.5, \
"CommunityStakingGold": 1.8, \
"CommunityStakingSilver": 2.2, \
"Discord": 1.6, \
"Ens": 1.7, \
"EthGTEOneTxnProvider": 1.6, \
"Facebook": 1.6, \
"FacebookProfilePicture": 1.6, \
"FiftyOrMoreGithubFollowers": 1.5, \
"FirstEthTxnProvider": 1.6, \
"FiveOrMoreGithubRepos": 1.7, \
"ForkedGithubRepoProvider": 1.7, "GitPOAP": 2.8, "GitcoinContributorStatistics#numGr14ContributionsGte#1": 1.7, "GitcoinContributorStatistics#numGrantsContributeToGte#1": 1.6, "GitcoinContributorStatistics#numGrantsContributeToGte#10": 1.6, "GitcoinContributorStatistics#numGrantsContributeToGte#100": 1.5, "GitcoinContributorStatistics#numGrantsContributeToGte#25": 1.5, "GitcoinContributorStatistics#numRoundsContributedToGte#1": 1.6, "GitcoinContributorStatistics#totalContributionAmountGte#10": 1.7, "GitcoinContributorStatistics#totalContributionAmountGte#100": 1.6, "GitcoinContributorStatistics#totalContributionAmountGte#1000": 1.9,

The specific weights of all the data points are here:

{% embed url="https://github.com/gitcoinco/passport-scorer/blob/main/api/scorer/settings/gitcoin_passport_weights.py" %}
Gitcoin Passport Stamp Weights
{% endembed %}

You can find more user-friendly descriptions of the different data points in the Passport stamps:&#x20;

{% embed url="https://passport.gitcoin.co/#/dashboard" %}
Gitcoin Passport Protocol
{% endembed %}
