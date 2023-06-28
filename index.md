Decentralized platform for high-quality, incentivized data curation and access

# Overview

In the rapidly evolving field of AI, data has become a crucial asset. However two significant challenges are hampering progress: data isolation by large enterprises, and the difficulty of sourcing specialized data from niche verticals.

Enterprises often guard their data closely, treating it as a proprietary asset. This creates an environment where innovation is stifled, and collaboration becomes difficult. Likewise, when developing AI models, access to diverse, high-quality datasets is crucial. These datasets, particularly in niche areas, are often scattered and hard to obtain.

Hadar is our answer to these challenges. We envision a decentralized data bank, openly curated by the crowd, with accessibility at its core, aiming to democratize data and ignite innovation.

By employing tokenomics, a system that uses tokens to incentivize specific behaviors, our platform encourages users to request, provide, verify, and maintain datasets. The contributors to these datasets stand to profit from their future use, the value of which is inherently tied to the data quality.

Through Hadar, we aim to empower data scientists, researchers, and innovators, providing them with the specific data they need, regardless of their niche vertical.

# How does it work

## Stakeholders

In the Hadar ecosystem, there are five key roles: Consumers, Curators, Suppliers, Verifiers, and Sponsors. Each role serves a unique function and has specific responsibilities, costs, and rewards.  Important to note that these roles are not mutually exclusive - we anticipate and encourage users to adopt multiple roles, fostering a dynamic, multi-faceted participation within the system.

|               |                                                 |                                                                                    |                                                                   |
| :-----------: | :---------------------------------------------: | :--------------------------------------------------------------------------------: | :---------------------------------------------------------------: |
| **User Role** |                   **Action**                    |                                     **Reward**                                     |                             **Cost**                              |
|   Consumer    |                   Access data                   |                                        None                                        |                    Pay for accessing datasets                     |
|    Curator    |  Request and verify datasets; set price terms   |                   Paid for consumer usage of requested datasets                    | Pay suppliers and verifiers (if employed)  for dataset collection |
|   Supplier    | Provide high-quality datasets;  set price terms |  Paid for consumer usage of provided datasets and by curators for data provision   |                               None                                |
|   Verifier    |           Verify datasets for quality           | Paid for consumer usage of verified datasets and by curators for data verification |                               None                                |
|    Sponsor    |       Sponsor cost of accessing a dataset       |                 To be determined (recognition, tax benefits, etc.)                 |              Cover the costs of accessing a dataset               |

### Consumers

Users, such as data scientists, researchers, or businesses, who use datasets available in our database to train AI models, analyze trends, or make informed decisions. Consumers access these datasets via our API and are charged based on the type, size, and complexity of data they require.

### Curators

Users who place requests for datasets and allow Data Suppliers to bid on fulfilling those requests. Curators also set verification criteria that could be fulfilled by themselves or by Data Verifiers. They are responsible for setting price terms and signing off on the quality of datasets prior to them being made available for use by Data Consumers. Curators play a crucial role in maintaining the quality and diversity of data in the ecosystem.

### Suppliers

Entities or individuals who supply/upload datasets for entry into the database. They can upload datasets on an ad-hoc basis, set pricing terms, and/or fulfill the dataset requirements of Data Curators. Suppliers are incentivized to provide high-quality and diverse datasets to increase their visibility and potential revenue on the platform.

### Verifiers

Community members who vet the quality of the data entered by Suppliers. Verifiers are an optional, but valuable add-on. They can apply to be a verifier and tag themselves with relevant areas of expertise. They play a key role in ensuring the authenticity and quality of datasets on the platform.

### Sponsors

Users who put up liquid capital to pay for the cost of accessing one or more datasets. Sponsors could be philanthropic entities, businesses investing in AI research, or even governments. They play a crucial role in supporting the data ecosystem and fostering innovation.

Each role is designed with specific responsibilities and rewards to maintain a balanced, self-sustaining data ecosystem. We invite you to contribute, learn, and profit in a way that suits your capabilities and needs.

## Data Provisioning Process 

The following diagram gives a brief overview of all how each of the aforementioned types of users uses the platform and interacts with each other:

###

### Supplier-Led Dataset Publishing

In the absence of specific Curator requests, our platform is still open for Suppliers to upload datasets, set price terms, foster competition, and promote the evolution of data resources through natural market choice.

#### Process Flow

1. A Supplier uploads a new dataset and describes its features using metadata.
2. The Supplier can optionally request Verifiers to ensure the quality of the uploaded data. Automated Quality Control integrated into the platform will assess all uploaded data regardless of this choice.
3. Following verification, the Supplier sets price terms for accessing the data. They can also choose to make the dataset free of charge, opting out of earning from consumer access.
4. The dataset becomes publicly available via the platform's API.
5. If Verifiers were involved in the process, they receive a portion of the revenue generated from consumers accessing the data. However, if the dataset was made free of charge, no earnings are allocated to the Verifiers.

### Curator-Led Dataset Publishing

Curators initiate data requests and select from bids offered by Suppliers and optionally, Verifiers. Data is uploaded, verified, and improved if necessary, before final approval and release.

#### Part I Curator-Led Data Request and Bid Selection

1. **Curator creates a Tender:** The Curator initiates the process by creating a tender, outlining the specific features and requirements of the desired dataset. Criteria need to be made public, examples include

   - **Relevance**: The data is relevant to the research question or use case.
   - **Completeness**: The data is comprehensive and includes all relevant information.
   - **Accuracy**: The data is accurate and verified through external sources, if necessary.
   - **Consistency**: The data is consistent and contains no obvious discrepancies.
   - **Validity**: The data is valid and meets any required formatting standards.

They may also call for independent Verifiers to participate in the process. For extremely niche data sets, the Curator should expect to receive more costly bids. And vice versa.

2. **Bidders Respond:** Suppliers and, if requested, Verifiers respond to the tender by submitting their respective bids for data supply and verification.
3. **Bid Matching**: The Curator selects desirable bids from both Suppliers and Verifiers. Upon this selection, the required tokens, covering all chosen bids collectively, are withdrawn from the Curator's wallet and escrowed by the platform.

#### Part II Data entry and quality control

1. **Dataset Submission:** The supplier submits the dataset into the database using various methods, such as API or direct upload.
2. **Quality Assurance:** The Curator and Verifiers inspect the data to validate its quality. They use platform-provided tools to ensure the data meets the tender requirements. The review will be conducted on the full data set, which will be made available through our platform dashboard interface.

- The data is not accessible via API at this stage. This prevents curators from using the data without quality sign-off, thus encouraging honesty and integrity in the process.
- Curators hold the final say on data quality. Verifiers can raise an issue and make recommendations on the final decisions.

3. **Sign-off and Reward Distribution**: If the Curator validates the data:

- The Suppliers and Verifiers receive tokens from the escrow, with the platform deducting a fee from their earnings.
- The dataset is then made accessible to all users via the platform API.

4. **Improvements and Deadlines:** if the Curator (or Verifier)  requests improvements:

- The tokens remain in escrow, and the data stays unavailable via the API.

- The Curator provides specific feedback, prompting Suppliers to submit updated data for another round of verification.

- There is a 180-day deadline for these changes.

  - If the Curator fails to sign off on the improved data within this period, approval is automatically assumed.
  - If the Suppliers do not submit the revised data within this period, the request is deemed a failure, and the Curator sign-off becomes impossible. In such a case, the escrowed tokens are returned to the Curator, and the dataset is discarded.

### Dispute Resolution Process

If a Supplier disputes a verifier's decision due to perceived inaccuracies, the following steps are taken:

1. **Dispute Initiation:** The Supplier initiates a dispute and stakes collateral amounting to 25% of the rewards they would have received had the data been approved.

2. **Independent Verifiers Selection:** The platform randomly selects a group of independent verifiers from a pool of trusted and qualified platform users, ensuring they possess the relevant expertise and experience.

3. **Data Evaluation:** The selected verifiers receive the disputed data and assess it using the same criteria as the initial verifiers.

4. **Dispute Resolution:**

- If the independent review concludes that the initial verifiers' reviews were unjust, the following occurs:

  - The staked collateral is returned to the Supplier.
  - The Supplier is compensated, and the data is accepted into the database.
  - The independent verifiers share the revenue generated from future API consumption requests.

- If the independent review corroborates the initial verdict:

  - The dispute is deemed resolved.
  - The staked collateral is confiscated from the Supplier and divided evenly among the independent verifiers.
  - The disputed data is removed from the platform.

This process aims to maintain the integrity and reliability of the platform's datasets by ensuring a fair and unbiased review system.

## Pricing and Payments

The platform is designed to be self-sustaining. It accomplishes this through priced access to data as well as monetary incentives for users who contribute and verify high-quality datasets. All bid/offer pricing and API fees are denominated in USD.

### Data Consumption and Payment

Consumers can access the datasets through API requests. The cost of accessing these datasets is set by the data suppliers or curators. These costs are automatically deducted from the consumer's account or charged to their credit card. The revenue from the API requests is then split between the platform and the original curators, verifiers, and suppliers of the data.

#### Transaction and Usage Records

- **Usage History:** Consumers have access to their usage history, which gives a detailed account of their data consumption. This includes the number of API requests, the datasets accessed, the total cost incurred, and the timestamp of access.
- **Invoice Generation:** On a monthly basis, an invoice is generated for consumers. The invoice includes a breakdown of all the API requests and the corresponding costs.

#### Dispute Resolution

If consumers have any disputes regarding their usage or the billed amount, they can raise a dispute. The platform will then review the dispute and take appropriate action based on the evidence provided and the platform's policies.

### Pricing Models

#### Set by Curators and Suppliers 

Data suppliers and curators have the flexibility to customize the pricing for their datasets, providing scalability and versatility for data consumers. Here are the possible pricing models:

- **Per-row micro-transaction pricing**: This model charges consumers for every individual row of data they access. It's a granular approach that allows for maximum flexibility in how much data a consumer wants to purchase.
- **Bulk batch pricing:** This model offers pricing tiers based on the size of the data batch accessed (e.g., 10k rows at price point A, 50k rows at price point B). It allows consumers to access large amounts of data at a reduced cost per row.
- **Single price for the entire dataset:** This model sets a flat rate for access to the entire dataset. It's the simplest and most straightforward model, particularly useful for consumers who know they need access to all the data in a given dataset.

#### Base Cost for Data Consumption

Aside from the specific pricing models set by suppliers and curators, there will be a base cost associated with consuming data via the platform. This cost is measured in USDC or USD per gigabyte accessed via the API. The exact cost will be determined closer to the platform's production launch once our infrastructure costs are finalized.

#### Commission Structure

To support the ongoing development, maintenance, and improvement of the platform, a commission on revenue earned by curators, suppliers, and verifiers is charged:

- New dataset creation payouts: The platform takes a one-off 25% commission from the earnings of suppliers and verifiers for new dataset creations.
- API consumption payouts: A 20% commission is also applied to the earnings of suppliers, verifiers, and curators for API data consumption.

### Sponsoring Data Access

For users who wish to sponsor the cost of accessing one or more datasets, they can follow the following process

1. **Dataset Selection:** A sponsor begins by selecting a dataset they wish to sponsor. This could be based on the potential social impact, commercial value, or the sponsor's specific interest in the dataset's subject matter.
2. **Funding Allocation:** Next, the sponsor adds capital to the platform to cover the costs of consumers accessing the sponsored dataset. This capital can be added using various methods supported by the platform.
3. **Sponsorship Announcement:** Upon successful allocation of funds, the sponsor can proceed to announce their sponsorship. The platform will label the sponsored datasets, helping consumers to identify datasets that can be accessed freely or at a reduced cost.
4. **Monitoring Sponsorship Usage:** Sponsors can track the usage of their sponsored datasets. The platform provides detailed statistics, such as the number of consumers using the sponsored dataset, total costs incurred, and remaining sponsorship funds. This data should help sponsors understand the impact of their sponsorship and plan future sponsorships.
5. **Top-Up or End Sponsorship:** Depending on the usage and the sponsor's intent, they can choose to add more funds to continue the sponsorship or decide to end the sponsorship when the allocated funds are exhausted. Upon ending the sponsorship, the dataset will no longer be labeled as sponsored on the platform.

This sponsorship model fosters data democratization by encouraging the availability of datasets to a wider user base, promoting research and development, and potentially uncovering innovative use cases.

### Payment Method

Users have flexibility in the form of payment they receive. They can choose to be paid in USDC, USD, or HAD our native tokens.

- **HAD Payments:** Users receiving payment in HAD have the added benefit of staking, subject to local laws and regulations.  The platform uses USDC revenue to purchase HAD from a DEX, which is then deposited into a staking contract on the recipient's behalf. Recipients can unstake their HAD at any time, offering them flexibility and control over their earnings.
- **USDC and USD Payments**: Users who choose to receive payment in USDC or USD will receive their funds directly, with no option to stake.

In all cases, users can freely withdraw their funds from the platform, offering them full control over their earnings.

## Additional Features

### Automated Quality Control

Our platform will provide automated tools and plugins to measure data completeness and validity. Automated quality control measures include:

- **Completeness**: Check for missing, duplications, outliers, or null values
- **Validity**: Check for formatting errors, such as inconsistent data types or invalid characters

These checks are standard, publicly disclosed, and flag data that falls below a specified threshold. Curators may reduce or require additional automated checks, and suppliers are mandated to rectify or provide explanations for flagged data.

### Open-sourced data verification toolings

Because data will not be downloadable via our API until it has been finalized, we will provide a system whereby stakeholders can develop and upload additional tooling for data verification within our online interface. This will give stakeholders the flexibility they need to run custom heuristics against the dataset for validity purposes, while at the same time enhancing the overall value of our ecosystem thanks to new and improved tooling.

### Versioning

We will implement version control for datasets. Specifically, there will be per-row version control. This will enable all parties who modify and curate dataset rows to track changes and roll back if necessary.

In addition, we will enable per-dataset change tracking. Once some rows have been modified and signed off as final, the system will increment the overall dataset version. This enables consumers to know when a newer version of the dataset is available as well as make sure that the version they’re currently using doesn’t change due to new data.

### Subset-tagging

Suppliers, when uploading data, are required to provide rich metadata to facilitate seamless data search.

We will allow for subsets of a dataset to be tagged with additional labels. Such tagged subsets will then be fetchable via the API. This will allow users to train models on subsets of a dataset that may have particular properties that are useful to them.

Tagging will usually be done by curators, suppliers, and verifiers on a row-by-row basis. Batch tagging of a selection of rows will also be possible.

### Centralized Storage

Our platform utilizes commercial cloud-hosting services for data storage to optimize data availability and manage costs effectively. To ensure low-latency access worldwide, we deploy serverless functions, such as Cloudflare Workers.

# Governance

Our platform is managed by a Decentralized Autonomous Organization (DAO) system which ensures that no single entity or person can make unilateral decisions about the data. This helps prevent data isolation and ensures that decision-making power is distributed among the community, promoting transparency and accountability. Our governance token, named HAD, has a capped supply of 10,000,000 tokens.

## Staking and Rewards

Stakeholders who acquire and stake HAD tokens on the platform are entitled to a proportionate share of our platform's revenue, specifically, 50% of the total.

Moreover, staking encourages active participation and increases the chances of selection for dataset verification tasks. Verifiers who maintain a stake exceeding 500 HAD for a period longer than 90 days have an increased probability of being chosen to verify a dataset. This likelihood is reflected in a verifier's "credibility" score visible next to their profile ID. The score integrates various factors, including the number of successful verifications, amount, and duration of staked HAD, among others.

## Treasury

All platform-generated fees, denominated in USD, contribute to the platform's treasury, which is under DAO governance. The DAO can vote to utilize a portion of the treasury funds to buy back and burn a part of the HAD circulating supply from the market. This action is intended to induce scarcity and drive further value to the token.

## Tokenomics

HAD tokens are only available through token sales and subsequent exchanges. This system ensures a controlled supply and a stable, predictable token economy. The self-sustaining economic model and aligned incentives across all users are designed to support a vibrant and thriving platform.

## Distribution

|                         |            |            |
| ----------------------- | ---------: | ---------: |
| **Total supply**        | 10,000,000 |            |
|                         |            |            |
| **_Vesting (months):_** |            |            |
| **Lock-up period**      |         12 |            |
| **Vesting duration**    |         48 |            |
|                         |            |            |
| **_Allocations:_**      |    **_%_** |            |
| **DEX liquidity**       |          5 |    500,000 |
| **Founders**            |         15 |  1,500,000 |
| **Employee pool**       |         15 |  1,500,000 |
| **Investors**           |         10 |  1,000,000 |
| **Advisors**            |          5 |    500,000 |
| **Launch partners**     |         10 |  1,000,000 |
| **Treasury**            |         40 |  2,000,000 |
|                         |            |            |
|                         |        100 | 10,000,000 |

## Licensing

All data will be under a [Creative Commons Attribution-ShareAlike](https://creativecommons.org/licenses/by-sa/4.0/) license.