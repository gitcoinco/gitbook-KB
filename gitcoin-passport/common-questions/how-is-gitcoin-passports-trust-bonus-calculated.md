---
description: Learn how Gitcoin Passport's scores are calculated.
---

# 🤔 How is Gitcoin Passport’s score calculated?

Matching weights for Passport holders will range between 50% and 150%.

The matching weight for a Passport holder is:

* _150%_ if their _Accumulated Partitioned Uniqueness_ (APU) score is above the median APU score.
* (_their APU score - minimum APU score_) / (_median APU score - minimum APU score_) _+ 50%_ if their APU score is below the median APU score.

By way of background, the [APU scoring method](https://docs.google.com/presentation/d/1h4\_hJdawGlf8VeJhdhJ5LKZfUh6PrBD\_0lLoDe7jwCM/edit?usp=sharing) maps scores to individual Passports according to the number of stamps and the uniqueness of their combination. It has the following properties:

* Scaled from 0 to 1 for straightforward interpretations
  * 0 = no stamps
  * 1 = all possible stamps
  * Median score = the APU score separating the higher half from the lower half of the APU scores of all the submitted Passports in cGrants.
* Scales linearly in the number of stamps while maintaining the same interpretation.
* It has a closed-form solution that is easy to implement.

For a complete breakdown of the Gitcoin Passport Stamp weights please check out below:&#x20;

{% embed url="https://github.com/gitcoinco/passport-scorer/blob/main/api/scorer/settings/gitcoin_passport_weights.py" %}
Gitcoin Passport Stamp Weights
{% endembed %}
