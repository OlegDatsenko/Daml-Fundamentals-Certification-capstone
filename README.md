# ESG Solar Projects
Daml templates designed for a platform to initiate solar projects, tokenize them and trade/exchange the tokens between community members.

### I. Overview 
Background: The adoption of renewable energy sources is a key part of ESG initiatives. Solar power projects can provide clean, sustainable energy while benefiting the environment and the community. However, financial barriers may limit the participation of local communities in such projects. Tokenization and fractional ownership can help break down these barriers by allowing individuals to invest in and benefit from local solar power projects.
Project Description: DAML-based platform that allows individuals to participate in community solar projects through the purchase and trading of tokenized solar energy shares. These tokens will represent a fractional ownership in the solar project and can be bought, sold, or traded among community members.
Key Features:
Solar Project Registry: registry of approved community solar projects that are available for investment. This includes key project details such as location, capacity, and estimated annual energy production.
Tokenization: a smart contract-based system for tokenizing each solar project, with each token representing a share of the project’s ownership.
Trading Platform: a decentralized trading platform that enables the exchange of solar energy tokens between community members.

### II. Workflow
  1. initiator creates a Solar project Proposal contract     
  2. approver review the proposal by exercising the choice ReviewSPProposal
  3. initiator exercises TokenizeSP on his(her) solar project with tokens amount and names a tokens lot
  4. token lot owner exercises Offer with a community members list, token lot price parameters and token amount owners wants to trade
  5. community member exercises Accept so he(she) becomes a new owner of a token lot.

### III. Compiling & Testing
To compile and test, run the pre-written script in the `Main.daml` under /daml OR run:
```
$ daml start
```
