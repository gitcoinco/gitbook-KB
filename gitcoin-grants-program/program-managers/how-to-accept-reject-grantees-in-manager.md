# How to Accept/Reject Grantees in Manager

_At the time of writing, grant reviews in Manager are very rudimentary. Most of the work will rely on the round operator(s) coming to a consensus on the approval or denial of a given grant outside of the protocol. After that decision has been made it will be implemented in the protocol via signing an on-chain transaction. It’s important to note that applications cannot be submitted while a round is running, but grant review decisions can be made at any time during the round. Reviews can also be reversed; accepted applications can be rejected at any point before or during the round and vice versa._

### Grant Review Steps

For a single grant application, review decisions can be made by clicking on the application in Manager and clicking Approve or Reject. This will initiate a transaction, and once approved the grant will move from the ‘Received’ tab to either ‘Approved’ or ‘Rejected’.

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-11 at 11.09.28.png" alt=""><figcaption></figcaption></figure>

Multiple reviews can be batched in a single transaction to reduce gas fees. This is done by clicking ‘Select’ at the top right of the ‘received’ applications tab:

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-11 at 11.09.37.png" alt=""><figcaption></figcaption></figure>

This will then show two boxes in the top right corner of each grant - one for approval, and one for rejection. Click on the box corresponding to the decision for each grant you want to batch into the transaction, then click ‘Continue’ at the bottom right of the page. This will initiate a single transaction for all the decisions made, and once approved all of those grants will be moved to the ‘Approved’ or ‘Rejected’ tabs.

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-11 at 11.09.47.png" alt=""><figcaption></figcaption></figure>

Grant review decisions can be adjusted mid-round, i.e. an accepted grant can be switched to denied or vice versa. This will require another on-chain transaction and the steps are identical to the initial review. If there are multiple grants whose decisions are being reversed, they can be batched together into one transaction as well. However, if they are already approved you will only see an option to reject:

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-11 at 11.09.55.png" alt=""><figcaption></figcaption></figure>

And if they are already rejected you will only see an option to approve:

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-11 at 11.10.03.png" alt=""><figcaption></figcaption></figure>

#### Gas Fees

The gas fees for these transactions will vary depending on network choice and congestion, however, batching multiple grant review decisions into one transaction will have a negligible impact on the gas fee and it will be comparable to approving or denying a single grant. For this reason, we highly recommend working through grant reviews and marking down decisions off-chain before coming back to Manager and batching all the decisions together into a single transaction.

#### Adding Questions & Requirements in Round Manager

Manager has built-in functionality to add a round description and a set of requirements that will show up above the ‘Apply’ button when grantees are about to start their applications. This is a great way to make sure the eligibility criteria are clear and visible to grantees before they apply to the round.

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-11 at 11.10.11.png" alt=""><figcaption></figcaption></figure>

On the next page, round managers are able to add questions to the ‘Application Information’ section and can toggle between making these optional or required. These will appear for the grantee in the application flow and can be used to make the grantee self-certify that they meet certain criteria and/or answer questions that might impact the reviewer’s decision about their application.

<figure><img src="../../.gitbook/assets/Screenshot 2023-02-11 at 11.10.18.png" alt=""><figcaption></figcaption></figure>

Ideally, by the time the grantee reaches this part of the application flow, they will have a crystal clear picture of the eligibility criteria. They will then submit their application that \*should\* be accepted, or they will realize they are not eligible and cancel their application before submitting any on-chain transactions. The better the criteria and round details are designed, the easier it will be on the round manager down the line.&#x20;

### General Tips for Grant Reviews

Determining eligibility criteria for a grant round can be difficult. You want to strike a balance between being inclusive and supportive to potential grantees but also implementing requirements that weed out any scams, impersonators, or low-quality projects. To see what requirements we implemented for our Protocol Alpha Round, check out [this document](https://docs.google.com/document/d/1I4U3RA-q9ZW\_Mtlz-EiFtj4YZTkPEwebQSKbEZlCfdY/edit#heading=h.kl4qenhpok7z) which contains information on general platform eligibility as well as round-specific criteria.
