# Addition of neighbor snooping into FRR 

A missing feature in FRR is neighbor snooping to ensure that Zebra is aware of neighbors that the kernel cannot detect on its own. This design document is intended to help us define and agree on the final architecture for this new FRR feature.

The goal of this documentation is to expose the following:

- Which scenarios do we aim to solve with this new snooping function?
- What technical choices will we make in designing this new feature?
- What limitations in the current FRR design need to be assessed?
- What future additions do we expect after snooping is introduced into FRR?
- And, what choices should we take now to make those future additions easier to move forward?

The structure of this repository is as follows:  

| Directory       | Purpose                                           |
| --------------- | ------------------------------------------------- |
| `architecture/` | Architectural desgn                               |
| `scenario/`     | Different scenarios we need to be able to support |
| `future-work/`  | Ideas beyond this project                         |
| `decisions/`    | Architecture decisions                            |

The main design document for the Neighbor Manger be found [neighmgr](architecture/neighmgr.md).

## How to Contribute

Design discussions should occur via GitHub pull requests.

Suggested workflow:

1. Create or update a design document  
2. Open a PR  
3. Discuss trade-offs  
4. Once consensus is reached, record a decision in `decisions/`

An example decision Architecture Decision Record (ADR) can be found [here](decisions/000-template.md).
