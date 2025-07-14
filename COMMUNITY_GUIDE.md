## Community Guide

[ZK-Kit](https://zkkit.pse.dev/) is a set of highly-optmized and audited libraries and utilities to empower ZK and MPC developers.

Before contributing please check if the functionality you want to implement does not exist in part or in whole in one of the existing libraries. If it does, please consider improving or extending it instead.

### Contributing new libraries or utilities:

When proposing a new library, please consider the following:

- **Broad utility**: Encapsulates a common primitive or a frequently-used utility
- **Security**: The library should be well-tested, and not widely advertised till after it has been reviewed and audited
- **Optimization**: To the extent possible, the code optimizes 'hot spots' while striving for good readability. In-code comments and good documentation are especially essential for hand-optmized code segments that may not be easily readable
- **Documentation**: Good and up-to-date documentation in code, in the README of each package, and in the official ZK-Kit documentation site

### Refactoring or extending existing libraries:

Before contributing a refactor or an extension to an existing code, please:

- Open a new issue and tag the package owner
- Describe the rationale and the improvements your contribution can bring
- If applicable, provide example(s) to support that if any
- Provide at least a sketch of how you intend on coding it up. It is particularly important to highlight a "`diff`" showing how your contribution alters the interface -if it does
- Share the issue on the [community channel](https://discord.com/channels/943612659163602974/1181613897871007834) for wider feedback

### Reporting a bug

If you find a bug please do not open a new issue. Instead, please contact the package maintainer listed in the `.github/CODEOWNERS` file of the respective repository, and/or send an email to security@pse.dev.

### Contributing new libraries

Please refer to each repo for its tailored instructions:

- [zk-kit.circom](https://github.com/privacy-scaling-explorations/zk-kit.circom/blob/main/CONTRIBUTING.md)
- [zk-kit.solidity](https://github.com/privacy-scaling-explorations/zk-kit.solidity/blob/main/CONTRIBUTING.md)
- [zk-kit.js](https://github.com/privacy-scaling-explorations/zk-kit/blob/main/CONTRIBUTING.md)
- [zk-kit.rust](https://github.com/privacy-scaling-explorations/zk-kit.rust/blob/main/CONTRIBUTING.md)
- [zk-kit.noir](https://github.com/privacy-scaling-explorations/zk-kit.noir/blob/main/CONTRIBUTING.md)

### Testing

Good libraries provide a self-contained and coherent functionality with an unambigeous interface, and so writing tests should be straight forward.

If you find yourself needing to write too many different tests, please consider how you designed your interface. Does the library need to be broken down into two or more?

### Coding conventions

Following good coding practices is crucial to maintaining the reliability and readability of ZK-Kit. Adhering to the project's conventions ensures a consistent codebase and makes collaboration smoother for all developers.

- Please use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- Ensure you code is well formatted and has ran through the linter setup in the repository.
- Documentation:
  - In-code comments: please add top and by-line comments to help developers understand your library, providing links for further reading in the package README.
  - Package README: Every package must include a `README.md` file. It should ideally contain the following:
    - Brief description: A short summary of what the library does.
    - Installation instructions: How to install and import the library.
    - Example usage: A minimal working example that demonstrates how to use the library effectively.
- MIT-licensed: if you are contributing a new package, it must be MIT-Licensed.

### Governance

- Dispute handling
  - At this time, PSE will be handling any disputes. This might change as more partners are onboarded as mantainers.
- Ownership of packages
  - Packages are usually owned by their primary developer, however this can be adjusted based on requests from potential collaborators.
- Onboarding of new governors
  - Please reach out to PSE and the other governors to discuss this
- Audits and expenses will be discussed on a case by case basis with partners
