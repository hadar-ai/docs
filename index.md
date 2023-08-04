# Hadar

**Platform for creative data publishing and ethical sourcing for AI**

## Overview

In the AI landscape, the value of data is undeniable, yet often, creators find their work utilized freely for AI training without their consent or compensation.

Hadar is stepping in to transform this dynamic. We're establishing a platform that empowers creative communities to share, control, and monetize their content for AI training and fostering a space for genuine collaboration and fair compensation. Through strategically designed tokenomics, our platform encourages high-quality content datasets that can be monetized, with profits linked to their future use and inherently tied to the quality of the content.

Essentially, Hadar is revolutionizing how creative content is shared, utilized, and remunerated in the AI sphere, thereby initiating a new era of creative data accessibility, content creator recognition, and creative innovation.

## How it works

### Stakeholders

In the Hadar ecosystem, there are 4 key roles: **Data Consumers**, **Data Supplier**, **Data Annotators**, **Sponsors**. Each role serves a unique function and has specific responsibilities, costs, and rewards.  It’s important to note that these roles are not mutually exclusive - we anticipate and encourage users to adopt multiple roles

|               |                                                               |                                                                      |                                       |
| :-----------: | :-----------------------------------------------------------: | :------------------------------------------------------------------: | :-----------------------------------: |
| **User Role** |                          **Actions**                          |                             **Rewards**                              |               **Costs**               |
|   Consumers   |         Access and use unique art data for AI models          |             High-quality, unique, and diverse datasets.              | Charged based on type, size of data.  |
|   Suppliers   |                         Publish data                          |         Ensure proper attributions and earn from its usage.          | Time, effort to curate, share, label. |
|  Annotators   | Annotate the data with additional attributes to aid training. |                           Earn HAD tokens.                           |     Time and effort to annotate.      |
|   Sponsors    |          Fund the project or tasks on the platform.           | Visibility, potentially earn a return if project/task is successful. |         Financial investment.         |

#### Consumers

These are individuals or entities, such as AI developers, academic researchers, or businesses that seek to leverage the rich, unique content for various purposes. They can access these curated datasets via our API and will be charged based on the type, size, and complexity of data they require.

#### Suppliers

These are primarily artists and creators who own and produce the creative work, as well as platforms like online content curation websites. Suppliers can share, label, verify the quality and authenticity of the content, ensuring that proper attributions are maintained and content creators are fairly compensated. They can control how their work is used in AI training while earning from its usage.

#### Annotators

These are individuals or entities that annotate the data supplied by Suppliers. They can apply to be annotators and tag themselves with relevant areas of expertise. They enhance the quality of datasets on the platform, and play a critical role in doing so.

#### Sponsors 

These are individuals, businesses, or organizations that fund the projects or tasks on the platform. Sponsors can gain visibility, contribute to the growth of the content and AI ecosystems, and potentially earn a return if the project or task they sponsor is successful.

Each role is designed with specific responsibilities and rewards to maintain a balanced, self-sustaining data ecosystem. We invite you to contribute, learn, and profit in a way that suits your capabilities and needs.

### Data Provisioning Process 

Community members who have access to valuable datasets can act as Suppliers to publish datasets, set price terms, foster competition, and promote the evolution of data resources through natural market choice.

1. A Supplier uploads a new dataset and describes its features using metadata.
2. The Supplier can optionally request Annotators to enhance the quality of the uploaded data. Automated Quality Control integrated into the platform will assess all uploaded data regardless of this choice.
3. The Supplier sets price terms for accessing the data. They can also choose to make the dataset free of charge, opting out of earning from Data Consumer access.
4. The dataset becomes publicly available to download or streamed via the platform's API.

### Annotation

Annotators are individuals or entities who wish to enhance the metadata of data by tagging it with additional labels and attributes. Good annotations enhance the value of a dataset by making it possible to train models on the data more accurately.

Initially, all annotation work will be vetted by the Hadar team prior to acceptance into the dataset. Successful annotations will be rewarded in the form of our platform token - HAD (see below).

Over time, as the no. of annotations and overall platform activity scales upwards we will introduce a more decentralized mechanism of vetting annotations.

### Pricing and Payments

The platform is designed to be self-sustaining. It accomplishes this through priced access to data as well as monetary incentives for users who contribute high-quality datasets. All bid/offer pricing and API fees are denominated in USD (US dollars).

#### Data Consumption and Payment

Consumers can access the datasets through API requests. The cost of accessing these datasets is set by the data Suppliers. These costs are automatically deducted from the consumer's account or charged to their credit card. The revenue from the API requests is then split between the platform and the original Suppliers of the data.

#### Transaction and Usage Records

- **Usage History:** Consumers have access to their usage history, which gives a detailed account of their data consumption. This includes the number of API requests, the datasets accessed, the total cost incurred, and the timestamp of access.
- **Invoice Generation:** On a monthly basis, an invoice is generated for consumers. The invoice includes a breakdown of all the API requests and the corresponding costs.

#### Dispute Resolution

If consumers have any disputes regarding their usage or the billed amount, they can raise a dispute. The platform will then review the dispute and take appropriate action based on the evidence provided and the platform's policies.

#### Pricing

#### Set by Suppliers

**Per-row micro-transaction pricing**: This model charges consumers for every individual row of data they access. It's a granular approach that allows for maximum flexibility in how much data a consumer wants to purchase and use.  
The price of the dataset will be locked in for the given Consumer’s lifetime usage of the dataset. Suppliers can update the dataset price at any point in time, but it will only impact the future Consumer’s cost.

#### Base Cost for Data Consumption

Aside from the specific pricing models set by Data Suppliers, there will be a base cost associated with consuming data via the platform. This cost is measured in USD per gigabyte accessed via the API. The exact cost will be determined closer to the platform's production launch once our infrastructure costs are finalised.

#### Commission Structure

To support the ongoing development, maintenance, and improvement of the platform, a 20% commission is applied to the earnings of Suppliers.

#### Sponsoring Data Access

For users who wish to sponsor the cost of accessing one or more datasets, they can follow the following process

1. **Dataset Selection:** A sponsor begins by selecting a dataset they wish to sponsor. This could be based on the potential social impact, commercial value, or the sponsor's specific interest in the dataset's subject matter.
2. **Funding Allocation:** Next, the sponsor adds capital to the platform to cover the costs of consumers accessing the sponsored dataset.
3. **Sponsorship Announcement:** Upon successful allocation of funds, the sponsor can proceed to announce their sponsorship. The platform will label the sponsored datasets, helping consumers identify datasets that can be accessed freely or at a reduced cost.
4. **Monitoring Sponsorship Usage:** Sponsors can track the usage of their sponsored datasets. The platform provides detailed statistics, such as the number of consumers using the sponsored dataset, total costs incurred, and remaining sponsorship funds. This data should help sponsors understand the impact of their sponsorship and plan future sponsorships.
5. **Top-Up or End Sponsorship:** Depending on the usage and the sponsor's intent, they can choose to add more funds to continue the sponsorship or decide to end the sponsorship when the allocated funds are exhausted. Upon ending the sponsorship, the dataset will no longer be labeled as sponsored on the platform.

This sponsorship model fosters data democratization by encouraging the availability of datasets to a wider user base, promoting research and development, and potentially uncovering innovative use cases.

#### Payment Currency

All dataset access is priced in USD. The preferred payment currency is also USD and/or the USDC stablecoin. This is to ensure predictability for both Consumers and Suppliers.

In all cases, users can freely withdraw their funds from the platform, offering them full control over their earnings.

In the future, once our platform token - HAD - is established and distributed amongst our community, we may enable HAD as an optional alternative currency with which to make and receive payments.

### Additional Features

#### Automated Quality Control

Our platform will provide automated tools and plugins to measure data completeness and validity. Automated quality control measures include:

- **Completeness**: Check for missing, duplicate, outlier, or null values
- **Validity**: Check for formatting errors, such as inconsistent data types

These checks are standard, publicly disclosed, and flag data that falls below a specified threshold. Suppliers may reduce or require additional automated checks, and Suppliers are mandated to rectify or provide explanations for flagged data.

#### Open-source data verification tooling

Because data will not be downloadable via our API until it has been finalized, we will provide a system whereby stakeholders can develop and upload additional tooling for data verification within our online interface. This will give stakeholders the flexibility they need to run custom heuristics against the dataset for validity purposes, while at the same time enhancing the overall value of our ecosystem thanks to new and improved tooling.

#### Versioning

We will implement version control for datasets. Specifically, there will be per-row version control. This will enable all parties who modify and curate dataset rows to track changes and roll back if necessary.

In addition, we will enable per-dataset change tracking. Once some rows have been modified and signed off as final, the system will increment the overall dataset version. This enables consumers to know when a newer version of the dataset is available as well as make sure that the version they’re currently using doesn’t change due to new data.

#### Subset-tagging

Suppliers, when uploading data, are required to provide rich metadata to facilitate seamless data search.

We will allow for subsets of a dataset to be tagged with additional labels. Such tagged subsets will then be fetchable via the API. This will allow users to train models on subsets of a dataset that may have particular properties that are useful to them.

Tagging will usually be done by Suppliers and Annotators on a row-by-row basis. Batch tagging of a selection of rows will also be possible.

#### Centralized Storage

Our platform utilizes commercial cloud-hosting services for data storage to optimize data availability and manage costs effectively. To ensure low-latency access worldwide we will employ CDNs and Edge functions where necessary.

## Community governance

We want our community to be actual stakeholders in our platform. With this in mind, we aim to introduce our community cryptocurrency token - HAD - as both a means of rewarding engagement with our platform and providing a voice for community members in shaping the future of the platform and ecosystem.

HAD is minted on Ethereum, a blockchain network that uses an environmentally friendly proof-of-stake consensus algorithm and is secured by $40 billion+ of distributed capital.

### Staking

Holders of our HAD community token can “lock” some or all of their HAD balance within the platform in the form of “staking”. Doing this increases the scarcity of HAD and is ultimately beneficial to our community. As a reward for staking, holders will obtain:

- Discounts on the fees charged by the platform to Data Consumers.
- Discounts on the fees taken by the platform from the earnings of Data Suppliers.

We also plan to investigate whether it is legally possible for us to distribute platform profits to stakers.

### Treasury

All platform earnings contribute to the platform's treasury, which is partially under community governance.

Additionally, all HAD earned by other stakeholders and platform contributors will be paid out from the treasury. The treasury also receives all HAD paid in by platform contributors. We aim to be self-sustaining over time.

### Distribution

HAD tokens will initially only be available through engagement with the platform. We will detail the tokenomics of our token in the near future.
