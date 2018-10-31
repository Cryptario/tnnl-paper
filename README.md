## tnnl: A Privacy Layer for Standards-Compliant Fungible Tokens

**ABSTRACT:** The current Ethereum token-oriented ecosystem is lacking in
privacy. With the 'Byzantium' hard-fork to the Ethereum network,
it became possible to implement a confidential transaction system
using zk-SNARKs; however, with a preexisting token infrastructure,
it is a non-trivial amount of work for current tokens that are in
want of privacy features to incorporate the technology enabled by
the latest hard-fork. We propose a system that provides 
_all_ preexisting ERC20-compliant, ERC223-compliant, ERC677-compliant, and ERC777-compliant tokens
a means of operating in a confidential manner.

[Read the full introductory "dark" paper and protocol specification!](../master/tnnl.pdf)

## FAQ

*For all unanswered questions that you may have, please open an issue and we'll be sure to respond and update our README when possible (at time of last commit, we're currently fighting poor cellular and WiFi networks in Prague).*

**Q:** How much gas does a transaction use?
<br />
**A:** Due to the current gas prices, a *tnnl* transaction costs about 1.45M gas. There is an EIP (1108) that should help reduce this cost.

**Q:** There are a few things in the procotol specification that are not instantiated. What are the these exact values?
<br />
**A:** Not all values have been decided on since implementation is not yet fully complete. We are open to suggestions from the community for much of these, so if you see a ***CONST*** or value not explicitly instantiated that does not yet have an existing issue, please open an issue to start a discusssion on the possible values it could be given.

**Q:** Does '*tnnl*' stand for anything?
<br />
**A:** Not really, no. It's a decent mispelling of '*tunnel*' that we were able to get a domain for. 😉

**Q:** Will there be an ICO?
<br />
**A:** No. *TNL* — which is how we refer to the *network token* (with a defensive acronym of '*tnnl* Network Laborage') — will be primarily distributed via a mining process. We're not fans of ICOs.

**Q:** Are there any hardware/software requirements?
<br />
**A:** Yes, but the exact specifications of the base-line requirements are to be determined as implementation progresses. Currently, it is estimated that 4GB of RAM is required for generating proofs. This proof generation program *can* be run inside a Docker container.

**Q:** Does *tnnl* suffer form the same problem as Zcash, where a trusted setup is required?
<br />
**A:** Unfortunately, yes. We will have to go through our own key generation ceremony since out circuit differs from Zcash's. It should be a *blast*.

**Q:** When will the code be made public?
<br />
**A:** There needs to be some cleanup and documentation before our code can be made public (there's some gross C++, and we recognize that some of our code is not yet comprehensible to mortals). That being said, we're frantically working on this to get this public ASAP, so other open-source developers can contribute.
