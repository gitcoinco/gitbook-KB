---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 🔺 AVAX Custom Scorer

Gitcoin allows communities to give higher priority to specific Stamps they find particularly significant. For the AVAX community, we have created a tailored scoring system.

\
According to this custom scoring model, participants in the Avalanche Community Grant Rounds must attain a score exceeding 25 to be eligible for voting. The only way to achieve this score is through verification using Civic Uniqueness or Holonym stamps. These stamps are available on The Avalanche network.

### How it works&#x20;

Have a step-by-step of the dashboard&#x20;

[https://passport.gitcoin.co/#/dashboard/avalanche](https://passport.gitcoin.co/#/dashboard/avalanche)&#x20;

### How to get the stamp?

* [Holonym Guide](https://support.gitcoin.co/gitcoin-knowledge-base/gitcoin-passport/how-do-i-add-passport-stamps/guide-to-add-holonym-stamp-to-gitcoin-passport)
* [Civic Guide](https://support.gitcoin.co/gitcoin-knowledge-base/gitcoin-passport/how-do-i-add-passport-stamps/civic-stamp-verification-guide-for-gitcoin-passport)

### What about my donation matching?&#x20;

For rounds running on Avalanche, once you’ve achieved a Passport score of 25 by verifying with either of the stamps listed on this [Avalanche-specific Passport dashboard](https://passport.gitcoin.co/#/dashboard/avalanche), you’ll see your new score updated on the round’s Explorer page. A Passport score of 25 means that you’ll be eligible for 100% of your donation match on Grants Stack.&#x20;

### How is the Passport Score Calculated for Participants in the Avalanche Round with Civic or Holonym Stamps?

Participants from the Avalanche round will observe their standard Passport score displayed on the Passport dashboard. Upon successful verification through Civic or Holonym stamps, the user interface (UI) will indicate an increase of +6.07 or +5.04 points, respectively. However, it is important to note that the Avalanche Custom Scorer API internally assigns a value of +25 points for either of these stamps.&#x20;

For example, if an individual verifies exclusively with the Civic stamp, while their Passport score displayed on the UI will be 6.07 points (as per the default Passport scoring system), their adjusted score in the Avalanche scenario would actually be 25 points.
